
# No\<think\> Conversation

> Modern LLMs like Qwen and DeepSeek support thinking modes. However, these slowdown response times in Home Assistant. By adding `/no_think` to your prompt, you disable thinking mode, however the response still contains `<think></think>` tags before the response.

This integration filters out those tags for a more seamless experience. Don't forget to add `/no_think` to your prompt!

- Works with any OpenAI compatible API (eg Fireworks, Groq etc)
- May have bugs - programmed by [Jules](https://jules.google) based of openai_custom_conversation
