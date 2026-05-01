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

2️⃣ Open in UiPath Studio
Open Main.xaml
Click Manage Packages → Restore
3️⃣ Install Required Packages

Ensure these packages are installed:

UiPath.System.Activities
UiPath.Excel.Activities
UiPath.PDF.Activities
UiPath.OCR.Activities
UiPath.IntelligentOCR.Activities
Newtonsoft.Json
4️⃣ Configure API Key

In UiPath:

Go to Variables Panel
Set:
apiKey = "YOUR_API_KEY"

⚠️ Never commit your API key to GitHub

5️⃣ Prepare Input Files

Place files in:

InputFiles/
Required Files:
QuestionPaper.pdf
MarkingScheme.pdf
Student Files:
InputFiles/Students/

Example:

student1.pdf
student2.pdf
6️⃣ Verify File Paths

Check in Main.xaml:

Directory.GetFiles("InputFiles\Students","*.pdf")
7️⃣ Run the Workflow
Click ▶ Run
Wait for execution
📊 Output

Generated file:

Output/EvaluationResults.xlsx
Output Format
Name	Score	Feedback	Suggestions
🧠 Workflow Logic
1. Input Processing
Reads question paper and marking scheme
Loads student PDFs dynamically
2. OCR Layer
Extracts text using OCR engine
3. Preprocessing
Cleans text
Removes unnecessary formatting
4. Prompt Engineering
Builds structured prompt:
Score:
Feedback:
Suggestions:
5. AI Evaluation
Sends prompt to LLM API
Receives evaluation response
6. Parsing Layer
Extracts:
Score
Feedback
Suggestions
7. Data Structuring
Stores in DataTable
8. Output Layer
Writes to Excel

# 🧱 Architecture
