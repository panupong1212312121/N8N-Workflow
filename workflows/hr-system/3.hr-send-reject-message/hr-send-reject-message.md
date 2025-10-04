### HR Send Reject Candidate

---

### Origin and Problem

This workflow was developed to streamline the often time-consuming and sensitive process of candidate rejection, ensuring timely and professional communication while maintaining human oversight. The challenges it addresses include:

1.  **Delayed Communication:** The manual process of notifying unsuccessful candidates often resulted in significant delays, leading to a poor candidate experience.

2.  **Required Human Review:** The need for HR personnel to **review and confirm** statuses (e.g., job role closure, candidate rejection status) before automatically dispatching final messages.

---

### Workflow Logic

This n8n workflow is designed to execute as a **Manual Trigger** only after HR personnel have finalized the recruitment status in the central sheets.

1.  **Manual Trigger Requirement:** The workflow requires manual execution by the user, ensuring that all pre-requisite reviews are completed by the HR team before messages are sent.

2.  **Pre-Flight Data Check:** The system first verifies the status columns in both the **Candidate Status Sheet** and the **Job Roles Sheet** to ensure they are marked as inactive, closed, or specifically tagged for rejection.

3.  **Filter for Rejection:** It filters the Candidate Status Sheet, identifying only those candidates who meet the criteria for rejection (e.g., `Status = 'Not Selected'`).

4.  **Automated Status Update (Cleanup):** For the identified rejected candidates, the workflow automatically updates their final status to `Inactive` or `Rejected` in the tracking sheet, signaling that the row is no longer actively processed.

5.  **Dynamic Email Generation & Dispatch:** Using a predefined template, the workflow retrieves the candidate's details (name, email, job role) and dynamically generates a personalized rejection email, which is then automatically dispatched.

---

### Benefits

Automating the rejection process under manual control provides critical advantages for both the HR team and the candidates:

* **Controlled Communication:** Ensures HR retains the final review step, preventing premature or erroneous communication, especially in sensitive rejection scenarios.

* **Process Efficiency:** Frees up recruiter time by eliminating the need to manually draft and send individual rejection emails while handling the necessary status clean-up automatically.

* **Improved Data Integrity:** The final automated status update (setting rows to `Inactive`) ensures the tracking sheet remains clean and accurate for future reporting.

---

### Workflow Diagram
![HR Send Reject Candidate Workflow Diagram](https://github.com/panupong1212312121/N8N-Workflow/blob/main/workflows/hr-system/3.hr-send-reject-message/asset/workflow.png)

---

### Sample Input/Configuration

This section illustrates the prerequisite steps required by the HR team before running the workflow.

#### 1. Candidate Status Sheet Preparation

The HR user manually sets the `Selection Status` for candidates who are not moving forward (e.g., setting the status to 'Not Selected').

![Candidate Status Sheet - Manual Status Update](https://github.com/panupong1212312121/N8N-Workflow/blob/main/workflows/hr-system/3.hr-send-reject-message/asset/input1.png)

#### 2. Job Roles Sheet Configuration

The HR user confirms that the status for the specific job role is closed (e.g., setting the `Status` to 'Inactive' or 'Hired'), signaling that the entire recruitment drive for that position is complete.

![Job Roles Sheet - Status Update](https://github.com/panupong1212312121/N8N-Workflow/blob/main/workflows/hr-system/3.hr-send-reject-message/asset/input2.png)

---

### Sample Output

#### 1. Updated Candidate Status (Automatic Cleanup)

The workflow automatically sets the status of the rejected candidate's row to `Inactive` or a definitive `Rejected` status in the master sheet, ensuring the data is correctly marked as complete and no longer active in the pipeline.

**Example Row Output:**
| Candidate Name | Selection Status (After Run) | Status |
| :--- | :--- | :--- |
| Candidate D | Not Selected | **Inactive** |

![Candidate Status Sheet - Inactive Status Update](https://github.com/panupong1212312121/N8N-Workflow/blob/main/workflows/hr-system/3.hr-send-reject-message/asset/result1.png)

#### 2. Rejection Email Sample

An example of the personalized, professionally formatted email automatically dispatched to the unsuccessful candidate.

![Rejection Email Sample](https://github.com/panupong1212312121/N8N-Workflow/blob/main/workflows/hr-system/3.hr-send-reject-message/asset/result2.png)

---

To download the workflow's JSON file, please visit the [**Link to JSON**](https://github.com/panupong1212312121/N8N-Workflow/tree/main/workflows/hr-system/3.hr-send-reject-message/hr-send-reject-message.json).