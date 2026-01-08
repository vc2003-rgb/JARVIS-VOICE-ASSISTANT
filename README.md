
 🎙️ JARVIS – AI Voice Assistant using Python

## 📌 Project Overview

*JARVIS* is a Python-based AI voice assistant inspired by Alexa and Google Assistant.
It listens for a wake word (“Jarvis”), accepts voice commands, and performs multiple real-time tasks such as opening websites, playing music, fetching news headlines, and answering general queries using OpenAI’s GPT model.

The project demonstrates practical implementation of *speech recognition, **text-to-speech, **API integration, and **AI-powered conversational logic*.

---

## 🚀 Features

* 🎧 Wake-word detection (“Jarvis”)
* 🌐 Open popular websites (Google, YouTube, Facebook, LinkedIn)
* 🎵 Play predefined songs via YouTube
* 📰 Fetch and read live news headlines (NewsAPI)
* 🤖 AI-based responses using OpenAI GPT
* 🔊 Voice output using Google Text-to-Speech (gTTS)
* 🧠 Modular code structure for easy scalability

---

## 🗂️ Project Structure


├── main.py                # Core logic of the voice assistant
├── musicLibrary.py        # Music dictionary with YouTube links
├── client.py              # Standalone OpenAI API test file
├── README.md              # Project documentation


---

## 🧩 File-wise Explanation

### 1️⃣ musicLibrary.py

This file contains a dictionary mapping *song names to YouTube URLs*.
It allows Jarvis to play songs using voice commands like:

> “Play stealth”

The assistant fetches the corresponding link and opens it in the browser. 

---

### 2️⃣ main.py

This is the *main execution file* of the project and includes:

#### 🔹 Speech Recognition

* Uses the speech_recognition library
* Continuously listens for the wake word *“Jarvis”*
* Converts spoken commands into text

#### 🔹 Text-to-Speech

* Uses *gTTS + pygame*
* Converts AI or system responses into natural-sounding speech

#### 🔹 Command Processing

Handles predefined commands such as:

* Opening websites
* Playing music
* Reading news
* Passing unknown queries to OpenAI

#### 🔹 News API Integration

* Fetches real-time Indian headlines using *NewsAPI*
* Reads headlines aloud

#### 🔹 OpenAI Integration

* Uses gpt-3.5-turbo
* Handles general questions conversationally

This file acts as the *brain of the assistant*. 

---

### 3️⃣ client.py

This is a *testing/demo script* for OpenAI integration.
It verifies:

* API connectivity
* Model response accuracy

Useful for debugging or learning how OpenAI API works independently. 

---

## 🛠️ Technologies Used

* *Python 3*
* *SpeechRecognition*
* *PyAudio*
* *pyttsx3*
* *gTTS*
* *pygame*
* *OpenAI API*
* *NewsAPI*
* *Webbrowser module*

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

bash
git clone https://github.com/your-username/jarvis-ai-assistant.git
cd jarvis-ai-assistant


### 2️⃣ Install Dependencies

bash
pip install speechrecognition pyttsx3 gtts pygame requests openai


> ⚠️ PyAudio installation may require platform-specific setup.

---

## 🔑 API Configuration

Replace the placeholders in main.py and client.py:

python
newsapi = "<Your NewsAPI Key>"
client = OpenAI(api_key="<Your OpenAI Key>")


---

## ▶️ How to Run

bash
python main.py


### Usage Flow:

1. Program starts → says *“Initializing Jarvis”*
2. Say *“Jarvis”*
3. Give a command like:

   * “Open Google”
   * “Play stealth”
   * “Tell me today’s news”
   * “What is machine learning?”

---

## 🧠 Sample Commands

| Command         | Action                    |
| --------------- | ------------------------- |
| Open Google     | Opens google.com          |
| Play march      | Plays song from YouTube   |
| News            | Reads live news headlines |
| What is coding? | AI-generated response     |

---

## 📈 Future Enhancements

* Add WhatsApp & email automation
* Integrate weather and calendar APIs
* Add GUI using Tkinter or PyQt
* Support multiple languages
* Improve NLP with intent classification

---

## 🎯 Learning Outcomes

* Hands-on experience with *AI APIs*
* Real-time *speech processing*
* API handling and error management
* Modular Python project design
* Practical AI assistant development

---

## 👤 Author

*Adithya Choudhary*
Final-year Computer Science student
Aspiring Data Analyst / AI Engineer
