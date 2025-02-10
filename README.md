# 🤖 Home Assistant Chat Card Web Component

[中文版本](#中文版本)

## 🌟 Advanced AI Interaction Platform

`ha-chat-card` is a sophisticated, highly customizable AI chat interface for Home Assistant, designed to provide an intelligent, multilingual, and feature-rich conversational experience.

## 🚀 Version
**Current Version:** `2025.01.25`

## ✨ Key Features

### 1. Intelligent Conversation Engine
- **Deep Thinking Mode**:
  - Comprehensive AI thought process before responding
  - Natural, stream-of-consciousness reasoning
  - Multi-dimensional problem analysis
  - Transparent thought process visualization

### 2. Voice Interaction
- **Voice Recognition**:
  - Voice input by long-pressing send button
  - Cross-platform support (Android, iOS)
  - Browser compatibility (recommended Chrome)

- **Wake Word Activation**:
  - Custom wake word
  - Low-latency recognition
  - Microphone permission management
  - Wake-up sound customization

### 3. Multilingual Support
- Interface language configuration
- AI response language customization
- Currently supported languages:
  - Chinese (Simplified) `zh-cn`
  - (Extensible)

### 4. AI Agent Management
- Multiple AI agent priority configuration
- Intelligent switching keywords
- Support for up to 3 parallel AI agents
- Automatic fallback mechanism

### 5. Text-to-Speech (TTS)
- Multiple TTS engine modes
  - Off
  - Browser playback
  - Home Assistant service call
- Support for various TTS engines
- Selectable voice devices and roles

### 6. Interaction Experience Optimization
- **Typing Effect**
  - Simulate real-time AI thinking
  - More natural conversation experience
- Conversation history management
- Session ID persistence
- Cookie storage

### 7. Security & Performance
- Intelligent audio context unlocking
- Anti-conflict design
- Low resource consumption
- Browser compatibility

## 🔧 Configuration Example
```yaml
type: custom:ha-chat-card
agent_id: conversation.home_assistant
agents: 
  - conversation.home_assistant
voice_recognition: true
wake_word: 'hey assistant'
language: 'en'
response_language: 'en'
deep_think: true
tts_mode: 'service'
tts_engine: 'tts.google_translate'
