# ai-mock-interview-coach
AI Mock Interview Coach using n8n and local LLM (Ollama)

# AI Mock Interview Coach

AI Mock Interview Coach is an AI-driven system designed to simulate real interview scenarios and help candidates improve their interview performance through structured questioning and professional feedback.

The system behaves like a real interviewer by asking role-based questions, evaluating responses, assigning a score, and providing constructive suggestions for improvement.

## Key Features
- Mock interview–style conversational flow
- Role-based interview questions
- Professional answer evaluation
- Scoring system (out of 10)
- Constructive feedback with improvement tips
- Lightweight and optimized prompt design for local execution

## Technology Stack
- n8n (Workflow Automation)
- Ollama (Local Large Language Model)
- Open-source LLM (phi3 / llama3)
- Node.js

## Workflow Overview
1. User starts the conversation with a greeting
2. AI asks for role and experience
3. AI conducts a mock interview like a real interviewer
4. User answers the interview question
5. AI evaluates the response and provides feedback

## Setup Instructions

### 1. Install Node.js
Download and install Node.js from the official website.

### 2. Install n8n globally
npm install -g n8n

### 3. Install Ollama and pull a model
ollama pull phi3

### 4. Start Ollama
ollama serve

### 5. Start n8n
n8n

### 6. Open n8n in a browser
http://localhost:5678

### 7. Import the workflow
Import the `workflow.json` file into n8n to load the AI Mock Interview workflow.

## Project Flow
Chat Trigger → AI Agent → Local LLM (Ollama) → Response

The AI Agent controls the interview logic, evaluation, and feedback generation.  
The system runs locally to avoid dependency on paid cloud APIs.

## Notes
- This project is executed locally using a lightweight LLM.
- Designed with a voice-ready architecture (speech-to-text and text-to-speech can be integrated as future enhancements).
- Focuses on AI agent behavior, workflow orchestration, and interview simulation.
