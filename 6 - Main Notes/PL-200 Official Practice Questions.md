

Tags: [[Power Bi]] [[Power Apps]] [[Power Apps]] [[Power Platform]] [[1 - Rough Notes/PL-200|PL-200]] [[PL-200 Official Practice Questions]]

### Question 1
You are developing a business process flow. You need to trigger a workflow on demand inside the business process flow to create a new account. Which component should you use?

- A. Stage  
- B. Condition  
- C. Data Step  
- D. Action Step

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** Action Step can be used to execute an action or workflow on demand. Each stage contains a group of steps. The exact step that can be used to trigger a workflow is the Action step.
</details>

---

### Question 2
You are capturing customer medical information in a model-driven app form. You must perform complex calculations with the app. You need to ensure that users cannot enter data while calculations are performed. Which tool should you use to lock the user interface?

- A. Power Fx  
- B. Instant workflow  
- C. Business process flow  
- D. Classic workflow

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** A classic workflow can be used as a real-time workflow, and the interface can be locked until the workflow has completed running.
</details>

---

### Question 3
You are troubleshooting a classic workflow developed for a customer. The workflow is failing to run and is set in a state of Waiting. You observe that the account of the workflow owner is deactivated. You need to resolve the issue. What should you do?

- A. Update the workflow owner and update the owner of the workflow runs  
- B. Update the workflow owner and cancel the previous runs in the Waiting state  
- C. Update the workflow owner and resubmit the previous workflow runs  
- D. Update the workflow owner and delete the previous workflow runs

<details>
<summary>Show Answer</summary>
**Correct Answer:** B  
**Explanation:** The workflow owner must be updated, and all previous runs in a state of Waiting must be canceled.
</details>

---

### Question 4
You are creating a dedicated Microsoft Power Platform solution for a customer. You must deploy the solution to the Power Platform production environment of the customer. You define the solution name. What should you define next?

- A. Required solution assets  
- B. Environment variables  
- C. Connection references  
- D. New publisher

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** The publisher data is used to identify components provisioned by the solution and search for them in the customer’s environment.
</details>

---

### Question 5
You are building a leave request canvas app. The app uses a Microsoft SharePoint Online list as a data source. The app must use a different data source in the development environment than in the production environment. You need to prepare a solution to export the app from the development environment and import it to the production environment. What should you use to manage the different data sources?

- A. Connection reference  
- B. Environment variable  
- C. Setting environment value  
- D. Action

<details>
<summary>Show Answer</summary>
**Correct Answer:** B  
**Explanation:** Environment variables allow you to define a connection to a specific site and list in SharePoint.
</details>

---

### Question 6
You manage solution deployment between Microsoft Dataverse environments. You import solutions from several customizers. You need to update the components that support merge behavior. Which component should you update?

- A. Model-driven app  
- B. Cloud flow  
- C. Dataverse table  
- D. Canvas app

<details>
<summary>Show Answer</summary>
**Correct Answer:** A  
**Explanation:** A model-driven app, form, and site map component update supports merge behavior.
</details>

---

### Question 7
You are creating a Microsoft Copilot Studio bot. You must isolate the bot environment from other Power Platform solutions. You need to create the environment for the bot to reside in. Where would you create the environment?

- A. Copilot Studio portal  
- B. Microsoft 365 Admin Center  
- C. Copilot Studio bot setup  
- D. Power Platform Admin Center

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** The Power Platform Admin Center is where environments are created, and bots can then be associated with the environment during the setup phase.
</details>

---

### Question 8
A company uses model-driven apps. The company integrates the Dataverse environment and Exchange Online. A new staff member is given an Exchange mailbox and is added to the Dataverse environment. The user is able to work with the model-driven apps but is unable to send emails from within Dataverse. You need to resolve the issue. What should you do?

- A. Add an email address to the user’s mailbox record  
- B. Add an email address to the user record in Dataverse  
- C. Create a mailbox record for the user in Dataverse  
- D. Test and enable the mailbox on the user’s mailbox record

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** Before a user can send emails from and receive emails in Dataverse, an administrator must test and enable the mailbox on the user’s mailbox record.
</details>

---

### Question 9
A company is configuring email integration between Exchange Online and Dataverse. The company requires email addresses to be approved for each mailbox in Dataverse. You need to recommend the security privileges the email approver must use. Which two roles should you recommend? (Select all that apply.)

