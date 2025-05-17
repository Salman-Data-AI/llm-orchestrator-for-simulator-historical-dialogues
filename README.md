# Cross-Provider LLM Orchestrator for Simulated Historical Dialogues

![image](https://github.com/user-attachments/assets/e838bab0-8a2f-44f6-bbd5-6098846bb702)

A compact Python showcase that **orchestrates three vendor models**—  
*GPT-4o-mini (OpenAI), Claude-3 Haiku (Anthropic) and Gemini 1.5 Flash (Google)*—in a round-robin conversation.  
Each model is “hard-locked” to a famous conqueror (Genghis Khan, Alexander the Great, Akbar the Great) using tagged persona prompts, stop-tokens and role-aware message routing.

---

## ✨  Features
| Capability | ✔ |
|----|------------|
| Cross-provider orchestration with a single Python script | ✔︎
| Persona locking: mandatory prefix + `<END>` stop sequence prevents voice-bleed | ✔︎
| Provider-specific message shaping (OpenAI/Anthropic/Gemini constraints handled) | ✔︎
| Clear, colour-coded console output for each legend | ✔︎
| Easily extensible to additional models or personas | ✔︎

---

## The Process

Wrote the code in Jupyter Lab.
Each persona was locked into an LLM.
- ChatGPT: Genghis Khan
- Anthropic: Alexander, the Great
- Gemini: Akbar, the Great

The prompt was that they were all resurrected in the year 2025.
They were made to talk to each other about their legacies in the contemporary world. 

---

## 📦 Requirements
* Python 3.9+  
* `openai`, `anthropic`, `google-generativeai`, `python-dotenv`

```bash
pip install openai anthropic google-generativeai python-dotenv
