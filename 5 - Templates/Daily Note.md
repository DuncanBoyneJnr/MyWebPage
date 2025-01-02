<%*
const dailyLogsFolder = "7 - Daily Logs"; // Folder for daily logs
const monthlyLogsFolder = "8 - Monthly Logs"; // Folder for monthly logs
const currentlyReadingFilePath = "6 - Main Notes/Currently Reading.md"; // Path to Currently Reading file
const completedReadingFilePath = "6 - Main Notes/Completed Reading.md"; // Path to Completed Reading file

const todayFileName = tp.file.title; // Today's note title (assumed format: DD-MM-YYYY)
const yesterdayFileName = tp.date.now("DD-MM-YYYY", -1); // Previous day in DD-MM-YYYY format
const yesterdayFilePath = `${dailyLogsFolder}/${yesterdayFileName}.md`; // Construct full path

let yesterdayTasks = [];
try {
    const yesterdayFile = app.vault.getAbstractFileByPath(yesterdayFilePath);
    if (!yesterdayFile) throw new Error(`File not found: ${yesterdayFilePath}`);
    const yesterdayContent = await app.vault.read(yesterdayFile);

    // Fetch "What Will I Do Today" tasks
    const taskMatches = yesterdayContent.match(/## What Will I Do Today:[\s\S]*?(##|$)/);
    if (taskMatches) {
        const tasks = taskMatches[0]
            .replace("## What Will I Do Today:", "")
            .trim()
            .split("\n")
            .filter(line => line.startsWith("-"));
        yesterdayTasks = tasks.map(task => task.trim());
    }
} catch (err) {
    console.error(`Error reading yesterday's file: ${yesterdayFilePath}`, err);
}

// Prompts
const workingDay = await tp.system.prompt("Is it a working day? (yes/no)");

let locationText = "";
let sprintNumber = "";
if (workingDay.toLowerCase() === "yes") {
    const location = await tp.system.prompt("Where are you working from? (home/office)");
    locationText = location.toLowerCase() === "home" ? "Home" : "Office";

    sprintNumber = await tp.system.prompt("Enter the Sprint Number:");
}

// Proceed to common questions for both working and non-working days
let weightKg = await tp.system.prompt("What is your weight in KG? (Press Enter to skip)");
let spaceGoodsDrink = await tp.system.prompt("Have you had a Space Goods drink today? (yes/no or press Enter to skip)");

// Handle optional inputs
weightKg = weightKg ? `${weightKg} KG` : "Not recorded";
spaceGoodsDrink = spaceGoodsDrink ? (spaceGoodsDrink.toLowerCase() === "yes" ? "Yes" : "Not recorded") : "Not recorded";

// Generate dynamic tags (only for working days with sprint number)
let tags = "";
if (workingDay.toLowerCase() === "yes" && sprintNumber) {
    tags = `#Sprint-${sprintNumber}`;
}

// Reading Activity Questions
let readingActivity = "";
const didReadYesterday = await tp.system.prompt("Did you do any reading yesterday? (yes/no)");
if (didReadYesterday.toLowerCase() === "yes") {
    // Fetch books from "Currently Reading"
    let currentlyReadingBooks = [];
    try {
        const currentlyReadingFile = app.vault.getAbstractFileByPath(currentlyReadingFilePath);
        if (!currentlyReadingFile) throw new Error(`File not found: ${currentlyReadingFilePath}`);
        const currentlyReadingContent = await app.vault.read(currentlyReadingFile);

        // Extract lines that look like books (e.g., numbered lines)
        currentlyReadingBooks = currentlyReadingContent
            .split("\n")
            .filter(line => line.match(/^\d+\s+-\s+/)) // Match lines like "1 - Book Title"
            .map(line => line.trim());
    } catch (err) {
        console.error(`Error reading Currently Reading file: ${currentlyReadingFilePath}`, err);
    }

    // Dropdown to select the book
    const selectedBook = await tp.system.suggester(currentlyReadingBooks, currentlyReadingBooks, false);

    // Ask if the book is finished
    const finishedBook = await tp.system.prompt(`Did you finish "${selectedBook}"? (yes/no or press Enter to skip)`);
    if (finishedBook.toLowerCase() === "yes") {
        // Move the book to "Completed Reading"
        try {
            let completedReadingFile = app.vault.getAbstractFileByPath(completedReadingFilePath);
            if (!completedReadingFile) {
                // Create the file if it doesn't exist
                await app.vault.create(completedReadingFilePath, `# Completed Reading\n\n`);
                completedReadingFile = app.vault.getAbstractFileByPath(completedReadingFilePath);
            }

            // Append the book to "Completed Reading"
            const completedReadingContent = await app.vault.read(completedReadingFile);
            await app.vault.modify(
                completedReadingFile,
                `${completedReadingContent}\n${selectedBook}`
            );
            console.log(`Book "${selectedBook}" moved to Completed Reading.`);
        } catch (err) {
            console.error(`Error handling Completed Reading file: ${completedReadingFilePath}`, err);
        }

        // Remove the book from "Currently Reading"
        try {
            const currentlyReadingFile = app.vault.getAbstractFileByPath(currentlyReadingFilePath);
            const currentlyReadingContent = await app.vault.read(currentlyReadingFile);
            const updatedCurrentlyReadingContent = currentlyReadingContent
                .split("\n")
                .filter(line => line.trim() !== selectedBook)
                .join("\n");
            await app.vault.modify(currentlyReadingFile, updatedCurrentlyReadingContent);
            console.log(`Book "${selectedBook}" removed from Currently Reading.`);
        } catch (err) {
            console.error(`Error updating Currently Reading file: ${currentlyReadingFilePath}`, err);
        }

        // Add to reading activity as finished
        readingActivity = `- Did you read yesterday? **yes**\n- Book: **${selectedBook}**\n- Action: **finished**`;
    } else {
        // Add to reading activity as in progress
        readingActivity = `- Did you read yesterday? **yes**\n- Book: **${selectedBook}**\n- Action: **still in progress**`;
    }
} else {
    readingActivity = `- Did you read yesterday? **no**`;
}

// Generate daily note output
tR += `# ${todayFileName}\n\n`;

if (yesterdayTasks.length > 0) {
    tR += `## What I Did Yesterday:\n`;
    yesterdayTasks.forEach(task => {
        tR += `- [ ] ${task.replace(/^-/, "").trim()}\n`;
    });
    tR += `\n`;
}

tR += `## What Will I Do Today:\n- ...\n\n`;
tR += `## Impediments:\n- ...\n\n`;
tR += `## How Am I Today?\n`;
tR += `- [ ] Sad\n`;
tR += `- [ ] Angry\n`;
tR += `- [ ] Nothing\n`;
tR += `- [ ] Happy\n`;
tR += `- [ ] Frustrated\n\n`;
tR += `## Interesting Things:\n- ...\n\n`;
tR += `## Things to Add to the Monthly Reflection:\n- ...\n\n`;
tR += `## Reflections:\n- ...\n\n`;
tR += `## Reading Activity:\n\n${readingActivity}\n\n`;
tR += `## Weight and Space Goods:\n`;
tR += `- Weight: **${weightKg}**\n`;
tR += `- Had a Space Goods Drink Today? **${spaceGoodsDrink}**\n\n`;
tR += `## Tags:\n\n**Tags:** ${tags || "None"}\n`;
%>
