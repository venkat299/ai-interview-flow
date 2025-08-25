# Interview Flow

## 1. Project Objective

The goal of this project is to develop an AI-powered technical screening platform that automates initial interviews. The system provides a dynamic, chat-based experience for candidates, asking intelligent, context-aware follow-up questions based on the job description and the candidate's live answers. 

## 2. Technical Approach

* Language & Framework**: The entire backend is built with **Python** and **FastAPI**
* **AI Engine**: The core intelligence is provided by an **`AI Orchestration Service`** that uses a large language model (LLM) to generate questions on the fly. It engineers prompts based on the job description and conversation history to ensure questions are relevant and insightful.
* **Real-Time Interaction**: An **`Interview Session Service`** manages the candidate experience. It uses **WebSockets** to create a real-time, low-latency chat interface.




## 3. Test Frontend & End-to-End Testing

Once the backend services are running, you can drive a sample interview using the lightweight test frontend located in `test_frontend/`.

1. Start the services if they are not already running:

   ```bash
   docker-compose up --build
   ```

2. In a new terminal, serve the static files:

   ```bash
   python -m http.server --directory test_frontend 3000
   ```
