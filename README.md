# campusmindaiauthentication
🧠 CampusMind AI

«An AI-powered academic assistant that helps students learn, research, organize knowledge, and maintain persistent academic conversations.»

CampusMind AI is a full-stack AI academic assistant designed to provide students with an intelligent and personalized learning experience.

The platform combines a modern Next.js frontend, FastAPI backend, MongoDB persistent storage, JWT authentication, and a local Ollama-powered LLM pipeline to create a secure and intelligent academic workspace.

---

🚀 Key Features

🤖 AI Academic Assistant

- Interactive AI-powered chatbot
- Academic question answering
- Local LLM inference using Ollama
- Fast and responsive conversational experience

💬 Multi-Threaded Conversations

- Create and manage multiple chat threads
- Organize conversations by topic
- Maintain separate academic discussions

🧠 Persistent Memory Bank

- Stores previous conversations
- Maintains user-specific academic history
- Enables students to revisit previous discussions

🔐 Secure Authentication

- Student registration and login
- JWT-based authentication
- Protected dashboard and API endpoints
- Secure logout functionality

👤 User Profile

- Personalized student profile
- User-specific conversations and data
- Protected account information

🎨 Modern AI Interface

- Cyberpunk-inspired AI theme
- Neon cyan and purple accents
- Glassmorphism UI
- Responsive design
- Futuristic academic workspace

---

🏗️ System Architecture

                    CAMPUSMIND AI
                         │
                         ▼
                ┌─────────────────┐
                │    Next.js      │
                │    Frontend     │
                └────────┬────────┘
                         │
                    REST APIs
                         │
                         ▼
                ┌─────────────────┐
                │     FastAPI     │
                │     Backend     │
                └───────┬─┬───────┘
                        │ │
              ┌─────────┘ └─────────┐
              ▼                     ▼
       ┌──────────────┐      ┌──────────────┐
       │   MongoDB    │      │    Ollama    │
       │   Database   │      │   Local LLM  │
       └──────────────┘      └──────────────┘

---

🔄 Application Workflow

Student
   │
   ▼
Signup / Login
   │
   ▼
JWT Authentication
   │
   ▼
CampusMind Dashboard
   │
   ▼
Ask Academic Question
   │
   ▼
Next.js Frontend
   │
   ▼
FastAPI REST API
   │
   ├──────────────► MongoDB
   │                  │
   │                  └── User & Chat Memory
   │
   └──────────────► Ollama
                      │
                      └── Local AI Response
   │
   ▼
FastAPI
   │
   ▼
Next.js
   │
   ▼
AI Response Displayed

---

🔗 Frontend–Backend Communication

The frontend communicates with the backend through REST APIs over HTTP.

For example:

Next.js
   │
   │ POST /login
   ▼
FastAPI
   │
   ▼
MongoDB
   │
   ▼
JWT Token
   │
   ▼
Next.js

For AI conversations:

Next.js
   │
   │ Chat Request
   ▼
FastAPI
   │
   ├──► MongoDB
   │
   └──► Ollama
          │
          ▼
       Local LLM
          │
          ▼
       AI Response
   │
   ▼
Next.js

This architecture keeps the frontend, backend, database, and AI model properly separated.

---

🛠️ Technology Stack

Layer| Technology
Frontend| Next.js, React
Backend| Python, FastAPI
Database| MongoDB
Authentication| JWT
AI Runtime| Ollama
AI Model| Local LLM
API Communication| REST API / HTTP
UI| Modern responsive web interface
Version Control| Git & GitHub

---

📁 Project Structure

CampusMind-AI/
│
├── frontend/
│   ├── components/
│   ├── pages/
│   ├── app/
│   ├── public/
│   └── ...
│
├── backend/
│   ├── app/
│   │   ├── main.py
│   │   ├── routes/
│   │   ├── models/
│   │   ├── services/
│   │   └── ...
│   ├── requirements.txt
│   └── ...
│
├── README.md
└── ...

«The exact structure may vary depending on the final project organization.»

---

⚙️ How It Works

1. User Registration

A student creates an account through the Next.js frontend.

The request is sent to FastAPI, which validates the information and stores the user data in MongoDB.

2. Secure Login

The student logs in with their credentials.

FastAPI verifies the account and generates a JWT authentication token.

3. Protected Dashboard

The JWT token is used to authenticate requests to protected backend endpoints.

4. AI Conversation

The student enters an academic question.

The frontend sends the request to FastAPI.

FastAPI communicates with Ollama, which runs the local language model and generates the response.

5. Persistent Memory

Conversation information is stored in MongoDB so that users can access their previous academic discussions.

6. Response

The generated AI response is returned through FastAPI and displayed in the Next.js interface.

---

🔐 Security

CampusMind AI uses authentication and protected API access to provide a secure user experience.

Security features include:

- JWT-based authentication
- Protected backend routes
- User-specific data
- Authentication-aware dashboard
- Secure logout
- Backend-controlled database access

---

💡 Why Ollama?

Instead of relying entirely on external cloud AI APIs, CampusMind AI uses Ollama to run an LLM locally.

This provides:

- Local AI inference
- Reduced dependency on external API services
- Better control over the AI pipeline
- Useful development and experimentation environment

---

🧠 Why MongoDB?

MongoDB provides flexible document-based storage for:

- User information
- Chat threads
- Messages
- Conversation history
- Persistent memory

This allows CampusMind AI to maintain a personalized academic workspace for each student.

---

🎯 Future Enhancements

Planned improvements include:

- 📄 Export memory bank to PDF/Markdown
- 🔎 Advanced vector-based semantic search
- 🎙️ Voice-to-text academic prompts
- 📚 Enhanced RAG-based academic knowledge retrieval
- 📊 Personalized learning analytics
- 🔔 Smart academic reminders
- 🌐 Additional AI model support

---

🏆 Hackathon Highlights

CampusMind AI demonstrates the integration of:

Frontend + Backend + Database + Authentication + Local AI

Next.js
   +
FastAPI
   +
MongoDB
   +
JWT
   +
Ollama
   =
CampusMind AI

The project focuses on creating a secure, personalized, and intelligent academic assistant for students.

---

👥 Team

CampusMind AI — Hackathon Project

Built with a focus on:

- Artificial Intelligence
- Full-Stack Development
- Personalized Learning
- Secure Authentication
- Persistent Knowledge Management

---

📌 Project Status

🟢 Core full-stack integration completed

Implemented and tested:

- ✅ Student Signup
- ✅ Secure Login
- ✅ JWT Authentication
- ✅ Protected Dashboard
- ✅ Multi-threaded AI Chat
- ✅ Ollama Local AI Pipeline
- ✅ MongoDB Persistence
- ✅ Memory Bank
- ✅ User Profile
- ✅ Logout
- ✅ Frontend–Backend Integration

---

⭐ Support

If you find this project interesting, consider giving the repository a ⭐ on GitHub.

CampusMind AI — Your Intelligent Academic Companion.
