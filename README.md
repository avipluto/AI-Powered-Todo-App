 AI-Powered-Todo-App

 Description
An intelligent Todo application that leverages OpenAI's natural language processing to categorize tasks, suggest deadlines, and understand user input via natural language. Built with React (frontend), Node.js + Express (backend), and MongoDB for storage.

---

 Features
- ✅ Smart task categorization using AI
- 🕒 Deadline suggestion based on task description
- ✍️ Natural language task entry (e.g., "Remind me to buy groceries tomorrow")
- 📁 Persistent storage with MongoDB
- 🧠 OpenAI integration for intelligent task processing

---
 Tech Stack
- **Frontend**: React
- **Backend**: Node.js, Express
- **Database**: MongoDB (Mongoose)
- **AI Service**: OpenAI API

---
Folder Structure
```
ai-todo-app/
├── client/                 # React frontend
│   ├── public/
│   └── src/
│       ├── components/
│       ├── pages/
│       ├── App.js
│       └── index.js
│
├── server/                 # Node.js + Express backend
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   ├── services/           # OpenAI integration
│   ├── app.js
│   └── server.js
│
├── .env                   # Environment variables
├── .gitignore
├── package.json
├── README.md
└── README.md
```

---

Setup Instructions

 Prerequisites
- Node.js & npm
- MongoDB (local or Atlas)
- OpenAI API key
 Environment Variables (`.env`)
```
MONGO_URI=your_mongodb_connection_string
OPENAI_API_KEY=your_openai_api_key
PORT=5000
```

---

Run Locally

Backend
```bash
cd server
npm install
npm run dev
```

 Frontend
```bash
cd client
npm install
npm start
```

---
 API Routes (Backend)
- `POST /api/tasks`: Add task (uses OpenAI to categorize and suggest deadline)
- `GET /api/tasks`: Fetch all tasks
- `DELETE /api/tasks/:id`: Delete task

---
 Future Enhancements
- [ ] User authentication (JWT)
- [ ] Task reminders via email
- [ ] Dark mode UI
- [ ] Voice input for tasks

---
 License
MIT