- A. Global Administrator  
- B. System Administrator  
- C. System Customizer  
- D. User Administrator

<details>
<summary>Show Answer</summary>
**Correct Answers:** A, B  
**Explanation:** To approve email addresses in Dataverse, the Global Administrator role in the tenant and the System Administrator role in Dataverse are required.
</details>

---

### Question 10
Members of a marketing department use a model-driven app to view record documents that are stored in SharePoint. You need to ensure that only the marketing department members can edit the documents. From where should you assign additional permissions to the members?

- A. Dataverse  
- B. Model-driven app  
- C. Microsoft Entra ID  
- D. SharePoint

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** The permission level should be assigned in SharePoint to ensure that the marketing department members can edit the documents.
</details>

---

### Question 11
You create a custom table in Microsoft Dataverse to capture blood donor information. You create a canvas app in which users will record and save data to the Dataverse table. Users must capture whether a donor donated blood previously. If the donor has, you must fill out a Donor ID column value. You use a business rule to enforce this. You need to configure the column. What should you do?

- A. Set the business rule scope to Information  
- B. Set the business rule scope to All Forms  
- C. Set the business rule to display the Donor ID column when a user confirms that they have donated previously  
- D. Set the business rule scope to Entity  
- E. Set the business rule to display the Donor ID column as Business Recommended when a user confirms a previous donation

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** Setting the scope to Entity enforces this behavior within the canvas app as well as any model-driven apps.
</details>

---

### Question 12
You manage a model-driven app. Users often enter data incorrectly in a model-driven app form. You need to display business recommendations based on business intelligence to help the users. What should you use?

- A. Business process flow  
- B. Workflow  
- C. Cloud flow  
- D. Business rule

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** A business rule can be used to provide business recommendations based on business intelligence in a model-driven app form.
</details>

---

### Question 13
You create a model-driven app to assist with customer service. The customer service employees must follow a consistent process guide for entering data for customer service requests. You need to implement the requirement. Which tool should you use?

- A. Workflow  
- B. Business process flow  
- C. Business rule  
- D. Cloud flow

<details>
<summary>Show Answer</summary>
**Correct Answer:** B  
**Explanation:** Business process flows walk users through a standard business process to ensure consistency.
</details>

---

### Question 14
A company is using Microsoft Dynamics 365 Sales. Managers must receive an email when a salesperson creates a new opportunity that is greater than $5,000 United States Dollar (USD). You need to create a flow to send the email. Which type of flow should you create?

- A. Scheduled cloud flow with a Switch action  
- B. Scheduled cloud flow with an Apply to each action  
- C. Automated cloud flow with a Condition action  
- D. Automated cloud flow with a Switch action

<details>
<summary>Show Answer</summary>
**Correct Answer:** C  
**Explanation:** An automated cloud flow is triggered when an event occurs, such as a new record creation in Dataverse, and uses a Condition action to test the opportunity value.
</details>

---

### Question 15
You are building an approval cloud flow for a company to assign tasks. The company plans to allow five days for task assignments. If an assignee does not complete an assigned task within the five days, the task must be assigned to the assignee’s manager. You need to configure the cloud flow. Which three actions should you perform? (Select all that apply.)

- A. Set the Wait for an approval action timeout setting to P5D  
- B. Add a Delay action and set it to pause at 120 hours  
- C. Use a parallel branch action  
- D. Configure a Start an approval action to run after the previous action times out  
- E. Use a condition control to verify whether the task is completed within the expected time  
- F. Use a switch control to assign tasks based on roles

<details>
<summary>Show Answer</summary>
**Correct Answers:** A, C, D  
**Explanation:** The Wait for an approval action timeout, parallel branch, and run-after configuration allow for the reassignment logic after the task times out.
</details>

---

### Question 16
You create a business process flow for a wedding planning company to capture event information. The company has the following requirements when customers confirm that they reserved a venue:

- Initiate a prompt to capture venue contact information.  
- Send an email from the company Office 365 email account to the customer.  

You need to configure the flow. What should you do?

- A. Use a condition component to capture contact information, and an action step to send an email  
- B. Use a stage component to capture contact information, and a flow step to send an email  
- C. Use a data step to capture contact information, and a workflow step to send an email  
- D. Use a condition component to capture contact information, and a flow step to send an email

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** Condition components are used to show/hide steps based on a condition, and flow steps are used to trigger Power Automate flows for sending emails.
</details>

