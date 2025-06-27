# Smartie Chat – eity20 Supportive Chatbot

Smartie is a supportive chatbot designed to help people stay consistent with their health and wellbeing goals using the **eity20 approach** — 80% consistency, 20% flexibility. It offers friendly, empowering responses across physical, mental, and gut health topics, using the SMARTS Framework.

---

## 🌱 Project Purpose

Smartie supports users in a holistic way by recognising that:
- **Food, stress, mood, and mindset are all connected**
- **Health isn’t all-or-nothing** — consistency and flexibility matter
- **Stress and cravings are normal** — guilt-free guidance makes habits sustainable

Smartie gently encourages users to reflect, realign, and take action without judgement.

---

## ⚙️ Features

- Friendly, human-style chat using OpenAI
- Personalised tone with eity20 values (SMARTS Framework)
- Encouraging, non-judgemental support for wellbeing choices
- Linked to a simple front-end chat interface
- Conversation-saving functionality
- Pinned eity20 logo for branding

---

## 📁 Project Structure

```
smartie-chat/
│
├── index.html               # Main frontend HTML with chat interface
├── style.css                # (optional if separated) Styles for layout and chat UI
├── script.js                # JS for sending/receiving messages
├── smartie_flask_backend.py # Flask backend that handles OpenAI responses
├── eity20_logo.png          # Branded logo shown on the chat
└── README.md                # You're here!
```

---

## 🚀 How to Run Locally

### 🧠 Prerequisites

- Python 3.10+
- Node.js (if adding advanced frontend build tools – optional)
- OpenAI API key with access to `gpt-3.5-turbo`
- Flask + CORS

### 🔧 Backend Setup

1. Clone the repo
2. Install dependencies:

```bash
pip install flask flask-cors openai
```

3. Set your OpenAI API key:

```bash
export OPENAI_API_KEY="your-key-here"
```

4. Run Flask server:

```bash
python smartie_flask_backend.py
```

Server will be live on: `http://localhost:5000/smartie`

---

### 💬 Frontend Setup

Open `index.html` in your browser. Make sure the fetch URL in `script.js` or inline `<script>` is pointing to:

```javascript
fetch("http://localhost:5000/smartie", { ... });
```

> ⚠️ If deployed (e.g. Render), update to your live URL.

---

## 💡 Deployment (e.g. Render)

1. Deploy Flask app to Render with the `OPENAI_API_KEY` in environment variables.
2. Ensure port binding is set to 5000.
3. Point frontend `fetch()` URL to your Render backend domain.

---

## 🧠 The SMARTS Framework

Smartie’s responses are powered by the **eity20 SMARTS mindset**:
- **S**ustainable
- **M**indful mindset
- **A**ligned
- **R**ealistic
- **T**rain your brain
- **S**peak up

---

## 🧪 Future Features

- User authentication
- Chat history tracking
- Multi-pillar progress suggestions (from eity20)
- Improved scroll and mobile support
- Enhanced tone customisation

---

## 📸 Branding

This chat experience is part of the **eity20** wellbeing ecosystem.  
The logo (`eity20_logo_transparent_FINAL.png`) is pinned to the top of the interface for brand continuity.

---

## 🤝 Credits

Created by Dr Kerry Swanton, eity20  
Built using:  
- Flask + OpenAI API  
- HTML, CSS, JavaScript  

---

## 📬 Questions or Help?

Feel free to get in touch at: [your contact or link]
