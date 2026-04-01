# Smart-knowledge-ai
# 🧠 SmartKnowledge AI – Multimodal AI Assistant

SmartKnowledge AI is a production-style multimodal AI assistant that allows users to interact with AI using **text, voice, and PDF documents**. It integrates **Large Language Models (LLMs), Retrieval-Augmented Generation (RAG), speech processing, authentication, and persistent memory** into a single intelligent system.

---

# ✨ Features

- 🔐 Secure User Authentication (Signup / Login)
- 💬 ChatGPT-like conversational interface
- 📄 PDF Upload & Document-based Q&A (RAG with FAISS)
- 🧠 Context-aware responses using LLMs
- 🎙 Voice Input (Speech-to-Text)
- 🔊 Voice Output (Text-to-Speech using gTTS)
- 💾 Persistent Chat History (SQLite Database)
- 📥 Download Chat History
- 🎨 Modern Streamlit UI with responsive design

---

# 🛠 Tech Stack

| Layer       | Technology |
|------------|------------|
| Frontend   | Streamlit |
| Backend    | Python |
| AI / LLM   | Large Language Models (Gemini / OpenAI compatible) |
| RAG        | FAISS (Vector Database) |
| Speech     | SpeechRecognition, gTTS |
| Database   | SQLite |
| Auth       | Custom Authentication System |

---

# 📂 Project Structure
SmartKnowledge-AI/
│
├── app.py # Main Streamlit application
├── llm.py # LLM response generation logic
├── pdf_rag.py # PDF processing + FAISS RAG pipeline
├── voice_input.py # Speech-to-text module
├── auth.py # User authentication system
├── chat_db.py # Chat history management
├── database.py # SQLite setup
├── requirements.txt
└── README.md

---

# ⚙️ Installation & Setup

## 1️⃣ Clone Repository
```bash
git clone https://github.com/Feezakhan1801/smartknowledge-ai.git
cd smartknowledge-ai

2️⃣ Create Virtual Environment
python -m venv venv

venv\Scripts\activate

3️⃣ Install Dependencies

pip install -r requirements.txt

4️⃣ Run Application
streamlit run app.py

🧠 How It Works
User logs in securely
User asks question (text or voice)
Optional PDF upload for knowledge base
PDF is processed into chunks
FAISS retrieves relevant context (RAG)
LLM generates context-aware response
Chat history is saved in SQLite

🏗 System Architecture

User Input (Text / Voice / PDF)
            ↓
     Streamlit UI Layer
            ↓
 Authentication System
            ↓
 Chat Interface Module
            ↓
 PDF Processing (Optional)
            ↓
 FAISS Vector Store (RAG)
            ↓
     LLM Engine (AI Response)
            ↓
 Voice Output (TTS)
            ↓
 SQLite Database (Memory)

🎯 Use Cases
📄 AI Document Assistant
🎙 Voice-enabled Chatbot
🧠 Knowledge Base Q&A System
🏢 Enterprise AI Assistant
📚 Personal Study Assistant
