# No\<think\> Conversation

**Why this exists:**
- Modern LLMs like Qwen3 are 'hybrid reasoning models' — they can either think (for a better response) or not think (for faster replies).
- For a voice assistant in Home Assistant, these models are great, but the thinking step can be too slow ⏳
- By adding `/no_think` to your prompt, you skip the thinking phase, however the response still contains `<think></think>` tags

This integration filters out those tags for a cleaner, more seamless experience. Just remember to add `/no_think` to your prompt! 💬

**How to Use:**
- Works with any OpenAI compatible API (e.g. GPT, Gemini, Groq, Ollama, Open WebUI, etc)
- Identical to the standard OpenAI integration, but with support for custom URLs and automatic `<think></think>` tag filtering

**Installation:**

1. Add the repository to HACS  
[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=duckida&repository=ha-nothink-llm&category=Integration)

2. Install the integration 📥  
3. Restart Home Assistant 🔄  
4. Search for the integration and set it up with your API Key and Base URL  
5. To disable thinking, add `/no_think` to your System Prompt

🔧 Programmed by [Jules](https://jules.google) based off the lovely [openai_custom_conversation](https://github.com/michelle-avery/openai-compatible-conversation)
