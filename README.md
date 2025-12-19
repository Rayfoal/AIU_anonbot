# Telegram Feedback Bot

**Telegram bot** that collects user feedback, saves it in Excel, and notifies the administrator.

---

## 📌 Features
- User commands:
  - `/start` — greeting and bot initialization
  - `/feedback` — start submitting feedback
  - `/cancel` — cancel feedback submission
- Category selection via buttons:
  - Teachers
  - Subjects
  - Schedule
  - Infrastructure
  - Other
- Admin notifications with:
  - Timestamp
  - Category
  - Feedback text
- Save all feedback to Excel (`feedbacks.xlsx`)  

---

## ⚙️ Installation & Running
** 1. Clone the repository **
git clone https://github.com/YOUR_USERNAME/telegram-feedback-bot.git
cd telegram-feedback-bot

** 2. Create a virtual environment and install dependencies **
python -m venv venv
** Linux/Mac **
source venv/bin/activate
** Windows **
venv\Scripts\activate
pip install -r requirements.txt

** 3. Create a .env file with your settings **
API_TOKEN=your_bot_token
ADMIN_CHAT_ID=your_chat_id

** 4. Project structure **
telegram-feedback-bot/
│
├─ bot.py               # Main bot code
├─ requirements.txt     # Python dependencies
├─ README.md            # This file
└─ .gitignore           # Ignored files, e.g., .env

---

## 📦 Dependencies
Python 3.11+  
aiogram — Telegram bot library  
openpyxl — Excel handling library  

---

## 💡 Notes
- The `.env` file is not uploaded to GitHub (keeps bot token and admin ID secure).  
- If `feedbacks.xlsx` is missing — it is created automatically on first run.  
- The bot requires internet access and works via the Telegram API.  

---

## 🔒 Security
- Bot token and admin ID are stored in `.env`.  
- Excel file is stored locally only.  

---

## Documentation
Full documentation and project description are available on [Notion](https://www.notion.so/Software-Requirements-Specification-SRS-2ce45bace9eb805ebbaad60dc79b73a3?source=copy_link)