---
### Question 17
You are developing a classic workflow.

You need to check the following:

- Current values for the row that the real-time workflow is running on  
- The values of any rows linked to the real-time workflow row in an N:1 relationship

Which condition type should you use?

- A. Conditional branch  
- B. Parallel wait branch  
- C. Check condition  
- D. Wait condition

<details>
<summary>Show Answer</summary>
**Correct Answer:** C  
**Explanation:** The "Under" and "Not Under" hierarchical operators can be used in a check condition type to get rows linked with the parent row in an N:1 relationship.
</details>

---

### Question 18
You are authoring a cloud flow in Power Automate. You plan to use data from a choice column retrieved from a Dataverse table. Users can select from 10 values in the choice column. The flow must follow the branch of whichever value is selected in the choice column.

Which flow component should you use?

- A. Do Until  
- B. Scope  
- C. Switch

<details>
<summary>Show Answer</summary>
**Correct Answer:** C  
**Explanation:** The Switch component provides multiple branches depending on the value of an item, such as a Dataverse column.
</details>

---

### Question 19
You are configuring an automated process for the Contact table in a model-driven app.

The process must run when a contact record is updated. The update must be prevented if specific business logic conditions are not met.

Which type of process should you use?

- A. Cloud flow with the "When an action is performed" trigger  
- B. Cloud flow with the "When a row is added, modified or deleted" trigger  
- C. Real-time classic workflow  
- D. On-demand classic workflow

<details>
<summary>Show Answer</summary>
**Correct Answer:** C  
**Explanation:** Only real-time classic workflows can prevent an update to a record.
</details>

---

### Question 20
You configure an automated cloud flow by using the Dataverse connector. The flow triggers when a user modifies the email address of a contact. You plan to add an "Update a row" action to the flow.

You need to select the column that will identify the updated contact when the flow is triggered.

Which column should you select?

- A. Contact  
- B. Email  
- C. Full Name  
- D. Import Sequence Number

<details>
<summary>Show Answer</summary>
**Correct Answer:** A  
**Explanation:** The "Contact" column contains the GUID for the contact, which is used to identify the row.
</details>

---

### Question 21
A company has an automated flow that triggers when an item is created in a SharePoint list. The list has a column named "Status."

You need to configure the flow to run only when the item status equals "Approved."

What should you configure in the trigger?

- A. Split on  
- B. Custom Tracking Id  
- C. Trigger condition  
- D. Concurrency Control

<details>
<summary>Show Answer</summary>
**Correct Answer:** C  
**Explanation:** Adding a trigger condition ensures that the flow runs only when the condition is met.
</details>

---

### Question 22
A company configures a Research business unit in Dataverse. The business unit has users who own contacts in the Contacts table. You use the Dataverse trigger in a cloud flow to access the Contacts table.

You need to ensure that the flow triggers only if users in the Research business unit modify the contacts.

Which two actions should you perform? (Select all that apply.)

- A. Set the scope to User  
- B. Set the scope to Organization  
- C. Set the scope to Business unit  
- D. Set the Change type to Modified  
- E. Set the Change type to Added or Modified or Deleted

<details>
<summary>Show Answer</summary>
**Correct Answers:** C, D  
**Explanation:** Setting the scope to "Business unit" limits the flow to the Research business unit, and the "Change type" of "Modified" ensures it triggers only on updates.
</details>

---


### Question 23
You manage a Microsoft Dataverse instance for a company. The Dataverse instance has a one-to-many (1:N) relationship between a Teachers table and a Classes table.

If a teacher record is deleted, the deletion must have no impact on the related class records.

You need to configure the behavior of the tables.

Which relationship behavior should you use?

- A. Cascade all  
- B. Parental  
- C. **Referential, remove link**  
- D. Referential, restrict delete

<details>
<summary>Show Answer</summary>
**Correct Answer:** C  
**Explanation:** In a referential relationship between two tables, actions taken on one will not affect the other. "Remove link" ensures no cascading impact when a parent record is deleted.
</details>

---

### Question 24
A company plans to store project details in a Microsoft Dataverse table.

Users require a new table to store projects and related tasks.

Which option should you select to create the new table?

- A. Activity table  
- B. Enable attachments  
- C. Enable connections  
- D. **Enable for activities**

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** The "Enable for activities" option allows activities such as tasks and emails to be connected to the table.
</details>

---

