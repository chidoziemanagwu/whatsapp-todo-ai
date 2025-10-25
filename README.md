# WhatsApp AI To-Do List (n8n Workflow)

Automatically log WhatsApp messages to Google Sheets and receive a daily AI-generated, prioritized to-do list via WhatsApp — powered by **n8n**, **Groq (Llama 3.1)**, and **Google Sheets**.

## 🌟 Features
- Logs all incoming WhatsApp messages with timestamp, sender, and content
- Runs daily at 10 PM (configurable)
- Uses AI to extract and prioritize tasks:
  - 🔴 High priority
  - 🟡 Medium priority
  - 🟢 Low priority
- Creates Google Sheet automatically if missing

## 🛠️ Prerequisites
- [n8n](https://n8n.io/) instance (cloud or self-hosted)
- WhatsApp Business API account (via Meta or provider like Twilio)
- Google Cloud project with **Google Drive** and **Google Sheets** API enabled
- [Groq API key](https://console.groq.com/)

## 📥 How to Use
1. Import `workflow.json` into your n8n instance.
2. Create credentials in n8n for:
   - Google Sheets (OAuth2)
   - WhatsApp (API token)
   - Groq (API key)
3. Replace placeholder IDs in the workflow with your actual credential IDs.
4. Update the recipient phone number in the "Send To-Do" node.
5. Activate the workflow!

> 💡 See `docs/setup-guide.md` for detailed instructions (coming soon!).

## 🤝 Contributing
We welcome contributions! Check out the [Issues](https://github.com/chidoziemanagwu/whatsapp-todo-ai/issues) tab for ideas or open a new one.

## 📄 License
MIT © Chidozie Managwu
