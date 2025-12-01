# 🤖 LLM Chatbot Template

A template for building AI-powered chatbots using Claude API integrated with Google Apps Script.

## 🎯 Overview

This template provides the foundation for creating LLM-powered chatbots for customer service, data processing, and business automation.

## ✨ Features

- **Claude API Integration:** Connect to Anthropic's Claude
- **Conversation Memory:** Maintain context across messages
- **Prompt Engineering:** Optimized system prompts for business use
- **Error Handling:** Graceful fallbacks and logging
- **Rate Limiting:** Built-in request throttling

## 🛠️ Tech Stack

- Google Apps Script
- Claude API (Anthropic)
- JavaScript
- Google Sheets (conversation logging)

## 📋 Template Structure
├── Code.gs           # Main chatbot logic
├── API.gs            # Claude API wrapper
├── Prompts.gs        # System prompts
├── Logger.gs         # Conversation logging
└── Config.gs         # Configuration settings

## 💡 Example Usage
```javascript
// Initialize chatbot
const chatbot = new LLMChatbot({
  apiKey: CLAUDE_API_KEY,
  model: 'claude-3-sonnet',
  systemPrompt: BUSINESS_PROMPT
});

// Process user message
function handleUserMessage(userInput) {
  const response = chatbot.chat(userInput);
  logConversation(userInput, response);
  return response;
}
```

## 🔧 Configuration
```javascript
const CONFIG = {
  model: 'claude-3-sonnet-20240229',
  maxTokens: 1024,
  temperature: 0.7,
  systemPrompt: `You are a helpful assistant for...`
};
```

## 📊 Applications Built

| Use Case | Description |
|----------|-------------|
| Customer Service | 24/7 automated responses |
| Data Enrichment | AI-powered data completion |
| Document Processing | Extract info from text |
| FAQ Bot | Automated question answering |

## 📫 Contact

**Trey Haulbrook**
- Email: Haulbrookai@gmail.com

---

*Template based on production chatbot implementations.*
