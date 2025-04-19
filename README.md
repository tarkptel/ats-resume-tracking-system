<div align="center">

  <a href="https://tarkptel.github.io/">
    <img src="https://img.shields.io/badge/🌐-Portfolio-blue" height="28">
  </a>
  <a href="https://www.kaggle.com/tark01/">
    <img src="https://img.shields.io/badge/-Kaggle-20BEFF?logo=kaggle&logoColor=white" height="28">
  </a>
  <a href="https://www.linkedin.com/in/tark-patel/">
    <img src="https://img.shields.io/badge/-LinkedIn-0077B5?logo=linkedin&logoColor=white" height="28">
  </a>

</div>

<h1 align="center"> 🏆 ATS Resume Score Checker</h1>

AI-powered app that evaluates your resume against a job description using **Google Gemini 1.5 Flash** — simulating how modern **ATS (Applicant Tracking Systems)** work.<br><br>

🔗 **Live Demo**: [View on Hugging Face](https://huggingface.co/spaces/tarkpatel/ATS-Tracking-System)  
📁 **Portfolio Post**: [Read Blog Post](https://tarkptel.github.io/posts/ats-resume-checker/) <br><br>



## 📌 Features

- **Job Description Input**
- **PDF Resume Upload**
- **Gemini Evaluation**
  - Match percentage score
  - Missing keywords
  - Strengths & weaknesses
- **ATS-style feedback**
- Fast, lightweight Streamlit frontend <br><br>



##	⚡ Workflow

1. User enters the job description.
2. User uploads a resume (PDF format).
3. The first page of the resume is converted to an image.
4. The image + job description are passed to **Google Gemini 1.5 Flash**.
5. Gemini returns a detailed match score and recommendations. <br><br>



## 🚀 Tech Stack

| Component      | Tech Used                        |
|----------------|----------------------------------|
| Frontend       | Streamlit                        |
| AI Model       | Google Gemini 1.5 Flash API      |
| Image Parsing  | `pdf2image`, `PIL`               |
| Hosting        | Hugging Face Spaces              | <br><br>


## 📁 How to Run Locally

### 1. Clone the repo

```bash
git clone https://github.com/yourusername/ats-resume-checker.git
cd ats-resume-checker 
```

### 2. Create and activate a virtual environment (optional)
```
python -m venv venv
source venv/bin/activate  # or `venv\Scripts\activate` on Windows
```

### 3. Install dependencies
```
pip install -r requirements.txt
```

### 4. Add your API key
```
Create a .env file in the root directory:
GOOGLE_API_KEY=your_gemini_api_key_here
```
🔐 Don't share your key publicly!

### 5. Run the app
```
streamlit run app.py
```

<br><br>

## Gemini Prompts Used

### 🎯 Resume Evaluation Prompt

> You are an experienced Technical Human Resource Manager, your task is to review the provided resume against the job description.  
> Please share your professional evaluation on whether the candidate's profile aligns with the role.  
> Highlight the strengths and weaknesses of the applicant in relation to the specified job requirements.

### 📈 Match Score Prompt

> You are a skilled ATS (Applicant Tracking System) scanner with a deep understanding of data science and ATS functionality,  
> your task is to evaluate the resume against the provided job description. Give me the percentage of match if the resume matches  
> the job description. First the output should come as percentage and then keywords missing and last final thoughts.

Both prompts are dynamic and tailored to extract detailed feedback from the **Gemini API**.

<br><br>

## 🙋‍♂️ About Me

Made with 💙 by **Tark Patel**  
Check out my [**portfolio**](https://tarkptel.github.io/) for more **AI + ML projects**.

