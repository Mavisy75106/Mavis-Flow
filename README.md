# Mavis-Flow: AI Email Intelligence

> Modern Gmail automation. Transform your overflowing inbox into a curated stream of intelligence.
> 現代化 Gmail 自動化系統。將擁擠的收件匣轉化為精確的情報流。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 🌐 Project Overview / 專案概述

**Mavis-Flow** is a lightweight automation tool built to solve inbox clutter. It leverages the underlying **OpenClaw** gateway of the host machine to access advanced language models, making it auth-agnostic and secure. 

**Mavis-Flow** 是一款為了解決收件匣混亂而開發的輕量化自動化工具集。它直接調用主機端底層的 **OpenClaw** 門戶來存取先進的語言模型，這使得它具備認證無關性（Auth-agnostic）且極其安全。

Whether the host uses API keys or OAuth, Mavis-Flow simply relays requests through the local gateway.
無論主機是使用 API Key 還是 OAuth 登入，Mavis-Flow 僅作為轉傳者，透過本地門戶處理模型請求，不涉及敏感金鑰存儲。

---

## ✨ Features / 功能亮點

- **🧠 Intelligent Summarization**: Concise, context-aware summaries of long threads.
- **🧠 智能摘要**：針對冗長的郵件串提供簡明且具備上下文意識的摘要。
- **🏷️ Semantic Classification**: Automatically labels emails based on intent (Action Required, etc.).
- **🏷️ 語義分類**：根據郵件意圖自動標記（如：需要行動、僅供參考等）。
- **🛡️ Noise Reduction**: Identifies and suppresses non-essential notifications.
- **🛡️ 雜訊過濾**：自動識別並抑制非必要的通知郵件。
- **🌐 Model Proxy**: OpenAI-compatible API relay for other OpenClaw instances.
- **🌐 模型代理**：提供 OpenAI 兼容的 API 接口，供其他 OpenClaw 實例或客戶端調用。

---

## 🚀 Getting Started / 快速上手

### Prerequisites / 前置需求
- Python 3.10+
- A running **OpenClaw Gateway** on the host machine. (主機需運行 OpenClaw Gateway)
- (Optional) Gmail API enabled Google Cloud Project. (選配：開啟 Gmail API 的 Google 專案)

### Setup / 安裝步驟

1. **Clone the repo / 複製專案:**
   ```bash
   git clone https://github.com/Mavisy75106/Mavis-Flow.git
   cd Mavis-Flow
   ```

2. **Install requirements / 安裝套件:**
   ```bash
   pip install -r requirements.txt
   pip install flask  # Required for proxy
   ```

### Running the Model Proxy / 執行模型代理

The proxy acts as a clean relay to your host's OpenClaw models.
代理伺服器將作為主機 OpenClaw 模型的純淨轉傳站。

```bash
python proxy/app.py
```
- **Endpoint**: `http://localhost:18790/v1`
- **Compatibility**: Any OpenAI-compatible client. (兼容任何 OpenAI 客户端)

---

## 📜 License / 授權

Distributed under the **MIT License**.

---
Built with ❤️ by [Mavis](https://github.com/Mavisy75106) 🌿
