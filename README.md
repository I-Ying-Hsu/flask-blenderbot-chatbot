# AI Chatbot Web Integration - IBM Guided Project

This project is a practical application developed as part of a guided course by **IBM**. It demonstrates how to transform a terminal-based chatbot into a fully functional web application by integrating a Large Language Model (LLM) with a Flask backend.

## 🚀 Project Overview
The goal of this project was to build a "ChatGPT-like" website. It consists of two main components:
1.  **Back-end Server**: A Flask application that hosts the chatbot model and processes requests.
2.  **Front-end Webpage**: A user interface that communicates with the server to display the conversation.

## 🧠 Learning Objectives
Through this IBM lab, I achieved the following:
* **Server Setup**: Configured a backend server using the **Flask** Python framework.
* **LLM Integration**: Integrated the `facebook/blenderbot-400M-distill` model using the **Hugging Face Transformers** library.
* **API Development**: Created a POST request route (`/chatbot`) to handle incoming JSON prompts.
* **Context Management**: Implemented a system to track and send `conversation_history` to the model so it can maintain context.
* **CORS Handling**: Learned to mitigate Cross-Origin Resource Sharing (CORS) errors to allow the frontend to talk to the backend.

## 🛠️ Technical Stack
* **Language**: Python 3.11
* **Backend**: Flask, Flask-CORS
* **AI Model**: Blenderbot 400M (Transformers library)
* **Frontend**: HTML, JavaScript (Fetch API)

---

## 📖 How to Run This Project

### 1. Install Prerequisites
You will need Python 3.11 installed. Install the necessary libraries using the following commands:
```bash
python3.11 -m pip install flask flask_cors transformers torch
```

### 2. Prepare the Project Structure
Ensure your files are organized so Flask can find the HTML templates and static assets correctly:
* app.py (The main Python server)
* templates/index.html (The web interface)
* tatic/script.js (The logic for sending messages)

### 3. Connect the Frontend to the Backend
Before running the app, you must update the API endpoint in the JavaScript file:
1. Open static/script.js.
2. Locate the url variable.
3. Set it to your backend address: http://127.0.0.1:5000/chatbot.

### 4. Launch the Application
Navigate to your project directory in the terminal and run the server using the Flask command:
```bash
flask run
```

### 5. Interact with the Chatbot
Open your web browser and navigate to http://127.0.0.1:5000/. You can now type a message in the chat box and receive a response directly from the model!

---
## 🎓 Acknowledgments
This exercise was completed as part of an IBM Generative AI Engineering.
