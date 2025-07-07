# 🦷 NoteBuddy – Engineering Case Study

NoteBuddy is a voice-to-note desktop application designed to streamline dental workflows by transcribing and formatting patient notes using Whisper and GPT. This case study documents the motivation, design process, technical architecture, and personal reflections behind the project.

---

## 🔍 Project Motivation

During my time working with a dental clinic, I observed how time-consuming and repetitive the note-taking process was for dentists after each patient visit. The process typically involved:

- Jotting down fragmented details during consultations
- Typing up structured notes into fields like "Diagnosis," "Procedure," and "Treatment Plan"
- Copying and pasting into clinical software like Dentrix

I realized this process was a perfect use case for generative AI — especially with new advancements in Whisper (speech-to-text) and GPT-3.5 (natural language processing). The idea was simple: eliminate repetitive manual entry and let AI handle note formatting.

---

## 🧠 Design Goals

I set out to build a desktop app that was:

- **Hands-off** during appointments (just hit “Record”)
- **Accurate** in transcribing medical dialogue
- **Consistent** in structuring outputs into defined dental fields
- **Lightweight** and easy to run on any Windows/Mac desktop

---

## 🛠️ Technologies Used

| Function                | Tools/Libraries                          |
|------------------------|------------------------------------------|
| Voice Capture          | `sounddevice`, `scipy.io.wavfile`        |
| Transcription          | OpenAI `Whisper`                         |
| AI Formatting          | OpenAI `GPT-3.5 Turbo` via `openai` API |
| UI                     | `tkinter`, `scrolledtext`                |
| Environment Handling   | `python-dotenv`                          |

---

## 🧩 Architecture Overview

### 1. Audio Capture  
- The app uses `sounddevice` to record `.wav` audio via a simple GUI.
- Files are saved locally as `recorded.wav`.

### 2. Transcription  
- Once recorded, the audio is passed into Whisper for STT (speech-to-text).
- The result is raw transcription of everything spoken during the session.

### 3. Formatting with GPT  
- I engineered a prompt that instructed GPT-3.5 to format transcriptions into predefined dental categories:
  - Patient Number
  - Chief Complaint
  - Tooth Surface
  - Diagnosis
  - X-ray
  - Treatment Plan
  - Procedure
  - Post-Op Instructions

### 4. Output Delivery  
- The output is shown in a scrollable text box.
- Clicking “Copy to Clipboard” saves the formatted note for easy pasting into EHR platforms.

---

## 💬 Sample Interaction

**Voice input:**  
_"Patient 304 came in complaining of pain in the upper right molar. On inspection, the tooth #16 showed signs of caries on the occlusal surface. We took an X-ray to confirm. Proceeded with a composite filling and gave post-op instructions regarding sensitivity."_

**Formatted output:**  
```
Patient Number: 304  
Chief Complaint: Pain in upper right molar  
Tooth Surface: Occlusal surface of Tooth #16  
Diagnosis: Caries  
X-ray: Taken to confirm decay  
Treatment Plan: Composite filling  
Procedure: Completed composite filling  
Post-Op: Informed patient about potential sensitivity
```

---

## 🧠 Prompt Engineering Challenges

- Ensuring GPT always outputs the same fields in the same order  
- Handling edge cases like missing fields (e.g., no X-ray taken)  
- Preventing hallucinations when GPT fills in information not present

I iterated several times on the prompt structure to enforce field consistency and maintain accuracy.

---

## 🎯 What Went Well

- Whisper handled low-quality audio surprisingly well.
- The UI stayed simple and intuitive throughout iterations.
- Real dentists who tested it found the tool intuitive and time-saving.

---

## 🤯 What Was Challenging

- Some microphones picked up background noise, confusing the transcription.  
- GPT formatting would sometimes fail if transcription was vague or lacked structure.  
- Whisper occasionally missed dental-specific terms, though improved with fine-tuning.

---

## 🔁 Future Improvements

- Integrate dental-specific vocabulary into Whisper fine-tuning  
- Add direct export to PDF or EHR systems  
- Mobile version with cloud sync  
- Add multi-language support for bilingual clinics

---

## 🙋‍♂️ My Role

This was a **solo project** — I handled:

- UX design  
- All Python code (GUI, audio recording, API integration)  
- Prompt tuning for GPT  
- Deployment-ready version for clinic testing

---

## 📦 Outcome

NoteBuddy was shared with several dentists in my network and tested in real scenarios. Feedback was overwhelmingly positive — especially for reducing end-of-day administrative load.

It became my first successful experiment in merging **AI with real-world professional workflows**.

---

> _NoteBuddy proves that even small tools can create massive time savings when designed with empathy and AI._ 🦷
