# Chatbot-api-Openrouter
# 🤖 AI Chatbot with OpenRouter API

This is a simple FAQ chatbot project built using **OpenRouter (ChatGPT) API**, hosted on an **AWS EC2 instance**. The chatbot is integrated into a basic HTML frontend and served via a Node.js Express backend.

---

## 🌐 Live Demo

**URL:** http://<your-ec2-public-ip>:5000  
> _(Replace with your actual EC2 IP if you want others to test)_

---

## 🛠️ Tech Stack

- **Frontend:** HTML, CSS, Vanilla JS
- **Backend:** Node.js, Express.js
- **AI Integration:** OpenRouter (ChatGPT API)
- **Hosting:** AWS EC2 (Ubuntu)

---

## 📂 Project Structure


---

## ⚙️ How to Run Locally

### 1. Clone the Repo
```bash
git clone https://github.com/Aryantyagi21/Chatbot-api-Openrouter.git
cd Chatbot-api-Openrouter


## ⚙️ EC2 Setup Commands (For Reference)

> This section lists all commands used to set up the chatbot backend on an Ubuntu EC2 server.

```bash
# Step 1: Update system
sudo apt update

# Step 2: Install Node.js v18 and Git
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
sudo apt install -y nodejs git

# Step 3: Create project directory and initialize
mkdir chatbot-api.ai
cd chatbot-api.ai
npm init -y

# Step 4: Install dependencies
npm install express cors body-parser dotenv openai axios

# Step 5: Create files
nano index.js
nano .env

# Step 6: Run the server
node index.js

# Step 7: Frontend setup
mkdir public
cd public
nano index.html
cd ..

# Step 8: Serve frontend
npm install -g http-server
npx http-server ./public

# Step 9: Test chatbot
curl -X POST http://localhost:5000/chat \
     -H "Content-Type: application/json" \
     -d '{"message": "What is XploreSports?"}'

# Step 10: GitHub repo setup
git init
git remote add origin https://github.com/Aryantyagi21/Chatbot-api-Openrouter.git
git add .
git commit -m "Initial commit"
git pull origin main --allow-unrelated-histories
git push -u origin main
