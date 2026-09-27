# WhatsApp AI Automation Bot (n8n)

An AI-powered WhatsApp automation bot built with n8n. This workflow acts as a smart customer service agent that can answer questions, check calendar availability, and book appointments directly through WhatsApp.

## 🚀 Features
*   **WhatsApp Integration:** Triggers on incoming WhatsApp messages.
*   **AI Agent (Google Gemini):** Uses a LangChain AI Agent powered by Google Gemini to understand user intent and generate human-like responses.
*   **Conversational Memory:** Uses Postgres to store chat history, allowing the bot to remember context across multiple messages.
*   **Google Calendar Integration:** (Optional/Disabled) The agent has tools to check availability and create calendar events.
*   **Automated Replies:** Sends the AI-generated response back to the user seamlessly.

## 🛠️ Tech Stack
*   **n8n:** Workflow automation platform.
*   **Google Gemini (PaLM):** Large Language Model for AI reasoning.
*   **PostgreSQL:** Database for storing chat memory.
*   **WhatsApp Business API:** Messaging interface.
*   **Google Calendar API:** Scheduling tool.

## 📋 How it Works
1.  **Trigger:** A user sends a message to the WhatsApp Business number.
2.  **Filter:** An `If` node checks if the message is a valid text message.
3.  **AI Processing:** The AI Agent receives the text. It uses the **Postgres Chat Memory** to recall previous messages and the **Google Gemini Chat Model** to generate a reply.
4.  **Action:** The AI Agent can optionally call the Google Calendar tools to book appointments.
5.  **Response:** The final output is sent back to the user via the WhatsApp node.

## 📸 Screenshots
*(Insert the screenshots you showed me here)*
*   **Workflow Canvas:** Shows the n8n node architecture.
*   **WhatsApp Chat:** Shows the bot successfully answering a user's query.

## ⚙️ Setup Instructions
1.  Import the `whatsapp-ai-agent-workflow.json` file into your n8n instance.
2.  Configure your credentials for:
    *   WhatsApp Trigger & Send
    *   Google Gemini API
    *   PostgreSQL
    *   Google Calendar (if using the tools)
3.  Activate the workflow.

## 🤝 Contact
**G Sinduja** - [Your LinkedIn Link]
