A high-performance, multi-language Telegram AI chatbot built with Python and python-telegram-bot v20+, powered by OpenRouter (DeepSeek-V3).
This is a rebranded and enhanced edition, focused on clean architecture, easy deployment, and flexible AI behavior control.

> ⚠️ Educational & experimental project. Use responsibly.




---

✨ What’s New in This Rebranded Version

🔁 Complete README rebranding

🧠 Cleaner bot flow & prompt handling

🌐 Multi-language system (🇮🇩 Indonesian / 🇺🇸 English)

💾 Persistent user language memory (JSON-based)

⚙️ Environment-variable driven configuration

🚄 Optimized for Railway / Replit / Local

🤖 DeepSeek-V3 via OpenRouter



---

🌍 Language Support

Users can choose their preferred language on /start using inline buttons:

🇮🇩 Indonesian

🇺🇸 English


The bot automatically remembers the user’s selection.

Manual Commands

/setlang id
/setlang en


---

📌 Core Features

🤖 AI responses via OpenRouter (DeepSeek Chat V3)

⚡ Async architecture (fast & scalable)

💬 Language-aware replies

🧠 Dynamic system-prompt injection

🔧 Easy to host anywhere

🗂 Lightweight JSON storage (no database required)



---

📂 Project Structure

WormGPT/
│
├── telegram_bot.py      # Core bot logic
├── main.py              # Entry point (Railway-compatible)
├── system-prompt.txt    # Optional custom system prompt
├── user_langs.json      # Auto-created language storage
├── wormgpt_config.json  # Optional advanced config
├── requirements.txt
└── README.md


---

🔧 Installation

1️⃣ Install Dependencies

pip install -r requirements.txt

Main packages used:

python-telegram-bot==20.3

requests

python-dotenv

flask (Railway support)



---

🔑 Environment Variables

Set the following variables in your hosting platform:

Variable Name	Description

TELEGRAM_TOKEN	Telegram Bot Token
OPENROUTER_KEY	OpenRouter API Key



---

▶️ Run Locally

python main.py


---

🤖 Bot Flow (How It Works)

/start

Shows welcome message

Displays language selector

Saves user preference


User sends message

Loads user language (default: Indonesian)

Builds language-specific system prompt

Sends request to OpenRouter (DeepSeek)

Returns AI response in selected language



---

🧠 Multi-Language Prompt Logic

The system dynamically injects a language-locked system prompt:

🇮🇩 Indonesian → Always reply in Indonesian

🇺🇸 English → Always reply in English


Prompt behavior can be customized via system-prompt.txt.


---

🧪 Example

/start

Bot response:

Welcome to WormGPT!
Please choose your language:
[🇮🇩 Indonesian] [🇺🇸 English]

After selection:

✅ Language set successfully. You can now start chatting.


---

🌐 Live Bot (Demo)

You can test the bot here (if active):
👉 https://t.me/Wormgpttested_bot


---

🚀 Deploy on Railway (Recommended)

1. Push this repo to GitHub


2. Create a new Railway service


3. Select Deploy from GitHub


4. Add environment variables


5. Deploy ✅



Railway handles everything automatically.


---

🛠 main.py (Minimal Example)

if __name__ == "__main__":
    run_bot()


---

🧾 Requirements

requests
python-telegram-bot==20.3
python-dotenv
flask


---

🧧 Credits & Acknowledgements

Original Concept & Development Credit: AbdulDev

Rebranding & README Enhancement: Community Edition

AI Provider: OpenRouter.ai

Model: DeepSeek Chat V3

Telegram Framework: python-telegram-bot


> ⚠️ Please do not remove credits. Respect open-source ethics.




---

❤️ License

MIT License
Free to fork, modify, and improve — attribution required.
