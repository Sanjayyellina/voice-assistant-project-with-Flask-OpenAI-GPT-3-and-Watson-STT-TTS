## AI Voice Assistant with OpenAI GPT-3 + IBM Watson STT/TTS
📌 Introduction
This project demonstrates how to build a full-stack AI-powered voice assistant that takes voice input, processes it using OpenAI GPT-3, and responds back with human-like speech using IBM Watson’s Speech-to-Text (STT) and Text-to-Speech (TTS) services.
The application is built with a Flask backend and a responsive frontend (HTML, CSS, JavaScript, Bootstrap). It showcases how to integrate multiple AI services into a seamless, production-ready solution.

---

## Features
 -*Speech-to-Text (STT) → Converts spoken input into text using IBM Watson STT.
 -*Conversational AI → Uses OpenAI GPT-3 to process user queries and generate intelligent responses.
 -*Text-to-Speech (TTS) → Converts GPT-3 responses back to audio using IBM Watson TTS.
 -*Web Interface → Clean, interactive frontend built with HTML, CSS, JS, and Bootstrap.
 -*Docker Support → Easily containerized and deployable anywhere.

 ---
 
## Tech Stack
Backend: Flask (Python)
AI Models: OpenAI GPT-3.5 (chat completions), IBM Watson Speech-to-Text & Text-to-Speech
Frontend: HTML, CSS, JavaScript, Bootstrap, JQuery
Deployment: Docker
Other Tools: Requests, Flask-CORS

---

##  Project Structure
chatapp-with-voice-and-openai-outline/
│── certs/                  # SSL certs for Watson
│── models/                 # IBM Watson STT & TTS configs
│── static/                 # JS and CSS files
│   ├── script.js
│   ├── style.css
│── templates/              # HTML frontend
│   ├── index.html
│── server.py               # Flask backend
│── worker.py               # Handles GPT + Watson logic
│── requirements.txt        # Python dependencies
│── Dockerfile              # Container setup
│── README.md               # Project documentation

---

## Setup Instructions
1️ Clone the Repository
git clone https://github.com/Sanjayyellina/voice-assistant-app.git
cd voice-assistant-app
2️ Create Virtual Environment
python3 -m venv my_env
source my_env/bin/activate
3️ Install Dependencies
pip install -r requirements.txt
4️ Run with Docker (Recommended)
docker build . -t voice-chatapp-powered-by-openai
docker run -p 8000:8000 voice-chatapp-powered-by-openai
5️ Run Locally (Flask)
python3 server.py
Navigate to:
 http://0.0.0.0:8000

 ---
 
## Example Use Case
Imagine a news agency that needs quick captioning of breaking news and interactive assistance for editors. This assistant can:
Transcribe journalist audio notes into text.
Summarize news content using GPT-3.
Convert approved headlines into audio for podcasts or radio.
<img width="1245" height="784" alt="Screenshot 2025-10-01 at 7 30 11 PM" src="https://github.com/user-attachments/assets/73a3aee8-2751-49fd-8b4c-40bd33efbdb1" />
<img width="1019" height="493" alt="Screenshot 2025-10-01 at 7 35 16 PM" src="https://github.com/user-attachments/assets/4e1f21c6-cfd7-412d-a421-725b616b1300" />


##  Future Enhancements
 Add authentication for secure API access.
 Multilingual speech-to-text and text-to-speech.
 Mobile-responsive interface.
 Deploy on AWS/GCP with CI/CD pipelines.

---

## Contributions
Pull requests and feature suggestions are welcome!
---

## License
This project is licensed under the MIT License.

---
