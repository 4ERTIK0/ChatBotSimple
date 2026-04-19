# ChatBotSimple
Простой чат-бот на Python с использованием обработки естественного языка (NLP) и нейронной сети на базе Keras. Бот обучен на заранее заданных интентах и умеет отвечать на пользовательские запросы в консоли.

📌 Возможности
Обработка текста с помощью NLTK
Лемматизация слов
Классификация интентов с помощью нейросети
Генерация ответов на основе intents.json
Консольный интерфейс общения
🧠 Как это работает
Пользователь вводит сообщение
Текст токенизируется и лемматизируется
Создается мешок слов (Bag of Words)
Модель предсказывает интент
Бот выбирает случайный ответ из соответствующего интента
📂 Структура проекта
Souce Code/
│
├── ChatBot_Application.py      # Основной файл запуска бота
├── chatBot_model_file.py      # Скрипт обучения модели
├── ChatBot.ipynb              # Jupyter Notebook (обучение/эксперименты)
├── chatbot_Application_model.h5  # Обученная модель
├── intents.json               # Интенты и ответы
├── words.pkl                  # Словарь слов
├── labels.pkl                 # Метки классов
⚙️ Установка

Убедись, что у тебя установлен Python 3.x

Установи зависимости:

pip install nltk numpy keras tensorflow

Также нужно загрузить ресурсы NLTK:

import nltk
nltk.download('punkt')
nltk.download('wordnet')
🚀 Запуск

Перейди в папку проекта и запусти:

python ChatBot_Application.py

После этого можно начать диалог:

You: Hello
BOT: Hi there!

Чтобы выйти:

quit
🧩 Основные функции
bank_of_words() — преобразует текст в вектор
predict_label() — предсказывает интент
Response() — выбирает ответ
chatbot_response() — объединяет всё
chat() — запускает цикл общения
📊 Модель
Используется Keras
Формат модели: .h5
Порог уверенности: 0.25




A simple Python-based chatbot that uses Natural Language Processing (NLP) and a neural network built with Keras. The bot is trained on predefined intents and can respond to user inputs via the console.

📌 Features
Text processing using NLTK
Word lemmatization
Intent classification with a neural network
Response generation based on intents.json
Console-based chat interface
🧠 How It Works
User enters a message
The text is tokenized and lemmatized
A Bag-of-Words representation is created
The model predicts the intent
The bot selects a random response from the matched intent
📂 Project Structure
Souce Code/
│
├── ChatBot_Application.py         # Main chatbot script
├── chatBot_model_file.py          # Model training script
├── ChatBot.ipynb                  # Jupyter Notebook (training/experiments)
├── chatbot_Application_model.h5   # Trained model
├── intents.json                   # Intents and responses
├── words.pkl                      # Vocabulary
├── labels.pkl                     # Class labels
⚙️ Installation

Make sure you have Python 3.x installed.

Install dependencies:

pip install nltk numpy keras tensorflow

Download required NLTK data:

import nltk
nltk.download('punkt')
nltk.download('wordnet')
🚀 Run the Project

Navigate to the project directory and run:

python ChatBot_Application.py

Example interaction:

You: Hello
BOT: Hi there!

To exit:

quit
🧩 Core Functions
bank_of_words() — converts text into a vector
predict_label() — predicts the intent
Response() — selects a response
chatbot_response() — integrates prediction + response
chat() — runs the conversation loop
📊 Model Details
Built using Keras
Model format: .h5
Confidence threshold: 0.25
