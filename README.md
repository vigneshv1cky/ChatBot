
# 🤖 Gemini-Pro ChatBot

A simple Streamlit application that lets you chat with Google’s Gemini-Pro AI models in a conversational UI.

---

## Table of Contents

1. [Overview](#overview)  
2. [Features](#features)  
3. [Prerequisites](#prerequisites)  
4. [Installation](#installation)  
5. [Configuration](#configuration)  
6. [Usage](#usage)  
7. [Code Structure](#code-structure)  

---

## Overview

This app provides a front-end wrapper around Google’s Gemini-Pro generative AI. Users can type questions or prompts into the Streamlit UI and receive AI responses in real time.

---

## Features

- 🔒 Secure loading of API keys via `.env`  
- 🎨 Simple, centered Streamlit layout with emoji favicon  
- ↔️ Bi-directional chat: user ↔️ assistant  
- 🔄 Persistent chat history across reruns (via `st.session_state`)  
- 🛠️ Easy to swap or list supported Gemini-Pro models  

---

## Prerequisites

- Python 3.8+  
- A valid Google Cloud API key with access to Gemini-Pro  
- Basic familiarity with Streamlit  

---

## Installation

1. **Clone the repo**  

   ```bash
   git clone https://github.com/your-username/gemini-pro-chatbot.git
   cd gemini-pro-chatbot
   ```

2. **Create & activate a virtual environment**  

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate    # macOS/Linux
   .\.venv\Scripts\activate     # Windows
   ```

3. **Install dependencies**  

   ```bash
   pip install -r requirements.txt
   ```

---

## Configuration

1. **Create a `.env` file** in the project root:

   ```dotenv
   GOOGLE_API_KEY=your_google_api_key_here
   ```

2. Streamlit will automatically load this on startup.

---

## Usage

Run the app locally with:

```bash
streamlit run app.py
```

Then open the URL printed in your terminal (usually `http://localhost:8501`) in your browser.

---

## Code Structure

```
.
├── app.py             # Main Streamlit application
├── requirements.txt   # Python dependencies
├── .env.example       # Example environment variables file
├── README.md          # This documentation
└── .gitignore
```

---
