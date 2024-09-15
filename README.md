# Проект Webpack и JSON-server

Этот проект демонстрирует настройку Webpack с `webpack-dev-server` и настройку JSON-server для получения данных. Также настроен линтер, который запускается при коммите.

## Установка

1. **Клонируйте репозиторий:**

   ```bash
   git clone <URL-вашего-репозитория>
   cd <директория-проекта>
Установите зависимости Node.js:

bash
Copy code
npm install
Установите зависимости Python:

Создайте виртуальную среду (если еще не создана):

bash
Copy code
python -m venv venv
Активируйте виртуальную среду:

На macOS/Linux:

bash
Copy code
source venv/bin/activate
На Windows:

bash
Copy code
venv\Scripts\activate
Установите зависимости из requirements.txt:

bash
Copy code
pip install -r requirements.txt
Команды
Node.js
Запуск сервера разработки с HMR:

bash
Copy code
npm run dev
Это запустит Webpack Dev Server с поддержкой Hot Module Replacement (HMR) на порту 3000.

Сборка проекта для продакшена:

bash
Copy code
npm run build
Это соберет проект в режиме продакшена и создаст оптимизированные файлы в папке dist.

Запуск JSON-server:

bash
Copy code
npm run json-server
Это запустит JSON-server, который будет слушать на порту 3001.

Python
Запуск серверной части (если есть):

Например, если у вас есть серверный скрипт на Flask, запустите его с помощью:

bash
Copy code
python server.py
Конфигурация
Webpack:

webpack.dev.js: Конфигурация для разработки, включает HMR.
webpack.prod.js: Конфигурация для продакшена, без HMR.
JSON-server:

Файл db.json содержит начальные данные для JSON-server.
ESLint:

Настроен для проверки кода с использованием eslint.config.mjs.
Линтер
При коммитах автоматически запускается линтер (ESLint). Если линтер находит ошибки, коммит будет прерван.

