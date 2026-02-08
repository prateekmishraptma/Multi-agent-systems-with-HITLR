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

