# 🏗️ System Architecture  
**Bridging Language Barriers: Real-Time AI Translation for Video Conferencing**

---

## 🔹 Overview
The system captures live speech from video conferencing platforms, processes it through an AI pipeline, and provides real-time translation as captions or synthesized voice.  

---

## 🔹 Workflow

### 1. Capture  
- Audio is captured from Zoom, Google Meet, or Microsoft Teams.  

### 2. Processing Pipeline  
- **Speech-to-Text (STT):** Converts spoken language to text (e.g., Whisper, Vosk).  
- **Translation Engine:** Translates text into the target language(s) (e.g., MarianMT, M2M100, GPT-based).  
- **Formatting & Output:** Prepares captions or voice output for users.  

### 3. Output  
- Display translated **captions** in the UI.  
- Provide optional **text-to-speech (TTS)** in the translated language.  

---

## 🔹 ASCII Architecture Diagram


[ Audio Input ] → [ STT ] → [ Translation ] → [ Captions / TTS Output ]

## 🔹 System Flow (Mermaid Diagram)

```mermaid
graph TD
A[Microphone / Meeting Audio] --> B[Speech-to-Text (STT)]
B --> C[Translation Engine]
C --> D[Caption Display]
C --> E[TTS Output]

---


