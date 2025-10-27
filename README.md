# 🤖 n8n AI Chat Agent — Cohere + LangChain Workflow

## 🧠 Overview
This n8n workflow integrates **LangChain** and **Cohere’s Chat Model** to create an **AI-powered conversational agent** that can also perform **mathematical calculations** using a built-in calculator tool.

Whenever a chat message is received, the workflow triggers an AI Agent powered by Cohere’s LLM to generate intelligent responses — with logic support for reasoning-based tasks and calculations.

---

## ⚙️ Workflow Components

| Node | Type | Purpose |
|------|------|----------|
| 🟢 **When Chat Message Received** | `@n8n/n8n-nodes-langchain.chatTrigger` | Triggers the workflow when a new chat message is received |
| 🧩 **AI Agent** | `@n8n/n8n-nodes-langchain.agent` | Central LangChain Agent orchestrating responses |
| 💬 **Cohere Chat Model** | `@n8n/n8n-nodes-langchain.lmChatCohere` | Uses Cohere LLM API to generate natural language responses |
| ➕ **Calculator** | `@n8n/n8n-nodes-langchain.toolCalculator` | Performs arithmetic or logical computations within responses |

---

## 🪄 Workflow Logic

**Event Flow:**

1. **Trigger:**  
   A chat message is received via the `Chat Trigger` node.

2. **Processing:**  
   The message is passed to the **AI Agent**, which connects to:
   - **Cohere Chat Model** for intelligent text generation.
   - **Calculator Tool** for performing numeric computations.

3. **Response:**  
   The AI Agent produces a dynamic response — blending language understanding and calculation results.

---

## 🚀 Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/n8n-ai-agent-workflow.git
   cd n8n-ai-agent-workflow

## 📚 Learnings

- Building AI agents in **n8n** using **LangChain**  
- Integrating **Cohere’s Chat Model** for dynamic responses  
- Using tools (like **Calculator**) to extend LLM capabilities  
- Structuring **multi-node automation workflows**  

---

## 🧑‍💻 Author

**Aditi Khare**  
🌐 [Aditi @ AI Product Portfolio](https://aditikhare007.github.io/AI_Research_Junction_Aditi_Khare/)  
💌 [aditikhare007@gmail.com](mailto:aditikhare007@gmail.com)  
📦 [GitHub](https://github.com/aditikhare007)

---

## 🤝 Connect with Me

💼 [LinkedIn](https://www.linkedin.com/in/aditikhare007)  
🐦 [X / Twitter](https://twitter.com/AditiKhare007)  
🤗 [Hugging Face](https://huggingface.co/AditiKhare007)  
📚 [Packt Publications](https://www.packtpub.com/) – Contributor: *Generative AI Application Integration Patterns (2024)*  

---

⭐ *Part of Aditi’s AI Hands 0n Gen-AI & Agentic AI Product Portfolio*  
---

© 2025 **Aditi Khare**. All rights reserved.

