# HireSync — AI Resume Analyzer & Smart Shortlisting Platform

HireSync is a full-stack AI-powered recruitment platform designed to help recruiters shortlist candidates efficiently and assist jobseekers in improving their resumes using NLP-based insights.



# Overview

* Resume parsing
* Skill extraction
* Resume scoring
* Candidate ranking
* Recruiter & Jobseeker dashboards
* Authentication with JWT



# 🚀 Features

## 👨‍💼 Recruiter Features

* Upload multiple resumes
* Match resumes with job description
* AI ranking using TF-IDF + cosine similarity
* Accept/Reject workflow
* Automatically store accepted candidates in CSV

## 👩‍💻 Job Seeker Features

* Upload resume (PDF/DOCX)
* Extract skills from resume
* Resume scoring
* Improvement suggestions
* Predicted job role
* Video recommendations for skill improvement



# 🏗️ Architecture

```
React Frontend
 │
 ├── Node.js Auth (JWT + MySQL)
 └── FastAPI ML Backend (NLP + TF-IDF)
```



# 🛠️ TechStack

### Frontend

* React.js
* React Router
* Framer Motion
* Axios

### Backend 1 (Auth)

* Node.js
* Express
* MySQL
* bcryptjs
* JWT

### Backend 2 (AI/NLP)

* FastAPI
* spaCy
* scikit-learn
* pdfplumber
* PyMuPDF
* docx2txt

# ⚙️ Installation

### Clone the repo

```bash
git clone https://github.com/yourusername/HireSync.git
```

## NodeAuth Setup

```bash
cd backend
npm install
node server.js

```
## FastAPI Setup

```bash
cd backend/pyreparser

# Activate virtual environment
.\venv\Scripts\activate   # Windows

# Install Python dependencies (requirements.txt is in /backend)
pip install -r ../requirements.txt

# Download spaCy model
python -m spacy download en_core_web_sm

# Run backend
uvicorn main:app --reload
```
## ReactFrontend Setup

```bash
cd frontend
npm install
npm run dev
```

# 🧠 How It Works

## Job Seeker Flow

* Upload resume
* FastAPI extracts text
* NLP skill extraction
* Score + tips + predicted role

## Recruiter Flow

* Upload resumes + job description
* TF-IDF vectorization
* Cosine similarity
* Top candidates returned

# 🔗 API Endpoints

* `/parse-resume` — Single Resume Analysis
* `/upload` — Multiple Resume Matching
* `/accept_candidate` — Save Accepted Candidate
* `/auth/register` — Signup
* `/auth/login` — Login

# 🚀 Future Enhancements

* OCR support
* Semantic search with BERT
* Admin dashboard
* Database storage for candidates

# 👥 Contributors

* **Venkata Vidya Vandana** && **Team Members**

