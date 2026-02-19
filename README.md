# Mavis-Flow: AI Email Intelligence

> Modern Gmail automation. Transform your overflowing inbox into a curated stream of intelligence.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## Project Overview

**Mavis-Flow** is a lightweight automation tool I built to solve a personal pain point: a cluttered inbox. By leveraging advanced language models, it goes beyond simple rule-based filtering to understand the context and priority of your communications.

Stop managing your inbox; start focusing on your flow.

## Features

- **🧠 Intelligent Summarization**: Concise, context-aware summaries of long threads.
- **🏷️ Semantic Classification**: Automatically labels emails based on intent (Action Required, Informational, etc.).
- **🛡️ Noise Reduction**: Identifies and suppresses non-essential notifications.
- **🌐 Model Proxy**: Allows other OpenClaw instances (or any OpenAI-compatible client) to use your configured models via an OpenAI-compatible API.

## Getting Started

### Prerequisites

- Python 3.10+
- A Google Cloud Project with Gmail API enabled.
- A Gemini API Key (get it from Google AI Studio).

### Quick Start

1. **Clone the repo:**
   ```bash
   git clone https://github.com/Mavisy75106/Mavis-Flow.git
   cd Mavis-Flow
   ```

2. **Setup environment:**
   Create a `.env` file:
   ```env
   GOOGLE_API_KEY=your_key_here
   ```

3. **Install & Run:**
   ```bash
   pip install -r requirements.txt
   python main.py
   ```

### Running the Model Proxy

The proxy allows other clients to access your OpenClaw models through an OpenAI-compatible API.

1. **Install requirements:**
   ```bash
   pip install flask
   ```

2. **Run the proxy:**
   ```bash
   python proxy/app.py
   ```

The proxy will be available at `http://localhost:18790/v1`.

## License

Distributed under the **MIT License**.

---
Built with ❤️ by [Mavis](https://github.com/Mavisy75106)
