# 🔄 HR Automation Workflow (n8n)

This workflow automates the hiring process using n8n and AI.



## 🚀 Features

- 📄 Job application form
- 📂 Resume upload to Google Drive
- 📊 Store candidate data in Google Sheets
- 🧠 AI resume screening (JD vs CV match)
- ✅ Auto shortlisting
- ❌ Auto rejection emails
- 📧 Interview invitation emails

---

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/97a960b1-5fd2-4767-b650-f2616e1fdf04" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b6fd510b-2f72-490c-bd4f-4d4f6620bb8e" />

<img width="1919" height="916" alt="image" src="https://github.com/user-attachments/assets/500f059c-ea3b-4770-8e93-6b598e6a04eb" />

<img width="1526" height="764" alt="image" src="https://github.com/user-attachments/assets/9f3ffe54-29bd-4077-b892-93f41aeb448c" />


## 🧩 Workflow Steps

1. Form submission (candidate applies)
2. Resume uploaded to Google Drive
3. Candidate data saved in Google Sheets
4. Resume text extracted from PDF
5. AI compares resume with job description
6. Candidate scored (0–1)
7. Decision:
   - Score ≥ 0.7 → Shortlisted
   - Score < 0.7 → Rejected
8. Email sent automatically

---

## 📁 File

- `hr-automation.json` → Import into n8n

---

## ⚙️ Requirements

- n8n installed
- Google Drive API
- Google Sheets API
- Gmail API
- OpenAI / LLM API

---

## 📥 How to Import

1. Open n8n
2. Click "Import Workflow"
3. Upload `hr-automation.json`
4. Configure credentials
5. Activate workflow

---

## 🧠 AI Logic

The AI agent compares:
- Job Description
- Resume content

Returns:
```json
{
  "score": 0.85,
  "reason": "Good skill match but lacks experience"
}