### Question 25
You manage a Microsoft Dataverse instance.

Users must receive a warning message when they try to save a contact that matches an existing contact record. A match in one of the following columns must trigger the message:

- First and last name  
- Email address  
- Mobile phone number

You need to configure duplicate detection on the Contact table.

How many duplicate detection rules must you create?

- A. One  
- B. Two  
- C. **Three**  
- D. Four

<details>
<summary>Show Answer</summary>
**Correct Answer:** C  
**Explanation:** Separate rules are needed for each column condition: one for first and last name, one for email address, and one for mobile phone number.
</details>

---

### Question 26
A company stores customer data in a Microsoft SharePoint list. The SharePoint list does not use data validation.

The company plans to deploy a model-driven app within Microsoft Dataverse to manage the customer data.

You need to reduce the risk of errors when bringing the data into Dataverse by using standard functionality as much as possible.

Which tool should you use?

- A. Microsoft Power Automate  
- B. Data map  
- C. **Template for data import**  
- D. Dataflow

<details>
<summary>Show Answer</summary>
**Correct Answer:** C  
**Explanation:** A template for data import ensures data is pre-validated, reducing errors during the import process.
</details>

---

### Question 27
You are creating a cloud flow to perform bulk operations on data in Microsoft Dataverse. You verify that the configuration in Microsoft Power Platform admin center is set up correctly.

Cloud flow searches two columns in a table by using the Search rows action. Dataverse search does not return any results.

What should you do?

- A. In the Power Platform admin center, turn on Dataverse search for your environment  
- B. Add table to the search index  
- C. Add a column to the quick find view  
- D. **Reset filter conditions for the column**

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** Resetting filter conditions ensures that preset filters in the quick find view do not block the column from being searched.
</details>

---

### Question 28
A company is using Microsoft Dataverse search.

You need to configure Quick Find View so the Relationship column appears in the filter pane when users search for accounts.

Which part of Quick Find View should you configure?

- A. Filter by  
- B. Sort by  
- C. Find columns  
- D. **View columns**

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** "View columns" appear in the filter pane of the search results.
</details>

---

### Question 29
A company uses Microsoft Power Platform in its Microsoft 365 tenant.

The company requires specific users to manage environments within the tenant.

You need to configure security for the tenant.

What should you use?

- A. **Microsoft 365 role**  
- B. Microsoft Dataverse security role  
- C. Access team  
- D. Microsoft Power Platform license

<details>
<summary>Show Answer</summary>
**Correct Answer:** A  
**Explanation:** Assigning the "Power Platform administrator" role in Microsoft 365 allows users to manage environments.
</details>

---

### Question 30
A company that delivers training courses uses Microsoft Dataverse.

The company wants to record course registration and attendance. The company configures a Contact table and a Course table.

You need to create a relationship between the attendees and registrations.

Which type of relationship should you create?

- A. One 1:N relationship with Contact as the parent  
- B. One 1:N relationship with Course as the parent  
- C. One N:N relationship between Contact and Course  
- D. **Two 1:N relationships, one with Contact as the parent and one with Course as the parent**

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** Two 1:N relationships allow for storing additional information like attendance status in a third table.
</details>

---

### Question 31
A company uses Microsoft Dataverse.

You must prevent users from creating contacts with the same first and last names as existing leads.

You need to configure the system.

What should you configure?

- A. Duplicate detection job  
- B. **Duplicate detection rule**  
- C. Alternate key on the lead table  
- D. Alternate key on the contact table

<details>
<summary>Show Answer</summary>
**Correct Answer:** B  
**Explanation:** A duplicate detection rule can be configured to prevent duplicates between two tables. The rule specifies which fields on the two tables must match for a record to be considered a duplicate.
</details>

---

### Question 32
You use Microsoft Entra ID Group teams to handle user security access to a Microsoft Dataverse application.

You need to set up security group teams within Dataverse and apply security roles to them.

What should you use to set up the team record in Dataverse?

- A. Microsoft Entra ID Group Team name  
- B. Security Role name  
- C. **Microsoft Entra ID Group ID**  
- D. Dataverse Business Unit

<details>
<summary>Show Answer</summary>
**Correct Answer:** C  
**Explanation:** To set up a team record in Dataverse that is linked to a Microsoft Entra ID Group team, you must use the Microsoft Entra ID Group ID.
</details>

---

