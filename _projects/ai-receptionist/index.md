---
layout: post
title: AIVA — AI Voice Assistant for Enterprises
description: Meet AIVA — an intelligent AI receptionist that listens, understands, and responds like a real human. Built during my internship at Systems Limited, Pakistan’s largest IT firm.
skills:
  - Whisper (STT)
  - GPT-3.5 + LangChain
  - ElevenLabs (TTS)
  - Streamlit
  - Web Scraping
  - FAISS
main-image: /images/aiva_banner_fixed.png
---

# 🧠 AIVA — AI Voice Assistant for Enterprises

> Imagine walking into an office and being greeted by an AI that listens, thinks, and speaks like a real receptionist. That’s AIVA.

<img src="/assets/images/aiva/aiva_chat.png" alt="AIVA Interface Preview" width="650"/>

---

## 🚀 TL;DR  
**AIVA** is a voice-based receptionist trained on 100+ internal company webpages. Just ask a question — it listens via Whisper, finds the answer with LangChain + FAISS, and replies using ElevenLabs in natural, human-like speech.

---

## 🧩 Problem / 💡 Solution

**Problem:** Static website chatbots are outdated, rigid, and text-only.  
**Solution:** A generative AI voice assistant that:
- Understands speech using OpenAI Whisper  
- Retrieves real-time answers from company content  
- Responds naturally via ElevenLabs TTS

---

## ✨ Key Features

- 🎙️ Voice-to-voice interaction (Talk to AIVA, it talks back)
- 🔍 Knowledge retrieval from 100+ scraped webpages
- 🧠 GPT-3.5 via LangChain with memory for follow-up context
- 💬 Web interface with both voice and text input (Streamlit)
- 🧩 Modular pipeline, adaptable to any company with a website

---

## 💻 Tech Stack & Tools

![Whisper](https://img.shields.io/badge/Whisper-OpenAI-blue?style=flat)
![GPT-3.5](https://img.shields.io/badge/GPT--3.5-LangChain-brightgreen?style=flat)
![ElevenLabs](https://img.shields.io/badge/ElevenLabs-TTS-orange?style=flat)
![FAISS](https://img.shields.io/badge/FAISS-VectorSearch-purple?style=flat)
![Streamlit](https://img.shields.io/badge/Streamlit-UI-red?style=flat)
![Python](https://img.shields.io/badge/Python-3.11-blue?style=flat)

---

## 🎥 Demo

{% include youtube-video.html id="_fyLJ0vlOlo" autoplay="false" %}

---

## 🧠 How It Works

1. **Voice Input Capture**  
   - Uses Whisper to convert user speech into text within a Streamlit interface.

2. **Query Processing**  
   - A LangChain-powered chatbot parses the input, then searches a FAISS vector database built from web-scraped business content.

3. **Response Generation**  
   - The LLM returns a helpful, conversational response formatted as a receptionist reply.

4. **Voice Output**  
   - ElevenLabs reads the response aloud using natural, expressive AI-generated speech.

---

## 🧠 Lessons Learned

- Seamless voice interaction is possible with the right audio tools (Whisper + ElevenLabs).
- LangChain’s modular chains make it easy to build multi-step retrieval pipelines.
- Designing for real-world use cases like onboarding or helpdesk requires domain-specific tuning of prompts and chunking strategies.

---

## 📖 Learn More

- [🔗 GitHub Repository](https://github.com/20mup/ai-receptionist)
- [📄 Full Engineering Case Study](/docs/aiva-case-study.md)

---

> _From static FAQs to conversational AI — meet the future of enterprise assistants._ 🤖
