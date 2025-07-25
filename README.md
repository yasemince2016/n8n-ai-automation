# 🌤️ AI-Powered Weather Report Automation (n8n Workflow)

This project is a fully automated AI workflow built in [n8n](https://n8n.io), designed to generate and send personalized weather reports via email using OpenAI and real-time weather APIs.

## ✨ What It Does

- Listens for a trigger (chat input or webhook)
- Uses a **LangChain AI Agent** with memory and OpenAI GPT-4 to interpret the request
- Calls a real-time weather API (Open-Meteo) for Chicago
- Crafts a customized email using AI-generated subject and body
- Sends the weather report to a recipient via **Gmail integration**

## 🧠 AI Stack

- **OpenAI GPT-4.1** – for generating human-like email messages and summaries
- **LangChain Memory Buffer** – to retain contextual awareness
- **n8n AI Agent Node** – coordinates all tools using an LLM agent
- **Claude / GPT-Compatible Design** – the workflow could easily be modified to use Claude API

## 🔧 Tools Used

- `n8n` (self-hosted or cloud)
- `OpenAI API`
- `LangChain Agent Nodes`
- `Gmail OAuth2`
- `HTTP Request Tool` (for Open-Meteo API)

## 📬 Sample Use Case

Imagine a scenario where a user says:  
> *"Can I get tomorrow's weather forecast for Chicago?"*

This workflow will:
1. Trigger on message
2. Pull weather data
3. Let GPT-4 generate a friendly summary email
4. Send it directly to your inbox

## 📁 Files

- `weather_report_workflow.json` → the full n8n export file for the automation

## 🔄 How to Use

1. Import `weather_report_workflow.json` into your n8n instance
2. Set your environment variables and credentials:
   - OpenAI API key
   - Gmail OAuth2 credentials
3. Activate the workflow
4. Trigger it via chat or webhook

---

## 📌 Author

**Yasemin Çelik**  
Business Analyst & Product Owner passionate about AI automation, prompt engineering, and business process transformation.