### Question 33
You are migrating data from various data sources into a Microsoft Dataverse solution data structure.

You need to ensure that duplicate records are removed when you import to Dataverse.

What should you use?

- A. Power Automate  
- B. Data Import Wizard  
- C. **Dataflows**  
- D. Microsoft Excel Online connected to the Dataverse table

<details>
<summary>Show Answer</summary>
**Correct Answer:** C  
**Explanation:** Dataflows can connect to multiple data sources to ingest data, transform, cleanse it, and check for duplicates before pushing the data to Dataverse.
</details>

---

### Question 34
You create a custom table named Books.

Users are not able to add notes to book records on the timeline.

You need to resolve the issue.

What should you do?

- A. Add a file column to the Books table  
- B. Add a multiple lines of text column to the Books table  
- C. **Select the Enable attachments property on the Books table**  
- D. Select the Creating a new activity property on the Books table

<details>
<summary>Show Answer</summary>
**Correct Answer:** C  
**Explanation:** The Enable attachments property on a table enables notes to be added to records. A note can optionally include an attachment.
</details>

---

### Question 35
A company uses Dataverse to store projects and project outcomes in two custom tables.

Users must be able to edit columns in the custom tables.

You need to assign a security role to the users by using the principle of least privilege.

Which security role should you assign?

- A. Environment Maker  
- B. System Administrator  
- C. **System Customizer**  
- D. Basic User

<details>
<summary>Show Answer</summary>
**Correct Answer:** C  
**Explanation:** The System Customizer role allows users to edit columns in custom tables without granting unnecessary permissions.
</details>

---

### Question 36
A company uses a Dataverse table named Milestones to store project milestone information.

You need to ensure that only users in the Project Managers team can view data in the Milestone status column.

Which three configuration steps should you perform? (Select all that apply.)

- A. Create a new security role  
- B. **Create a new column security profile**  
- C. **Enable column security on the Milestone status column**  
- D. Apply a security role to the Project Managers team  
- E. Assign read privilege on the Milestones table to the security role  
- F. **Assign permissions and add the Project Managers team to the column security profile**

<details>
<summary>Show Answer</summary>
**Correct Answers:** B, C, F  
**Explanation:** Column security should be enabled for the Milestone status column, and permissions must be assigned to a column security profile.
</details>

---

### Question 37
A company is using a model-driven app.

When users view contacts for an account by navigating to the Related tab, they do not see the Job Title column in the default view.

You need to configure the view to include the Job Title column.

Which view should you configure?

- A. Advanced Find  
- B. Quick Find  
- C. **Associated**  
- D. Default public

<details>
<summary>Show Answer</summary>
**Correct Answer:** C  
**Explanation:** The Associated view is the default view shown when viewing contacts on the Related tab.
</details>

---

### Question 38
You create a canvas app to collect information for emergency medical technicians.

You must perform a calculation on the blood pressure screen to display a score result to the user. You must use a variable for only the blood pressure screen.

You need to set the variable.

Which function should you use?

- A. Collect  
- B. Set  
- C. ClearCollect  
- D. **UpdateContext**

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** The UpdateContext function is used to set a local variable, which is specific to a single screen.
</details>

---

### Question 39
You are building a canvas app for reporting accidents by on-site construction workers.

Employees report experiencing intermittent internet connectivity. The employees must have access to up-to-date information for their work.

You need to provide the employees with offline access to the latest data received when devices are online.

What should you do?

- A. Use a Microsoft Excel file as a data source  
- B. **Store the data locally by using SaveData and a collection**  
- C. Store the data locally by using LoadData and a collection  
- D. Get the data by using a Microsoft Power Automate cloud flow

<details>
<summary>Show Answer</summary>
**Correct Answer:** B  
**Explanation:** The SaveData formula saves data from a collection locally on a device, ensuring offline access to up-to-date data.
</details>

---

### Question 40
You are developing a canvas app named app1. The app has two screens, BrowseScreen1 and EditScreen1.

BrowseScreen1 includes a vertical gallery named gallery1. EditScreen1 includes an Edit form named form1.

You need to ensure that an item selected in gallery1 is populated in form1.

What should you configure?

- A. Set the DefaultMode property of form1 to gallery1.selected  
- B. Set the DataSource property of form1 to gallery1.selected  
- C. **Set the Item property of form1 to gallery1.selected**  
- D. Set the OnSuccess property of form1 to gallery1.selected

