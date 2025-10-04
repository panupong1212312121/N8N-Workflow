### HR Candidate Status

---

### Origin and Problem

This workflow was developed to resolve the disorganization and lack of visibility often encountered during the talent acquisition process. The previous challenges included:

1.  **Fragmented Data:** Candidate information and progress were scattered across multiple spreadsheets and communication platforms, leading to difficult tracking and reporting.

2.  **Inconsistent Status Updates:** Manually updating recruitment status was prone to error and delay, making it hard for stakeholders to know the exact stage of each candidate.

---

### Workflow Logic

This n8n workflow establishes a centralized system for monitoring and managing the recruitment pipeline:

1.  **Central Data Synchronization:** The system periodically pulls essential candidate data (e.g., name, contact, job role) from initial screening outputs.

2.  **Master Sheet Management & Status Tracking:** The workflow maintains a **master tracking sheet** that displays all key candidate metrics. This sheet is the core mechanism for monitoring the recruitment pipeline, designed to facilitate manual updates to the candidate's selection status, supporting granular stages such as *Screening Pass, Assessment Scheduled, Interview Complete, Hired, Application Withdrawn*, or *Not Selected*.

---

### Benefits

Implementing this centralized tracking workflow offers distinct advantages:

* **Single Source of Truth:** Creates one reliable, easily accessible location for all critical candidate information, significantly improving data integrity and reducing lookup time.

* **Enhanced Pipeline Visibility:** Provides immediate and clear oversight of the entire recruitment pipeline, enabling recruiters and managers to identify and resolve bottlenecks quickly.

* **Improved Decision Making:** Consistent and near real-time status tracking supports timely actions, helping to accelerate the hiring process.

---

### Workflow Diagram
![HR Candidate Status Workflow Diagram](https://github.com/panupong1212312121/N8N-Workflow/blob/main/workflows/hr-system/2.hr-candidate-status/asset/workflow.png)

---

### Sample Output

#### Central Tracking Sheet (Master Data)

This shows the main Google Sheet serving as the core of the system, displaying crucial data fields and the current selection status column.

![Central Tracking Sheet Example](https://github.com/panupong1212312121/N8N-Workflow/blob/main/workflows/hr-system/2.hr-candidate-status/asset/result1.png)

---

To download the workflow's JSON file, please visit the [**Link to JSON**](https://github.com/panupong1212312121/N8N-Workflow/tree/main/workflows/hr-system/2.hr-candidate-status/hr-candidate-status.json).