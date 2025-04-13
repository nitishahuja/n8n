# n8n - Workflow Automation for Everyone ⚙️

![n8n logo](https://n8n.io/images/n8n-logo.png)

n8n (pronounced "n-eight-n") is an open-source, extendable workflow automation tool that lets you connect services, APIs, and logic using a visual editor. It allows both developers and non-developers to automate repetitive tasks, create backend logic, and build intelligent agents — all without heavy lifting.

---

## 🚀 Features

- 🔌 600+ pre-built integrations (Google Sheets, Slack, OpenAI, PostgreSQL, etc.)
- 🧠 Built-in support for conditional logic, loops, and code blocks (JavaScript)
- 💬 Native support for AI tools like OpenAI and HuggingFace
- 🏠 Can be self-hosted or used via n8n cloud
- 📤 Trigger workflows with webhooks, cron jobs, events, or manual runs
- 📦 Reusable workflows with templates and custom nodes

---

## 🛠️ Getting Started

### 📦 Option 1: n8n Cloud

1. Go to [https://cloud.n8n.io](https://cloud.n8n.io)
2. Create an account (free trial available)
3. Use the visual editor to start building workflows

### 🐳 Option 2: Self-host via Docker

```bash
docker run -it --rm \
  -p 5678:5678 \
  -v ~/.n8n:/home/node/.n8n \
  n8nio/n8n
```

Then open `http://localhost:5678` in your browser.

---

## ✨ Example: AI Agent Chat (OpenAI + SerpAPI)

This workflow creates an AI agent that can hold a conversation using OpenAI’s LLMs and answer questions using SerpAPI.

> 📌 Requires n8n `v1.50.0` or above.

### 🔗 Import from Template

1. Visit: [AI Agent Chat Template](https://n8n.io/workflows/ai-agent-chat)
2. Click **"Use Workflow"** to add it to your workspace

### 🧩 Workflow Components

| Node                    | Description                                       |
| ----------------------- | ------------------------------------------------- |
| `Manual Trigger`        | Starts the workflow manually                      |
| `Memory Buffer (Read)`  | Retrieves conversation history                    |
| `OpenAI`                | Generates a response using LLM                    |
| `SerpAPI`               | Pulls live web data if needed (e.g., news, facts) |
| `Memory Buffer (Write)` | Stores the interaction for future context         |
| `Respond`               | Outputs the final answer                          |

---

## 🧠 Use Cases

- **Customer Support Chatbot**: Integrated with Slack or WhatsApp
- **Research Assistant**: Fetches data and answers questions on-the-fly
- **Compliance AI**: Reads uploaded documents and answers regulation-based questions
- **Internal Tools**: Connect OpenAI to Notion, Google Sheets, or Jira

---

## 📚 Resources

- [n8n Documentation](https://docs.n8n.io/)
- [n8n Templates Library](https://n8n.io/workflows)
- [n8n GitHub Repo](https://github.com/n8n-io/n8n)
- [Community Forum](https://community.n8n.io)

---

## 🧩 Contribute

n8n is open source and welcomes contributions!  
If you want to build your own custom integrations, check the [Creating Custom Nodes](https://docs.n8n.io/nodes/creating-nodes/) guide.

---

## 📝 License

n8n is licensed under [Fair-Code License (Sustainable Use License)](https://faircode.io/).  
Commercial usage may require a license — [see pricing](https://n8n.io/pricing) for more details.

---