<details>
<summary>Show Answer</summary>
**Correct Answer:** C  
**Explanation:** To ensure that the selected item in gallery1 is populated in form1, you should set the Item property of form1 to gallery1.selected.
</details>

---

### Question 41
You create a canvas app within a solution.

You require a Microsoft Power Automate flow that is triggered from within the canvas app.

You need to create the Power Automate flow.

Which flow type should you create?

- A. Instant cloud flow under My flows in the Power Automate portal designer  
- B. Automated cloud flow inside the solution  
- C. **Instant cloud flow inside the solution**  
- D. Desktop flow inside the solution

<details>
<summary>Show Answer</summary>
**Correct Answer:** C  
**Explanation:** Canvas apps can use existing instant cloud flows that exist within the solution.
</details>

---

### Question 42
A supermarket requires a solution that recognizes products on shelves.

The solution must be able to take pictures of products on shelves. The solution must then automatically identify the products.

You need to create the solution.

What should you use?

- A. Power Pages  
- B. **Canvas app**  
- C. Model-driven app  
- D. Microsoft Dataverse for Teams

<details>
<summary>Show Answer</summary>
**Correct Answer:** B  
**Explanation:** Canvas apps can use the device camera to capture an image, and then use AI Builder Object Detection to process the image.
</details>

---

### Question 43
You need to build a canvas app that captures people’s names at a trade show.

Internet connectivity is unreliable. The app must store the names until a reliable connection can be made.

Which object should you use to store the data?

- A. **Collection**  
- B. Data table  
- C. Gallery  
- D. Variable

<details>
<summary>Show Answer</summary>
**Correct Answer:** A  
**Explanation:** In Power Apps, a collection is used to store multiple rows of data such as people’s names until the data is saved to a data location.
</details>

---

### Question 44
You need to use Microsoft Power Fx to create formulas in a canvas app.

Which type of low-code language enables this?

- A. Compiled  
- B. **Declarative**  
- C. Assembly  
- D. Interpreted

<details>
<summary>Show Answer</summary>
**Correct Answer:** B  
**Explanation:** Power Fx is a declarative language where the maker defines behavior, and the system optimizes how to achieve it.
</details>

---

### Question 45
You are creating a canvas app. You are using the Accounts table in the app.

You need to set the action to navigate to the default view of the Accounts table.

Which syntax should you use?

- A. **Navigate (Accounts)**  
- B. Navigate (‘Accounts (Views)’ . ’Active Accounts’)  
- C. Navigate (Account.Selected)  
- D. Navigate ( Defaults (Accounts))

<details>
<summary>Show Answer</summary>
**Correct Answer:** A  
**Explanation:** To navigate to a default view of a table, use the Navigate command and pass in just the table name as the argument.
</details>

---

### Question 46
You create a model-driven app.

You need to configure the columns that are searched when users use global search.

Which table view should you configure?

- A. Default public view  
- B. **Quick Find view**  
- C. Lookup view  
- D. Advanced Find view

<details>
<summary>Show Answer</summary>
**Correct Answer:** B  
**Explanation:** The Quick Find view is used to configure the columns that are searched during global search.
</details>

---

### Question 47
You develop a custom page by using Power Fx in a model-driven app.

You add a ContactsGallery1 gallery control to the custom page.

You need to navigate to the Contacts table default main form to edit a selected item in ContactsGallery1.

Which two Power Fx formulas can you use? (Select all that apply.)

- A. Navigate(Contacts)  
- B. Navigate(Defaults(Contacts))  
- C. **Navigate(ContactsGallery1.Selected)**  
- D. Navigate('Contacts (Views)'.'Active Contacts')  
- E. **Navigate(ContactsGallery1.Selected,{Page: 'Contacts (Forms)'.Contact })**

<details>
<summary>Show Answer</summary>
**Correct Answers:** C, E  
**Explanation:** The custom page in the model-driven app allows navigation to the Dataverse table forms and views using Power Fx.
</details>

---

### Question 48
A company uses a model-driven app.

Employees in the company access a list of accounts through the model-driven app.

You need to customize the account views for the employees’ mobile devices.

Which form should you customize?

- A. **Card**  
- B. Main  
- C. Quick Create  
- D. Quick View

<details>
<summary>Show Answer</summary>
**Correct Answer:** A  
**Explanation:** The Card form is used to display a list of accounts in model-driven apps on mobile devices.
</details>

