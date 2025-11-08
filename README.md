# ☁️ Chatbot Weather Assistant  
### 🔹 Rasa | OpenWeather API | Docker | Python

![Chatbot Demo](https://github.com/AbiramiSubramaniam2222/weatherbot/blob/main/chatbot_screenshot.png)

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

## Project Structure

- `actions/`  
  Contains the custom action file with `ActionWeather` class that calls the OpenWeatherMap API.

- `.env`  
  Stores your OpenWeatherMap API key (this file should **not** be committed to GitHub).

- `.gitignore`  
  Ensures sensitive files like `.env` are ignored by Git.

- `README.md`  
  This file.

- Other Rasa project files (domain, data, config) governing chatbot behavior.

## Setup Instructions

1. **Clone the repository:**

    ```
    git clone https://github.com/AbiramiSubramaniam2222/weatherbot.git
    cd weatherbot
    ```

2. **Create a `.env` file in the project root directory:**

    ```
    OPENWEATHER_API_KEY=your_actual_api_key_here
    ```

   Replace `your_actual_api_key_here` with your valid OpenWeatherMap API key.

3. **Ensure `.env` is listed in `.gitignore` to keep your key private.**

4. **Install required dependencies**  
   Make sure to install the Rasa SDK and related packages used by your custom actions.

    ```
    pip install -r requirements.txt
    ```

5. **Run the custom action server:**

    ```
    rasa run actions
    ```

6. **Run your Rasa bot and interact with it:**

    ```
    rasa shell
    ```

7. **Test input a query like:**

    ```
    What is the weather in Bangalore?
    ```

    The bot should respond with the weather description and temperature.

## Notes

- The API key is loaded at runtime from the environment variable `OPENWEATHER_API_KEY` for security.
- The `.env` file should **never** be committed to GitHub.
- You can extend this bot with additional features like forecasts, traffic updates, or multiple intents.

---

Feel free to ask if you want a sample `.gitignore` file or help with other parts of your project!
