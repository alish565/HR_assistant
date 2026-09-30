### Interactive HR Assistant Agent

# 💬 AI-Powered HR Assistant Agent

An interactive HR Assistant chatbot built with **LangChain**, **OpenAI GPT-4 Turbo**, and **Gradio**. The agent uses custom tool calling to query employee records, check leave balances, and search Wikipedia to assist with recruitment and interview preparation.

---

## 📌 Features

* **Custom Tool Integration**:
  * `get_employee_details`: Looks up employee names, roles, and departments by ID.
  * `check_leave_balance`: Retrieves remaining annual and sick leave balances.
  * `WikipediaQueryRun`: Searches Wikipedia to generate job-specific interview questions or provide industry context.
* **Conversational Memory**: Retains discussion context across multi-turn chats using `ConversationBufferMemory`.
* **Domain Guardrails**: Configured to restrict answers exclusively to HR topics and the tech industry.
* **Gradio Web Interface**: Provides an interactive chat window for effortless testing.

---

## 🚀 Getting Started

### Prerequisites

* Python 3.9+
* OpenAI API key

### Installation


pip install langchain langchain-openai langchain-community gradio python-dotenv wikipedia
Environment Setup
Create a .env file in your project root:

Code snippet
OPENAI_API_KEY=your_openai_api_key_here
Usage
Run the script to launch the chatbot interface:

Bash
python hr_assistant.py
Open the local Gradio link (e.g., http://127.0.0.1:7860) in your browser to start chatting.

💡 Example Queries
"What is the position and department of employee E001?"

"How many annual leave days does E002 have left?"

"Can you generate a few interview questions for a UX Designer?"

🛠️ Tech Stack
Framework: LangChain (Agent & Tools)

LLM: OpenAI gpt-4-turbo

User Interface: Gradio

Memory: LangChain ConversationBufferMemory
