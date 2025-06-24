---
layout: post
title: AI Receptionist — Voice-Enabled Generative AI Assistant
description: A solo AI/ML project that acts as a voice-interactive AI receptionist using Whisper, LangChain, and ElevenLabs, trained on 100+ pages of company data.
skills:
  - Whisper
  - LangChain
  - FAISS
  - ElevenLabs
  - Streamlit
  - Web scraping
  - GPT-3.5
  - Python
main-image: /images/ai-receptionist-main.jpg
---

## 📺 Demo

🎥 [Watch the recorded demo](https://drive.google.com/file/d/1JInIiivD3RBrqDqMrg24oT3hcPp_cvXB/view)

---

## 🧠 Why I Built This

Receptionists are often the first point of contact for a business — but most chatbots today are limited to static FAQs and clunky interfaces.

**This project reimagines that role using cutting-edge generative AI:**
- It understands natural spoken language using Whisper (OpenAI)
- It’s trained on real company knowledge using LangChain and FAISS
- It speaks back fluently using ElevenLabs TTS
- It’s adaptable to any company, instantly becoming their voice

> This was my first-ever project in AI/ML, and I completed it solo in just 4 weeks — from idea to deployment-ready prototype.

---

## ✨ Key Features

✅ Voice-to-voice interaction (speak and get a spoken answer)  
✅ Trained on over **100+ pages of company data**  
✅ Real-time transcription + response using LLM  
✅ Web UI built in Streamlit  
✅ Modular and fully open-source

---

## 🧰 Tech Stack

| Component | Tool |
|----------|------|
| Speech to Text | [Whisper](https://github.com/openai/whisper) |
| Vector Store + Retrieval | FAISS + LangChain |
| Text to Speech | [ElevenLabs](https://www.elevenlabs.io/) |
| UI | Streamlit |
| Data Source | Web scraping from [Systems Limited](https://www.systemsltd.com/) |
| Language Model | OpenAI GPT-3.5 via LangChain |

---

## ⚙️ How It Works

1. **Web Scraping**
   - Scraped 100+ pages from the official Systems Limited website
   - Cleaned and concatenated the content into documents
   - Embedded using OpenAI + FAISS for vector search

2. **LangChain + LLM**
   - Integrated LangChain’s `ConversationalRetrievalChain` with GPT-3.5
   - Enabled multi-turn memory with session history

3. **Voice I/O**
   - **Input**: Uses `st_audiorec` + Whisper to transcribe user voice
   - **Output**: ElevenLabs generates natural speech in a custom voice

4. **Frontend**
   - Built a responsive UI in Streamlit with both text and voice options

---

## 💡 Use Cases

- AI-powered Receptionist for corporate websites  
- Onboarding assistant for new employees  
- Internal HR or IT Helpdesk Q&A bot  
- Custom voice bots for product support or marketing  

---

## 📁 Learn More

- [GitHub Repo](https://github.com/20mup/ai-receptionist)
- [Recorded Demo](https://drive.google.com/file/d/1JInIiivD3RBrqDqMrg24oT3hcPp_cvXB/view)
