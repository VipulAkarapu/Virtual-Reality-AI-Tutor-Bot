# Virtual-Reality-AI-Tutor-Bot
"The source code is in the releases section"


# 🤖 VR AI Tutor

A high-performance Node.js backend powering an AI-driven Virtual Reality tutor and interactive chatbot. Built to seamlessly integrate with React Three Fiber (R3F) frontends, handling real-time AI prompt responses, text-to-speech (TTS) audio generation, and 3D avatar synchronization.

---

## 🚀 Features

* **AI Chat Processing:** Connects user prompts to LLM endpoints for contextual responses.
* **Audio & TTS Pipeline:** Generates and serves `.mp3` / `.wav` audio files alongside facial animation and lip-sync JSON data.
* **R3F Ready:** Built specifically to stream structured payloads to React Three Fiber web clients.
* **Environment Configuration:** Secure secret management using `.env` templates.

---

## 🛠 Tech Stack

* **Runtime:** [Node.js](https://nodejs.org/) (v18+)
* **Package Manager:** [Yarn](https://yarnpkg.com/)
* **Core Libraries:** Express / Node ecosystem, OpenAI / TTS API integration
* **Client Compatibility:** React Three Fiber (R3F) / Three.js

---

## 📁 Project Structure

```text
.
├── audios/           # Cache directory for generated audio and lip-sync metadata
├── .env.example      # Environment variable configuration template
├── .gitignore        # Git exclusion rules
├── package.json      # Dependencies and scripts
└── README.md         # Project documentation



The 3D virtual friend application will be live at http://localhost:5173



## Frontend setup:
# Open a new terminal and navigate into frontend
cd frontend

# Install dependencies
yarn install

# Start Vite dev server
yarn dev


## Docker Deployment:

cd backend

# Build Docker image
docker build -t r3f-virtual-friend-backend .

# Run container with environment variables
docker run -d -p 3000:3000 --env-file .env r3f-virtual-friend-backend

## PM2 PROCESS MANAGER SETUP:

# Install PM2 globally
npm install pm2 -g

# Start server
cd backend
pm2 start server.js --name "vr-ai-backend"

# Setup auto-restart on system reboot
pm2 startup
pm2 save


📄 License
This project is licensed under the MIT License.
