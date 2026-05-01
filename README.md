# 🤖 AI-Powered Student Evaluation Bot  
### (UiPath + OCR + LLM Integration)

An end-to-end automation system that evaluates student answer sheets using **OCR + Large Language Models (LLMs)** and generates structured results in Excel.

---

# 🚀 Project Overview

Manual evaluation of student answer sheets is:
- Time-consuming ⏳  
- Inconsistent ❌  
- Hard to scale 📉  

This project solves that by combining **RPA (UiPath)** with **AI (LLMs)** to create a fully automated evaluation pipeline.

---

# 🎯 Key Features

✅ Extracts text from PDFs (question paper, marking scheme, student answers)  
✅ Uses AI to evaluate responses  
✅ Generates:
- Score  
- Feedback  
- Suggestions  

✅ Handles multiple students automatically  
✅ Outputs structured results into Excel  
✅ Designed to handle inconsistent AI responses  

---
# 🧱 Architecture

📂 Input PDFs
↓
🔍 OCR Extraction
↓
🧹 Text Cleaning
↓
🧠 Prompt Engineering
↓
🤖 LLM API (Groq / Gemini)
↓
🧩 Response Parsing
↓
📊 Data Structuring
↓
📁 Excel Output


---

# 📂 Directory Structure
StudentEvaluationBot/
│
├── Main.xaml # Main UiPath workflow
├── project.json # Project configuration
│
├── InputFiles/
│ ├── QuestionPaper.pdf
│ ├── MarkingScheme.pdf
│ └── Students/
│ ├── student1.pdf
│ ├── student2.pdf
│ └── ...
│
├── Output/
│ └── EvaluationResults.xlsx
│
├── Assets/ # (Optional) Screenshots / diagrams
│ ├── architecture.png
│ ├── workflow.png
│ └── output.png
│
└── README.md


---

# ⚙️ Tech Stack

| Component | Technology |
|----------|----------|
| Automation | UiPath Studio |
| OCR | UiPath OCR / Tesseract |
| AI | Groq API / Gemini |
| Data Processing | VB.NET (UiPath expressions) |
| Output | Excel Automation |

---

# 🛠 Setup Guide (Step-by-Step)

## 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/StudentEvaluationBot.git
cd StudentEvaluationBot

# 🧱 Architecture
