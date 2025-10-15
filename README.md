# 🩺 Healthcare Symptom Checker (Educational Purpose)

### 📘 Overview
The **Healthcare Symptom Checker** is an AI-powered application that takes user symptom descriptions and provides **probable conditions** and **recommended next steps** — strictly for **educational purposes only**.  

It demonstrates how **Large Language Models (LLMs)** can assist in symptom interpretation while emphasizing **safety, reasoning quality, and clear disclaimers**.

---

### 🎯 Objective
- **Input:** Free-form symptom text from user  
- **Output:** Probable conditions + recommended next steps  
- **Goal:** Educational reasoning only (no diagnosis or treatment)

---

### ⚙️ Features
- ✅ **Single Python file** — no separate frontend or backend  
- 🧠 **OpenAI LLM integration** for reasoning and suggestions  
- 💾 **Local SQLite database** to store query history  
- 📜 **Automatic disclaimers** and emergency awareness  
- 🧩 Simple **Streamlit UI** for instant demo  
- 📤 **CSV export** of query history  

---

### 🧠 Example Prompt Used
> “Based on these symptoms, suggest possible conditions and next steps with educational disclaimer.”

---

### 🛠️ Tech Stack
| Component | Technology |
|------------|-------------|
| Framework | Streamlit |
| Language | Python |
| AI Model | OpenAI GPT (gpt-3.5-turbo or later) |
| Database | SQLite (local) |

---

### 🚀 Setup & Run

#### 1️⃣ Clone this Repository
```
git clone https://github.com/Saketh16coder/Healthcare-Symptom-Checker.git
cd Healthcare-Symptom-Checker
```

### 2️⃣ Install Dependencies
```
pip install -r requirements.txt
```

### 3️⃣ Set Your API Key
Set your OpenAI API Key as an environment variable:

Windows (PowerShell):
```
setx OPENAI_API_KEY "sk-yourkeyhere"
```

macOS/Linux (bash/zsh):
```
export OPENAI_API_KEY="sk-yourkeyhere"
```

### 4️⃣ Run the App
```
streamlit run app.py
```
Then open your browser and go to 👉 http://localhost:8501

| Symptom Input                                                   | Expected Output                                |
| --------------------------------------------------------------- | ---------------------------------------------- |
| `Fever, sore throat, mild cough, started 2 days ago`            | Common cold / viral infection; self-care steps |
| `Sudden chest pain, sweating, shortness of breath`              | **Emergency alert** – seek immediate care      |
| `Frequent urination, excessive thirst, unexplained weight loss` | Possible diabetes; medical evaluation advised  |
| `Itchy rash after using new soap`                               | Possible allergic reaction; avoid irritant     |

📦 Deliverables
✅ Working Streamlit app (app.py)
✅ README file (this file)
✅ Demo video showcasing functionality

| Criteria              | Description                                 |
| --------------------- | ------------------------------------------- |
| **Correctness**       | Logical and medically coherent outputs      |
| **Reasoning Quality** | Clear, safe, and explainable responses      |
| **Safety Disclaimer** | Prominent educational disclaimer            |
| **Code Quality**      | Clean, single-file Streamlit implementation |


### ⚠️ Disclaimer
⚕️ This app is intended for educational and informational use only.
It does not provide medical advice, diagnosis, or treatment.
Always seek professional medical care for any serious or persistent symptoms.

### 🧩 Future Enhancements
Add keyword-based triage system for local emergency detection
Deploy on Streamlit Cloud / AWS
Include voice input for symptoms
Add basic analytics dashboard for usage insights
