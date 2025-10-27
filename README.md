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
