# 🤖 Home Assistant Chat Card Web 组件

[[English Version](#[english-version](https://github.com/knoop7/ha-chat-Card/blob/hass/README.md))
](https://github.com/knoop7/ha-chat-Card/blob/hass/README.md)

## 🌟 概述
`ha-chat-card` 是一款强大且高度可定制的 AI 聊天界面，专为 Home Assistant 设计，提供智能、多语言、无缝的对话体验。

## 🚀 版本
**最新发布:** `2025.01.25`

## ✨ 主要功能

### 🔹 智能 AI 引擎
- **深度思考模式**：先进的推理能力，多维度问题分析，透明的思维过程可视化。
- **输入效果**：模拟实时 AI 思考，带来更自然的交互体验。

### 🎙️ 语音交互
- **语音识别**：支持在 Android 和 iOS 设备上长按发送按钮进行语音输入，并针对 Chrome 进行了优化。
- **唤醒词激活**：自定义唤醒词，低延迟识别，麦克风权限管理，支持个性化唤醒音效。

### 🌍 多语言支持
- 可配置界面语言和 AI 回复语言。
- 目前支持简体中文 (`zh-cn`)，并可扩展至更多语言。

### 🤖 AI 代理管理
- 可配置多 AI 代理的优先级。
- 支持最多 3 个并行 AI 代理，具备智能切换和自动回退机制。

### 🔊 语音合成 (TTS)
- 多种 TTS 引擎模式：关闭、本地浏览器播放、Home Assistant 服务调用。
- 可配置语音设备与语音引擎选择。

### 🔧 配置与安全
- **会话管理**：对话历史存储、会话 ID 持久化、Cookie 存储。
- **性能优化**：低资源消耗，智能音频上下文解锁，防冲突设计。

## 📌 配置示例
```yaml
type: custom:ha-chat-card
agent_id: conversation.home_assistant
agents: 
  - conversation.home_assistant
voice_recognition: true
wake_word: 'hey assistant'
language: 'zh-cn'
response_language: 'zh-cn'
deep_think: true
tts_mode: 'service'
tts_engine: 'tts.google_translate'
```

## 📦 安装指南

### 先决条件
- Home Assistant（2023.x 及以上版本）
- 现代浏览器，支持 ES 模块（Chrome、Firefox、Edge）
- 麦克风权限（可选）

### 安装步骤
1. 复制 `ha-chat-card.js` 文件到 Home Assistant 的 `www` 目录。
2. 在 `configuration.yaml` 文件中添加以下内容：

```yaml
frontend:
  extra_module_url:
    - /local/ha-chat-card.js
```

## ⚙️ 高级配置

### 唤醒词设置
- 请选择简单的 2-4 个单词短语。
- 避免使用复杂句子。
- 支持自定义唤醒音效。

### 语音合成 (TTS) 设置
- 选择合适的语音引擎。
- 配置媒体播放设备。
- 支持个性化语音选择。

## 🌐 兼容性
- **桌面浏览器**：Chrome、Firefox、Edge。
- **移动设备**：Android、iOS。
- **Home Assistant 版本**：2023.x 及以上。

## 🤝 贡献
欢迎大家提交 Issue 和 Pull Request，为项目贡献力量！

## 📜 许可证
[请指定您的许可证]

## 🔗 相关项目
- Home Assistant
- Web 组件

## 📞 支持
如遇问题或有建议，请在项目仓库提交 Issue 进行讨论。

