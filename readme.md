# n8n Workflow Collection

This repository serves as a collection of n8n workflows I've created. Each workflow is designed to automate a specific task or process, and is documented to help you understand its purpose and logic.

### 1. How to Use n8n

If you don't have n8n set up yet, you can use Docker to run it locally.
[วิธีติดตั้ง n8n + Docker ที่สามารถอัพเดตเวอร์ชั่นได้โดยที่ไฟล์ข้อมูลไม่สูญหาย | QWERTY N8N EP.09.](https://www.youtube.com/watch?v=UhtT86foTrU)

### 2. Repository Purpose

The primary goal of this repository is to store and document various n8n workflows. Each workflow is a `.json` file that you can easily import into your own n8n instance.

### 3. Workflow Index

| **System Name** | **Sub-System / Workflow Name** | **Description** | **Link to Details** |
| :---: | :--- | :--- | :--- |
| **HR Automation** [System Overview](https://github.com/panupong1212312121/N8N-Workflow/tree/main/workflows/hr-system/hr-system.md) | HR Screening | Automates the initial screening and evaluation of resumes submitted through an input form, providing an assessment score and analysis. | [View Details](https://github.com/panupong1212312121/N8N-Workflow/tree/main/workflows/hr-system/1.hr-screening/hr-screening.md) |
| | HR Candidate Status | Acts as a centralized tracking sheet to display essential candidate data and monitor recruitment status through various stages, such as Screening Pass, Assessment Scheduled, Interview Complete, Hired, Application Withdrawn, or Not Selected (Interview). | [View Details](https://github.com/panupong1212312121/N8N-Workflow/tree/main/workflows/hr-system/2.hr-candidate-status/hr-candidate-status.md) |
| | HR Send Reject Message | Automatically generates and dispatches personalized rejection notifications to candidates who did not pass the selection process for specific job roles. | [View Details](https://github.com/panupong1212312121/N8N-Workflow/tree/main/workflows/hr-system/3.hr-send-reject-message/hr-send-reject-message.md) |

Feel free to explore the folders to find the workflow you need!

### 📝 Memo
Workflows cannot be used directly in n8n. You must first configure the necessary settings, such as credentials and API keys for services like Google Drive, Google Sheets, Open Router, OpenAI, Gemini etc.