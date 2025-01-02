
# [[PL-200 Exam Practice Questions]]

## Section 1: Configure Microsoft Dataverse (25–30%)

### Question 1
You are setting up a Microsoft Dataverse environment. You need to ensure that a specific user can create, update, and delete records in the "Accounts" table but cannot share records. Which security role configuration should you apply?
- A. User-level create, update, and delete permissions with no share permissions
- B. Team-level create, update, delete, and share permissions
- C. Organization-level create, update, and delete permissions
- D. Environment Admin role

<details>
<summary>Show Answer</summary>
**Correct Answer:** A  
**Explanation:** User-level permissions allow create, update, and delete access without the ability to share records.
</details>

---

### Question 2
You need to configure a one-to-many (1:N) relationship in Dataverse between the "Accounts" table and the "Contacts" table. What should you configure as the primary lookup field?
- A. Account Name
- B. Account ID
- C. Contact Email
- D. Contact ID

<details>
<summary>Show Answer</summary>
**Correct Answer:** B  
**Explanation:** The primary lookup field in a 1:N relationship is typically the unique identifier, such as Account ID.
</details>

---

### Question 3
A company uses a custom Dataverse table to store information about projects. You need to ensure that a specific column only allows values from a predefined list. What should you configure?
- A. Choice Column
- B. Lookup Column
- C. Text Column with Validation
- D. Business Rule

<details>
<summary>Show Answer</summary>
**Correct Answer:** A  
**Explanation:** A choice column restricts input to a predefined list of values.
</details>

---

### Question 4
You need to ensure that all changes to a "Customers" table in Dataverse are recorded for auditing purposes. What should you configure?
- A. Enable table-level auditing
- B. Enable field-level security
- C. Create a business rule
- D. Configure a Power Automate flow

<details>
<summary>Show Answer</summary>
**Correct Answer:** A  
**Explanation:** Table-level auditing captures all changes made to records in the table.
</details>

---

## Section 2: Create Apps by Using Microsoft Power Apps (25–30%)

### Question 1
You need to create a Power Apps canvas app that uses multiple screens and allows users to navigate between them. Which control should you use?
- A. Button
- B. Gallery
- C. Screen
- D. Navigate

<details>
<summary>Show Answer</summary>
**Correct Answer:** D  
**Explanation:** The Navigate function allows transitioning between screens in a canvas app.
</details>

---

### Question 2
You are building a model-driven app for a sales team. The app must display opportunities grouped by their status and allow inline editing of certain fields. What feature should you configure?
- A. Sub-grid
- B. Editable grid
- C. Quick View Form
- D. Lookup Field

<details>
<summary>Show Answer</summary>
**Correct Answer:** B  
**Explanation:** Editable grids allow inline editing and grouping of records based on a specific column.
</details>

---

## Section 3: Create and Manage Logic and Process Automation (25–30%)

### Question 1
You need to create a flow that triggers when a file is uploaded to a SharePoint document library. The flow must send an email notification to a specified recipient. What type of flow should you use?
- A. Scheduled Flow
- B. Automated Cloud Flow
- C. Instant Flow
- D. Business Process Flow

<details>
<summary>Show Answer</summary>
**Correct Answer:** B  
**Explanation:** Automated Cloud Flows are triggered automatically by an event, such as a file upload.
</details>

---

### Question 2
You need to automate an approval process for expense reports. The flow must allow the manager to approve or reject the request. Which action should you include in the flow?
- A. Condition
- B. Create Approval
- C. Email Notification
- D. Apply to Each

<details>
<summary>Show Answer</summary>
**Correct Answer:** B  
**Explanation:** The "Create Approval" action starts the approval process and allows for responses.
</details>

---

## Section 4: Manage Environments (15–20%)

### Question 1
You need to create a new environment in the Power Platform admin center to support a development project. What type of environment should you create?
- A. Production
- B. Sandbox
- C. Trial
- D. Default

<details>
<summary>Show Answer</summary>
**Correct Answer:** B  
**Explanation:** Sandbox environments are used for development and testing without affecting production data.
</details>

---

### Question 2
A company wants to enforce specific data loss prevention policies across all environments. What tool should you use?
- A. Power Platform Admin Center
- B. Azure AD
- C. Environment Variables
- D. Data Gateway

<details>
<summary>Show Answer</summary>
**Correct Answer:** A  
**Explanation:** The Power Platform Admin Center allows you to configure data loss prevention policies at an environment level.
</details>

---

Let me know if further adjustments are needed or if additional content should be added!
```