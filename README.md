# 🤖 Home Assistant Chat Card Web Component

[中文版本](https://github.com/knoop7/ha-chat-Card/blob/hass/ZH_README.md)

## 🌟 Overview
`ha-chat-card` is a powerful and highly customizable AI chat interface for Home Assistant, providing an intelligent, multilingual, and seamless conversational experience.

## 🚀 Version
**Latest Release:** `2025.01.25`

## ✨ Features

### 🔹 Intelligent AI Engine
- **Deep Thinking Mode**: Advanced reasoning, multi-dimensional problem analysis, and transparent thought process visualization.
- **Typing Effect**: Simulates real-time AI thinking for a more natural interaction.

### 🎙️ Voice Interaction
- **Voice Recognition**: Supports voice input via long-press send button on Android and iOS, optimized for Chrome.
- **Wake Word Activation**: Customizable wake words, low-latency recognition, microphone permission handling, and wake-up sound customization.

### 🌍 Multilingual Support
- Configurable interface and response languages.
- Supports Chinese (Simplified) `zh-cn` with extensibility for additional languages.

### 🤖 AI Agent Management
- Configurable multi-agent priority settings.
- Supports up to three parallel AI agents with intelligent switching and automatic fallback mechanisms.

### 🔊 Text-to-Speech (TTS)
- Multiple TTS engine modes: Off, browser playback, Home Assistant service call.
- Configurable voice devices and engine selection.

### 🔧 Configuration & Security
- **Session Management**: Conversation history storage, session ID persistence, and cookie storage.
- **Performance Optimization**: Low resource consumption, intelligent audio context unlocking, and an anti-conflict design.

## 📌 Configuration Example
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
```

## 📦 Installation Guide

### Prerequisites
- Home Assistant (2023.x or later)
- Modern browser supporting ES modules (Chrome, Firefox, Edge)
- Microphone permissions (optional)

### Installation Steps
1. Copy `ha-chat-card.js` to Home Assistant's `www` directory.
2. Add the following to `configuration.yaml`:

```yaml
frontend:
  extra_module_url:
    - /local/ha-chat-card.js
```

## ⚙️ Advanced Configuration

### Wake Word Settings
- Use simple 2-4 word phrases.
- Avoid complex sentences.
- Supports custom wake-up sounds.

### TTS Service Configuration
- Select an appropriate voice engine.
- Configure media playback devices.
- Supports personalized voice selection.
- If Android users cannot run voice recognition, please manually download it from the official website  https://play.google.com/store/apps/details?id=com.google.android.tts
- 
## 🌐 Compatibility
- **Desktop Browsers:** Chrome, Firefox, Edge.
- **Mobile Devices:** Android, iOS.
- **Home Assistant:** 2023.x and above.

## 🤝 Contributing
We welcome contributions! Feel free to submit issues and pull requests to improve this project.


## 🔗 Related Projects
- Home Assistant
- Web Components

## 📞 Support
For issues and discussions, please submit an issue in the project repository.

