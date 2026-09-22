🤖 AI Fluency Training — Day 1

## Exploring LLMs, Workflows and AI Agents

**Roll Number:** 7376241CS218

---

## 📖 Project Overview

This repository contains my Day 1 AI Fluency Training implementation.

The lab focuses on understanding how applications can progress from a simple language-model chatbot to an AI agent that can interact with custom tools.

Three implementations were developed during the lab:

- Direct LLM Chatbot
- Rule-Based Workflow
- Tool-Calling AI Agent

---

## 🔍 Learning Flow

The project follows this progression:

```text
Basic LLM
    ↓
Programmed Workflow
    ↓
LLM + Tools
    ↓
AI Agent

Each stage provides a different way of solving the same type of course-related problems.

💬 LLM Chatbot

The chatbot sends the user's question directly to the language model and displays the generated response.

User
 ↓
Question
 ↓
LLM
 ↓
Answer

This approach is flexible for natural-language questions, but the model does not automatically have access to the application's private course-fee information.

⚙️ Rule-Based System

The workflow implementation uses predefined Python logic.

It identifies course codes from the input and retrieves their corresponding fees from the stored course data.

Input Question
      ↓
Course Code Detection
      ↓
Fee Lookup
      ↓
Rule Processing
      ↓
Output

This approach produces predictable results for the cases covered by the programmed rules.

🧰 AI Agent

The agent combines the language model with custom functions.

Two tools are available:

Course Fee Lookup
get_course_fee()

Retrieves the fee of a course.

Calculator
calculator()

Evaluates arithmetic expressions.

The agent can decide when these tools are required and use their results while generating the final response.

💰 Course Information
Course Code	Fee
CS101	Rs. 12,000
AI202	Rs. 18,000
DS303	Rs. 15,000
🧪 Questions Tested

The implementations were tested using questions involving:

Individual course fee lookup
Multiple course fee calculation
Scholarship calculation
Comparison of course fees
General text generation
Budget-based course selection
🎯 Budget Challenge

The final challenge uses a budget of Rs. 30,000.

The system needs to determine which two available courses can be selected together without exceeding the given amount.

The agent can use the course lookup and calculator tools to work with the available course information.

📁 Repository Contents
AI-Fluency-Training-Day1/
│
├── .gitignore
├── requirements.txt
├── config.py
├── check_setup.py
├── chatbot.py
├── workflow.py
├── tools.py
├── agent.py
└── challenge.py
▶️ Execution

Activate the virtual environment:

.\.venv\Scripts\Activate.ps1

Verify the setup:

python check_setup.py

Run the individual components:

python chatbot.py
python workflow.py
python tools.py
python agent.py
python challenge.py
🔐 API Configuration

The project uses Groq for LLM access.

PROVIDER=groq
GROQ_API_KEY=your_api_key_here
MODEL=openai/gpt-oss-20b

The actual API key is kept locally and is not included in the repository.

💡 Key Takeaway

The lab demonstrates that an LLM can be combined with normal programming logic and external functions.

A chatbot mainly generates responses, a workflow follows predefined instructions, while an agent can determine which tool is useful for completing a task.

👨‍💻 Student Details

Roll Number: 7376241CS218
Training: AI Fluency Training
Day: 1
Focus: LLMs, Workflows and AI Agents
