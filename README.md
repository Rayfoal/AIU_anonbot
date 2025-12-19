# Telegram Feedback Bot

Бот для Telegram, который собирает отзывы пользователей, сохраняет их в Excel и уведомляет администратора.

## Функционал
- `/start` — приветствие пользователя.  
- `/feedback` — начать процесс отправки отзыва.  
- `/cancel` — отменить отправку отзыва.  
- Выбор категории отзыва через кнопки:  
  - Преподаватели  
  - Предметы  
  - Расписание  
  - Инфраструктура  
  - Другое  
- Отправка уведомления админу с текстом, категорией и временем.  
- Сохранение всех отзывов в Excel (`feedbacks.xlsx`).  

## Установка и запуск
1. Клонируйте репозиторий:
```bash
git clone https://github.com/ВАШ_ЮЗЕРНЕЙМ/telegram-feedback-bot.git
cd telegram-feedback-bot
```
Создайте виртуальное окружение и установите зависимости:

bash
Копировать код
python -m venv venv
source venv/bin/activate   # для Linux/Mac
venv\Scripts\activate      # для Windows
pip install -r requirements.txt
Создайте файл .env и добавьте переменные:

env
Копировать код
API_TOKEN=ваш_токен_бота
ADMIN_CHAT_ID=ваш_chat_id
Запустите бота:

bash
Копировать код
python bot.py
Зависимости
Python 3.11+

aiogram

openpyxl

Структура проекта
Копировать код
telegram-feedback-bot/
│
├─ bot.py
├─ requirements.txt
├─ README.md
└─ .gitignore
Примечания
.env файл не загружается в репозиторий.

Excel создаётся автоматически при первом запуске, если файла нет.
