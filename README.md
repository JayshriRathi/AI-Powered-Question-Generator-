# 📘 AI-Powered Question Generator

An interactive web app to generate intelligent educational questions (MCQs, MSQs, Fill-in-the-Blanks, and Math with step-by-step solutions) from uploaded text documents using Google Gemini Pro. Built using **Streamlit** and designed for easy deployment on **Google Colab**.

---

## 🔍 Features

- ✅ Upload `.pdf`, `.docx`, or `.txt` files
- ✅ Extracts key content using NLP
- ✅ Choose number of questions
- ✅ Choose difficulty level: `Easy`, `Intermediate`, `Tough`
- ✅ Automatically generates:
  - MCQs (single correct)
  - MSQs (multiple correct)
  - Fill-in-the-Blank
  - Math questions with step-by-step solutions
  - Descriptions of diagrams (if applicable)
- ✅ Download questions as `.txt` or `.pdf`

---

## 🧪 Demo
![Screenshot 2025-04-13 165728](https://github.com/user-attachments/assets/4b3f857f-bfb4-4228-b48b-95b025621bac)






---

## 📄 Required API Key

This project uses [Google Gemini](https://makersuite.google.com/app/apikey).

1. Visit [https://makersuite.google.com/app/apikey](https://makersuite.google.com/app/apikey)
2. Copy your API key
3. Paste it in `app.py`:

```python
os.environ["GOOGLE_API_KEY"] = "your-api-key-here"
```

---

## 📦 Dependencies

```txt
streamlit
fpdf
pdfplumber
python-docx
google-generativeai
pyngrok
```

---

## 🚀 Deployment Options

### ✅ Run on Google Colab (Streamlit + Ngrok):
- Works even without local setup
- Best for beginners

### ✅ Or run locally with:
```bash
streamlit run app.py
```

---

## 🖼 Sample Output Format

```text
### QUESTION
Type: MCQ
Question: What is the capital of France?
A) Berlin
B) Paris
C) Madrid
D) Rome
Correct Answer: B
Explanation: Paris is the capital of France.

---

### QUESTION
Type: Math
Question: Solve 2x + 3 = 11
Correct Answer: x = 4
Explanation:
Step 1: Subtract 3 from both sides → 2x = 8
Step 2: Divide by 2 → x = 4
```