---

### Question 49
A company uses a Power Pages site for customers to create and view their cases.

You configure the site to display a list of cases when a customer is logged in.

A new customer reports that they cannot display the cases. Other customers can display cases.

You need to troubleshoot the display issue.

What should you check?

- A. **Web roles**  
- B. Security roles  
- C. Table permissions  
- D. Permissions in Page settings

<details>
<summary>Show Answer</summary>
**Correct Answer:** A  
**Explanation:** Users of a Power Pages site derive privileges from being assigned to web roles, which govern access to site features.
</details>

---
### Question 50
A company added a custom column to a table in a production instance of Microsoft Dataverse by importing a managed solution from a development instance.

The column must be removed.

You delete the column in an unmanaged solution in the development instance.

What should you do next?

- A. Export an unmanaged solution  
- B. Create a patch solution  
- C. **Export a managed solution**  
- D. Modify the managed properties of the Account table

<details>
<summary>Show Answer</summary>
**Correct Answer:** C  
**Explanation:** A managed solution can be used to delete a column. An unmanaged solution and a patch solution cannot be used to delete a column. The managed properties of a component cannot be configured to allow a column to be deleted.
</details>

---

### Question 51
You create a Microsoft Power Platform solution in a development environment. The solution includes connection references and environment variables. Cloud flows use the values from the environment variables.

You export the solution as a managed solution. You import the managed solution to a production environment. You observe that the cloud flows use the values of the environment variables from the development environment.

You need to resolve the issue.

What should you do?

- A. **Remove the values from environment variables in the solution and then export the solution**  
- B. Set the default values of the environment variables before export  
- C. Delete the values from environment variables in the development environment and then export the solution  
- D. Create new environment variables in the solution after you import the solution into the production environment

<details>
<summary>Show Answer</summary>
**Correct Answer:** A  
**Explanation:** To set values of environment variables after import, remove the current values from the solution before export.
</details>

---

### Question 52
You manage solution deployment between Microsoft Dataverse environments.

You need to control which managed solution components are customizable after a solution is imported into a destination environment.

What should you use?

- A. Stage for upgrade  
- B. Solution segmentation  
- C. Configuration page  
- D. **Managed properties**

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** Managed properties control which managed solution components can be customized.
</details>

---

### Question 53
You are configuring integration between Exchange Online and Dataverse.

You need to enable the Dynamics 365 App for Outlook for users.

What should you do?

- A. Enable tracking tokens  
- B. Install an SSL certificate  
- C. Configure a forward mailbox  
- D. **Configure server-side synchronization**

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** Synchronization of email using server-side synchronization is a prerequisite for using the Dynamics 365 App for Outlook.
</details>

---

### Question 54
You are creating a Word template for a custom table named Customers. Each record in the table will store a customer logo.

You need to display the customer logo in the Word template.

Which two actions should you perform? (Select all that apply.)

- A. **Create a new image type column in the table**  
- B. Create a new file type column in the table  
- C. Create a new placeholder in the template  
- D. **Add the new image column to the Word template**  
- E. Add the new file column to the Word template

<details>
<summary>Show Answer</summary>
**Correct Answers:** A, D  
**Explanation:** To display an image in the Word template, create a new image field and add it to the template.
</details>

---

### Question 55
You are configuring a model-driven app by using business rules.

You need to ensure that the business rules run on the server side.

What should you use to configure the scope of the business rules?

- A. **Entity**  
- B. All forms  
- C. Information form  
- D. Account form

<details>
<summary>Show Answer</summary>
**Correct Answer:** A  
**Explanation:** Business rules run on the server side when the scope is configured as "Entity."
</details>

---

### Question 56
You create a custom table in Microsoft Dataverse to capture blood donor information. You create a canvas app in which users will record and save data to the Dataverse table.

Users must capture whether a donor donated blood previously. If the donor has, you must fill out a Donor ID column value. You use a business rule to enforce this.

You need to configure the column.

What should you do?

- A. Set the business rule scope to Information  
- B. Set the business rule scope to All Forms  
- C. Set the business rule to display the Donor ID column when a user confirms that they have donated previously  
- D. **Set the business rule scope to Entity**  
- E. Set the business rule to display the Donor ID column as Business Recommended when a user confirms a previous donation

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** Setting the scope to "Entity" enforces this behavior across all apps, including canvas and model-driven apps.
</details>

---