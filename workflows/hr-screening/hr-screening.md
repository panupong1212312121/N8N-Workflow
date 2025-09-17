### HR Screening (1st Draft)

---

### Origin and Problem

This workflow was created to address the significant challenges of manual resume screening. The original problems included:

1.  **Time-consuming Process:** A large volume of daily applications led to a slow and inefficient initial screening process, delaying the identification of suitable candidates.
2.  **Human Error:** The manual handling of applicant data increased the risk of mistakes, such as sending emails or making calls to the wrong contact information.

---

### Workflow Logic

This n8n workflow automates the initial screening of resumes by following a clear, step-by-step logic:

1.  **Data Extraction:** It pulls applicant information from a specified input form.
2.  **Data Organization:** The extracted data is automatically organized and saved to designated locations, such as individual folders for each applicant and a specific Google Sheet.
3.  **Candidate Analysis:** The workflow analyzes the applicant's data based on predefined criteria, including desired qualifications and a scoring rubric. It then assigns a score and provides a reasoned explanation for the evaluation, streamlining the selection process.

---

### Benefits

This workflow provides several key advantages:

* **Increased Efficiency:** It drastically reduces the time spent on manual screening, allowing for faster recruitment cycles.
* **Improved Accuracy:** Automation minimizes human error in handling data, ensuring that all information is correctly stored and processed.
* **Objective Evaluation:** The automated scoring system provides a consistent and unbiased assessment of candidates, improving the quality of the initial screening.

---

### Workflow Diagram
![HR Screening Workflow](https://github.com/panupong1212312121/N8N-Workflow/blob/main/workflows/hr-screening/asset/workflow.png)

---

### Sample Output

**Candidate Folder Structure**

This shows how the workflow automatically creates a dedicated folder for each candidate.

![Specific of each Candidate folder](https://github.com/panupong1212312121/N8N-Workflow/blob/main/workflows/hr-screening/asset/result1.png)

**Candidate's Resume**

Inside each candidate's folder, their resume and other documents are stored.

![Candidate's Resume](https://github.com/panupong1212312121/N8N-Workflow/blob/main/workflows/hr-screening/asset/result2.png)

**Candidate Evaluation Sheet**

A Google Sheet that stores all applicant data, complete with an automated score and reasoning.

![Candidate Evaluation Sheet](https://github.com/panupong1212312121/N8N-Workflow/blob/main/workflows/hr-screening/asset/result3.png)

---

To download the workflow's JSON file, please visit the [**Link To JSON**](https://github.com/panupong1212312121/N8N-Workflow/tree/main/workflows/hr-screening/hr-screening.json).