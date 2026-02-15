# 🧠 Cognivise AI

**Where Understanding Becomes Visible**

Cognivise AI is a confusion-aware learning assistant that diagnoses conceptual misunderstandings instead of simply answering questions.

Unlike traditional AI tutors, Cognivise identifies *why* a learner is confused and repairs flawed mental models using structured explanation and reinforcement.

---

## 🚀 Problem

Most AI learning tools:
- Provide generic explanations
- Do not detect misconception patterns
- Encourage memorization instead of understanding

Learners often:
- Repeat the same conceptual mistakes
- Misunderstand foundational logic
- Struggle with mental model clarity

---

## 💡 Solution

Cognivise AI introduces a **diagnostic-first learning system**:

1. Generates targeted diagnostic questions  
2. Analyzes learner responses  
3. Identifies confusion type  
4. Repairs the mental model  
5. Provides reinforcement exercise  
6. Tracks confusion patterns  

This ensures conceptual reconstruction, not passive consumption.

---

## ⚙️ Features

- 🧠 Diagnostic Question Engine
- 🔍 Confusion Classification System
- 📘 Structured Mental Model Repair
- 🎯 Reinforcement Module
- 📊 Confusion Heatmap Dashboard

---

## 🏗 Architecture

Frontend:
- HTML / CSS / JavaScript

Backend:
- FastAPI (Python)

AI Layer:
- LLM-based diagnostic and classification engine

Storage:
- In-memory session tracking (MVP)

---

## 🔄 How It Works

1. User selects a concept (e.g., Recursion).
2. System generates diagnostic questions.
3. User submits answers.
4. AI classifies confusion type.
5. Targeted explanation + reinforcement is provided.
6. Dashboard updates confusion trends.

---

## 🧪 MVP Scope

- 3–5 Data Structures & Algorithms topics
- Diagnostic + classification pipeline
- Structured AI outputs
- Basic confusion tracking dashboard

---

## 📂 Project Structure

CogniviseAI/
│
├── backend/
│   ├── app/
│   │   ├── main.py              # FastAPI entry point
│   │   ├── routes.py            # API route definitions
│   │   ├── services/
│   │   │   ├── diagnostic.py    # Diagnostic question generator
│   │   │   ├── classifier.py    # Confusion classification logic
│   │   │   └── reinforcement.py # Reinforcement logic
│   │   ├── models/
│   │   │   └── schemas.py       # Pydantic request/response models
│   │   ├── storage/
│   │   │   └── tracker.py       # Confusion tracking system
│   │   └── config.py            # Environment + API configuration
│   │
│   ├── requirements.txt
│   └── .env                     # API keys (NOT committed)
│## ▶️ How to Run Cognivise AI (Local Setup)

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/<your-username>/CogniviseAI.git
cd CogniviseAI
```

---

### 2️⃣ Setup Backend

```bash
cd backend

# Create virtual environment
python -m venv venv

# Activate virtual environment
# Windows:
venv\Scripts\activate

# Mac/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
```

---

### 3️⃣ Add Environment Variables

Create a `.env` file inside the `backend/` folder:

```
OPENAI_API_KEY=your_api_key_here
```

⚠️ Do NOT commit this file to GitHub.

---

### 4️⃣ Start Backend Server

```bash
uvicorn app.main:app --reload
```

If using simple structure (single main.py):

```bash
uvicorn main:app --reload
```

Backend will run at:
```
http://127.0.0.1:8000
```

---

### 5️⃣ Open Frontend

Go to:

```
frontend/index.html
```

Open it directly in your browser.

---

### ✅ Test API (Optional)

Visit:
```
http://127.0.0.1:8000/docs
```

FastAPI interactive documentation will appear.
├── frontend/
│   ├── index.html               # Main UI
│   ├── style.css                # Styling
│   └── script.js                # API calls + UI logic
│
├── docs/
│   ├── DESIGN.md                # System design document
│   └── architecture.png         # (Optional diagram)
│
├── .gitignore
├── README.md
└── LICENSE


