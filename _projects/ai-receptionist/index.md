---
layout: post
title: AIVA — AI Voice Assistant for Enterprises
description: Voice-interactive AI receptionist built with Whisper, LangChain, and ElevenLabs to answer company questions in real-time.
skills:
  - Whisper (STT)
  - GPT-3.5 + LangChain
  - ElevenLabs (TTS)
  - Streamlit
  - Web Scraping
  - FAISS
main-image: /assests/images/avia/aiva_banner.png
---

# 🧠 AIVA — AI Voice Assistant for Enterprises

> AIVA (AI Voice Assistant) is a generative AI receptionist that listens, understands, and speaks — built during my internship at Systems Limited, Pakistan’s largest IT company.
<img src="/assets/images/avia/aiva_chat.png" alt="AIVA Interface Preview" width="650"/>

---

## 🚀 TL;DR  
**AIVA** is a voice-based receptionist trained on 100+ real company webpages. You ask a question out loud — it listens via Whisper, searches company info with LangChain + FAISS, and responds using ElevenLabs in a natural voice.

---

## 🧩 Problem / 💡 Solution

**Problem:** Static website chatbots are outdated, rigid, and text-only.  
**Solution:** A generative AI voice assistant that:
- Understands speech using OpenAI Whisper  
- Retrieves real-time answers from company content  
- Responds naturally via ElevenLabs TTS

---

## ✨ Key Features

- 🎙️ Voice-to-voice interaction (talk to AIVA, it talks back)
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

## 📺 Demo

🎥 [Watch the Recorded Demo](https://drive.google.com/file/d/1JInIiivD3RBrqDqMrg24oT3hcPp_cvXB/view)

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
