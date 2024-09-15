# Проект Webpack и JSON-server

Этот проект демонстрирует настройку Webpack с `webpack-dev-server` и настройку JSON-server для получения данных. Также настроен линтер, который запускается при коммите.

## Установка

1. **Клонируйте репозиторий:**

   ```bash
   git clone <URL-вашего-репозитория>
   cd <директория-проекта>

2. **Установите зависимости Node.js:**

   npm install

3. **Установите зависимости Python:**

   #Создайте виртуальную среду (если еще не создана):


   python -m venv venv
   #Активируйте виртуальную среду:

   #На macOS/Linux:
   source venv/bin/activate
   #На Windows:


   venv\Scripts\activate

   #Установите зависимости из requirements.txt:

   pip install -r requirements.txt

4.  **Запуск сервера разработки с HMR: **

    npm run dev

   
Это запустит Webpack Dev Server с поддержкой Hot Module Replacement (HMR) на порту 3000.

5. **Сборка проекта для продакшена:**

   npm run build

Это соберет проект в режиме продакшена и создаст оптимизированные файлы в папке dist.

6. **Запуск JSON-server:**


   npm run json-server

Это запустит JSON-server, который будет слушать на порту 3001.

Python
Запуск серверной части (если есть):

Например, если у вас есть серверный скрипт на Flask, запустите его с помощью:

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

