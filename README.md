# 🩺 VR Patient Simulator

An AI-powered medical training tool that allows students to interact with **virtual patients** in different **personas** — calm, anxious, rude, or overly patient.
Built with **FastAPI (backend)** and **React + Vite (frontend)**, it uses **Groq API / LLMs** to simulate realistic patient responses.

---

## 🚀 Features

* 🎭 **Multiple Personas**: Patients behave differently (Calm, Anxious, Rude, Overly Patient).
* 💬 **Chat-like UI**: Doctor–Patient conversation in a **WhatsApp-style chat interface**.
* 🧠 **AI Responses**: Powered by Groq LLM (or fallback to OpenAI / HuggingFace models).
* 🎨 **Modern UI**: Responsive, card-based interface with customizable themes.
* ⚡ **Lightweight**: Runs locally with FastAPI + Vite.

---

## 📂 Project Structure

```
vr-patient-simulator/
│── backend/                # FastAPI backend
│   ├── app.py              # FastAPI entrypoint
│   ├── patient_api.py      # AI integration (Groq/OpenAI/HF)
│   ├── requirements.txt    # Backend dependencies
│   └── .env                # API keys & settings
│
│── frontend/               # React + Vite frontend
│   ├── src/
│   │   ├── App.jsx         # Main React app
│   │   ├── main.jsx        # Entry file
│   │   ├── api.js          # Connects to backend
│   │   ├── index.css       # Styling
│   │   └── index.html      # HTML entry
│   ├── package.json        # Frontend dependencies
│   └── vite.config.js      # Vite config
│
└── README.md               # Project documentation
```

---

## ⚙️ Installation & Setup

### 🔹 1. Clone the repository

cd vr-patient-simulator
```

---

### 🔹 2. Backend Setup

```bash
cd backend
pip install -r requirements.txt
```

Create a **`.env`** file inside `backend/`:

```
GROQ_API_KEY=your_groq_api_key_here
USE_LOCAL_MODEL=false
```

Run the backend:

```bash
uvicorn app:app --reload --host 0.0.0.0 --port 8000
```

---

### 🔹 3. Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

Frontend runs at 👉 `http://localhost:5173/`
Backend runs at 👉 `http://localhost:8000/`

---

## 🖼️ Screenshots

### 🏠 Home UI

Doctor selects persona + types question.
<img width="1898" height="874" alt="image" src="https://github.com/user-attachments/assets/096ca229-a26a-4098-a5fe-117f5f332c84" />


### 💬 Chat Window
<img width="1888" height="878" alt="image" src="https://github.com/user-attachments/assets/c3fe2947-2fec-48ba-b7d7-7f5fb55068c5" />


## 🔮 Future Enhancements

* 🎙️ **Voice Support** (Text-to-Speech for patient responses).
* 🧾 **Patient Profiles** (Age, Gender, Condition).
* 🕶️ **Full VR Integration** with 3D avatars.
* 📊 **Analytics Dashboard** for student progress.

---

## 👩‍⚕️ Use Case

This project is designed for **medical schools, training centers, and rural students** who may not always have access to real patients.
It allows **safe, repeatable, and controlled** practice of doctor–patient interactions.

---

## 🤝 Contributing

Contributions are welcome! Please fork the repo and create a PR.


