---
title: My First Blog Post
date: 2025-01-02
tags:
  - blog
  - personal
  - "#Obsidian"
  - "#GitHub"
---
# How I Set Up My Blog from Obsidian Using GitHub Pages

Hello everyone! 🎉

I’ve just set up my personal blog directly from my Obsidian vault using GitHub Pages, and now you can too! This guide walks you through every step of the process. Whether you’re looking for a simple setup or want to use your own custom domain, this guide has you covered.

---

## **Step 1: Prepare Your GitHub Repository**

1. Go to [GitHub](https://github.com/) and log in.
2. Create a new repository for your blog. Name it something like `MyWebPage`.
3. Set the repository to public and **DO NOT** initialize it with a README, `.gitignore`, or license (we’ll handle these later).

---

## **Step 2: Prepare Your Blog Folder in Obsidian**

1. In your Obsidian vault, create a new folder to hold your blog content. You can name this folder `blog` or any other name you prefer.
2. Inside this folder, add a markdown file for your first blog post. For example:
   - File name: `My First Blog Post.md`
   - Content:
     ```markdown
     ---
     title: "My First Blog Post"
     date: 2025-01-02
     tags: [blog, personal]
     ---
     
     # My First Blog Post
     
     This is the content of my very first blog post! It’s exciting to start this journey.
     ```

---

## **Step 3: Create the `index.html` File**

1. Inside your `blog` folder, create a new file named `index.html`.
2. Add the following content to this file:
   html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>My Blog</title>
   </head>
   <body>
       <h1>Welcome to My Blog</h1>
       <ul>
           <li><a href="My%20First%20Blog%20Post.md">My First Blog Post</a></li>
       </ul>
   </body>
   </html>

---

# Step 4: Create a `.gitignore` File

1. In the root of your Obsidian vault, create a new file named `.gitignore`.
2. Add the following content to the file: .obsidian/ *.log !blog/
3. This will exclude Obsidian’s configuration files and logs from being uploaded to GitHub, while ensuring the `blog` folder is included.

# Step 5: Initialize the Git Repository

1. Open your terminal (Git Bash or Command Prompt) and navigate to your Obsidian vault folder:
   cd "path/to/your/vault"
2. Initialize a Git repository
   git init
3. Add the blog folder and `.gitignore` file:
   git add blog/
   git add .gitignore
4. Commit your changes:
   git commit -m "Initial commit for blog"

---

# Step 6: Link the Repository to GitHub

1. Link your local repository to the GitHub repository you created earlier:
   git remote add origin https://github.com/YOUR-USERNAME/MyWebPage.git
2. Push your changes to GitHub:
   git push -u origin main


---

# Step 7: Enable GitHub Pages

1. On GitHub, navigate to your repository and go to **Settings**.
2. Scroll down to the **GitHub Pages** section.
3. In the **Source** dropdown, select `main` as the branch and `/ (root)` as the folder.
4. Save your changes. Your blog will be live at `https://YOUR-USERNAME.github.io/MyWebPage`.
# Step 8: (Optional) Set Up a Custom Domain

1. In the **GitHub Pages** section of your repository’s settings, enter your domain name in the **Custom domain** field (e.g., `www.example.com`).
2. Add a `CNAME` file to the root of your repository:
   echo "www.example.com" > CNAME
   git add CNAME
   git commit -m "Add CNAME for custom domain"
   git push origin main
3. Update the DNS settings of your domain to point to GitHub Pages. Add the following CNAME record:
	- Host: `www`
	- Points to: `YOUR-USERNAME.github.io`

# Congratulations! 
 Your blog is now live and ready to go.
 
 You can add new blog posts by creating markdown files in your blog folder and linking them in the `index.html` file.
 
 If you set up a custom domain, your blog will be accessible at your domain name. Happy blogging! 



