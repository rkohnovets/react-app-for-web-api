Фронтенд к бэкенду из репозитория: https://github.com/rkohnovets/AspNetCoreWebAPI

В нем используется React Router v6, реализованы вход/выход/регистрация и маршрутизация с приватными роутами.

Скачав, в терминале (командной строке) набираем: 
    
    npm install
    
Далее, чтобы запустить, в терминале набираем: 
    
    npm run start
    
Чтобы запустить через Docker:
  1) Если на винде, то нужно установить Docker Desktop (на других ОС не знаю) и запустить
  2) В терминале в папке с репозиторием пишем (вместе с точкой):
     
     ```
     docker build -t sample:dev .
     ```
     
  3) Для запуска пишем:
     
     ```
     docker run -it -v ${PWD}:/app -v /app/node_modules -p 3000:3000 sample:dev
     ```
     
