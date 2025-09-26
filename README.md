# 🌐 AutoAccess — Next-Gen Web Accessibility Chrome Extension  

> *One Click. Infinite Accessibility.*  
> AutoAccess makes any website instantly accessible for 1.3 billion differently-abled people worldwide — with AI-powered assistance, voice interaction, and inclusive design tools.  

---

## 🚀 Overview  

AutoAccess is a *Chrome Extension (Manifest V3)* that transforms any website into an *inclusive and accessible experience*.  
With features like *AI Chat Assistant, OCR-based Image Labeling, Text-to-Speech, Voice Commands, Smart Contrast Fixes, Global Accessibility Mode, and Enhanced Keyboard Navigation, AutoAccess ensures **barrier-free browsing* for everyone.  

---

## ✨ Core Features  

### 1. 🌍 One-Click Global Accessibility Mode  
- Runs a full *axe-core accessibility audit*.  
- Automatically applies *safe fixes*:  
  - Missing alt text placeholders  
  - ARIA labels for forms & buttons  
  - Heading hierarchy correction  
  - Smart contrast adjustments  
  - Skip links for keyboard navigation  
- Provides a *Before/After visual diff*.  
- Generates a *downloadable accessibility report* (PDF + JSON).  

---

### 2. 🤖 AI Chat Assistant  
- Context-aware chatbot integrated in every webpage.  
- Use-cases:  
  - “Summarize this article”  
  - “Describe this image”  
  - “Why is this button inaccessible?”  
- Responds with *confidence levels + provenance (local/OpenAI/HF)*.  
- Optional *Text-to-Speech playback*.  

---

### 3. 🖼 AI Image Labeling + OCR  
- Detects images without alt text.  
- Uses *Tesseract.js OCR* (local) or *OpenAI/HuggingFace* (cloud, optional) for captioning.  
- Provides AI-generated description → User can *edit & apply*.  
- Updates DOM with accessible alt attributes.  

---

### 4. 🔊 Text-to-Speech (TTS)  
- Reads aloud any text on webpage.  
- Word-by-word *highlight sync* for dyslexic/blind users.  
- Multiple voice options (Browser TTS + optional premium voices).  
- Shortcut: Alt+R (start/pause reading).  

---

### 5. 🎤 Speech-to-Text (STT) / Voice Commands  
- Voice-powered browsing & navigation.  
- Supported commands:  
  - *Navigation:* “Scroll down”, “Next link”, “Go back”  
  - *Interaction:* “Click buy now”, “Add to cart”  
  - *Reading:* “Read this page”  
- Implemented with *Web Speech API* (local).  

---

### 6. 🎨 Smart Contrast Fixer  
- Improves text readability with *WCAG 2.1 AA compliant colors*.  
- Includes *color-blind presets*: Protanopia, Deuteranopia, Tritanopia.  
- Preserves brand colors while ensuring accessibility.  

---

### 7. ⌨ Enhanced Keyboard Navigation  
- Logical tab order for all focusable elements.  
- Injects skip links for main content.  
- Adds *visual focus indicators*.  
- SPA (single-page-app) route change support with MutationObserver.  

---

## 🏗 Tech Stack  

### 🔹 Core Technologies  
- *React 18* — UI framework for modular components.  
- *TypeScript* — Strong typing for scalable codebase.  
- *Tailwind CSS* — Utility-first responsive styling.  
- *Chrome Extension Manifest V3* — Secure extension architecture.  

### 🔹 Accessibility & Auditing  
- *axe-core* — Industry-standard accessibility audit engine.  
- *html2canvas* — For Before/After visual diff.  
- *jsPDF* — For generating downloadable PDF reports.  

### 🔹 AI & OCR  
- *Tesseract.js* — Local OCR engine for extracting text from images.  
- *OpenAI GPT-4 (optional)* — Image captions, chatbot, TTS/STT (requires API key).  
- *HuggingFace Inference API (optional)* — Open-source AI models for captions/summaries.  

### 🔹 Voice & Speech  
- *Web Speech API* — Speech-to-Text (STT).  
- *SpeechSynthesis API* — Text-to-Speech (TTS).  
- *ElevenLabs / OpenAI TTS (optional)* — Premium voices.  

### 🔹 Security  
- *CSP (Content Security Policy)* — Prevents script injection attacks.  
- *Web Crypto API (AES-GCM)* — Encrypts API keys & sensitive settings.  
- *chrome.storage.local* — Secure storage for profiles and reports.  

---

## 🔒 Privacy & Security  

- *Local-first architecture* — all features work locally.  
- *Cloud AI (optional)* — enabled only with user consent + API keys.  
- *API keys encrypted* with AES-GCM before storage.  
- *No personal data collection* — extension never tracks URLs or page content.  



