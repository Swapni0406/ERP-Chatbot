# ERP Chatbot (Demo Version)

This project is a **Flask-based AI Chatbot** for ERP systems that uses **OpenAI GPT** to process employee queries related to leave management, clock-in/clock-out, and attendance tracking.

---

## 🚀 Features
- Intent recognition powered by GPT-4o-mini  
- Leave application via natural language  
- Clock-in/out management  
- Smart entity extraction (dates, reasons, types)  
- Modular backend integration  
- Secure `.env` configuration (no credentials in code)

---

## 🧠 Architecture
The system flow:
1. User sends natural message (e.g., *"Apply sick leave for tomorrow till Friday"*).
2. GPT extracts intent (`apply_leave`) and entities (leave type, start/end date, reason).
3. Chatbot validates and sends structured payload to backend.
4. Backend processes the request and returns status.
5. GPT generates concise confirmation.

---

## 🧩 Tech Stack
- **Python 3.9+**
- **Flask** (API Framework)
- **OpenAI GPT-4o-mini** (Intent + NLP)
- **Requests** (Backend communication)
- **dotenv** (Environment management)

---

## ⚙️ Setup
```bash
git clone https://github.com/yourusername/erp-chatbot.git
cd erp-chatbot
pip install -r requirements.txt
cp .env.example .env
