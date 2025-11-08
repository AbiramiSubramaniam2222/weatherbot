# ☁️ Chatbot Weather Assistant  
### 🔹 Rasa | OpenWeather API | Docker | Python

![Chatbot Demo](https://github.com/AbiramiSubramaniam2222/weatherbot/blob/main/images/Weatherbot%20screenshot%20image.png)

---

## 💬 Overview  
This project is an **AI-powered chatbot** built using the **Rasa open-source framework** that provides **real-time weather updates**.  
It connects to the **OpenWeatherMap API**, processes user input with **NLP**, and responds conversationally with temperature, humidity, and weather conditions for any city.

---

## 🧠 Key Features
- 🌦️ Fetches live weather data using **OpenWeatherMap API**  
- 💬 Built with **Rasa NLU and Core** for intent recognition and dialogue management  
- 🐳 Fully **containerized with Docker** for easy deployment  
- ⚙️ Modular architecture with customizable intents and responses  
- 📡 REST API integration for real-time responses  

---

## 🧰 Tech Stack
- **Framework:** Rasa (Open Source)  
- **Language:** Python  
- **API:** OpenWeatherMap API  
- **Containerization:** Docker  
- **Libraries:** requests, json, asyncio  

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the repository  
```bash
git clone https://github.com/AbiramiSubramaniam2222/weatherbot.git
cd weatherbot
2️⃣ Build Docker image
bash
Copy code
docker build -t weatherbot .
3️⃣ Run the chatbot container
bash
Copy code
docker run -p 5005:5005 weatherbot
4️⃣ Chat with your bot
Once it’s running, open your terminal and type:

bash
Copy code
rasa shell
Or access via REST API at:

bash
Copy code
http://localhost:5005/webhooks/rest/webhook

📂 Repository
👉 View on GitHub
