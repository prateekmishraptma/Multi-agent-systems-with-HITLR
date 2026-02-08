# 🧠 Multi-Agent Personal Assistant using LangChain

This repository contains a Jupyter Notebook implementation of a **Multi-Agent Personal Assistant** built using **LangChain**.  
The project demonstrates how a main agent can delegate tasks to multiple specialized sub-agents to answer complex user queries more effectively.

The implementation is based on the official LangChain documentation:  
🔗 https://docs.langchain.com/oss/python/langchain/multi-agent/subagents-personal-assistant

---

## 📌 Project Overview

Traditional single-agent LLM systems can struggle with complex, multi-step queries.  
This project solves that by using:

- **One main controller agent**
- **Multiple specialized sub-agents**
- **Tool-based task delegation**

Each sub-agent focuses on a specific responsibility (e.g., reasoning, retrieval, calculation), enabling better modularity, clarity, and scalability.

---

## 🧩 Architecture

### High-Level Flow

1. **User Query**
2. **Main Agent**
   - Understands the request
   - Decides which sub-agent(s) to use
3. **Sub-Agents**
   - Perform focused tasks using tools
4. **Final Response**
   - Aggregated and returned to the user

User → Main Agent → Sub-Agent(s) → Final Answer


---

## 🛠️ Technologies Used

- **Python**
- **LangChain**
- **OpenAI / LLM provider**
- **Jupyter Notebook**

---

## 📂 Repository Structure

├── notebook.ipynb # Main implementation notebook
├── README.md # Project documentation
└── requirements.txt # (Optional) Python dependencies


---

## ⚙️ Key Concepts Demonstrated

- **Multi-Agent Systems**
- **Agent Orchestration**
- **Sub-Agent Delegation**
- **Tool Calling**
- **LLM-Driven Reasoning**
- **Modular AI Design**

---

## 🚀 How It Works

### 1. Main Agent
- Acts as the **decision maker**
- Determines which sub-agent is best suited for a task

### 2. Sub-Agents
- Each sub-agent is created with:
  - A specific role
  - Access to relevant tools
- Examples:
  - Information retrieval agent
  - Reasoning agent
  - Task execution agent

### 3. Tool Usage
- Tools are wrapped using LangChain’s `@tool` decorator
- Agents call tools dynamically based on the query

---

## ▶️ How to Run

### 1. Install Dependencies

```bash
pip install langchain openai
(Add any additional packages used in the notebook)

2. Set Environment Variables
export OPENAI_API_KEY="your_api_key_here"
3. Open the Notebook
jupyter notebook
Run all cells step by step to see the multi-agent system in action.

📖 Reference
This implementation follows the official LangChain guide:

LangChain Multi-Agent Personal Assistant
https://docs.langchain.com/oss/python/langchain/multi-agent/subagents-personal-assistant

🌱 Future Enhancements
Add memory to sub-agents

Introduce role-based agent permissions

Integrate vector databases (FAISS / Chroma)

Add logging and tracing for agent decisions

Convert notebook into a production-ready Python service

🤝 Contributions
Contributions are welcome!
Feel free to fork the repository, improve the implementation, or add new sub-agents.

📜 License
This project is for educational and experimental purposes.
Please review LangChain and OpenAI licensing terms before production use.
