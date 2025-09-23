<h1 align="center"> Привет! Я <a target="_blank"> Кармеев Артур из группы ЭФМО-01-25 </a> 
<img src="https://github.com/blackcater/blackcater/raw/main/images/Hi.gif" height="32"/></h1>
<h3 align="center"> Данная практика была выполнена со всеми доп заданиями!</h3>

## Структура проекта

    helloapi/
    ├── go.mod
    ├── go.sum
    ├── helloapi.exe
    ├── .git/
    └── cmd/
        └── server/
            └── main.go
Директории создавались с помощью утилиты "mkdir"

Файл создавался с помощью утилиты "New-Item"

## 1. Подготовка окружения и проверка версий
go version

git --version

<img width="444" height="96" alt="image" src="https://github.com/user-attachments/assets/fa771553-1d1e-46ee-a2e0-33b0d183eaa2" />

## 2. Минимальный HTTP-сервер

Финальный код можно посмотреть в файле main.go (Путь к файлу "helloapi/cmd/server/main.go")

## 3. Запуск сервера и быстрая проверка

Запускае сервер в PowerShell командой "go run ./cmd/server" или ".\helloapi.exe"

<img width="974" height="409" alt="image" src="https://github.com/user-attachments/assets/f21b8b07-3e48-4320-83f7-3ca9d35490c4" />


<img width="974" height="130" alt="image" src="https://github.com/user-attachments/assets/db030ff1-c86f-4410-9d0d-2a7ee21d6999" />


Проверяем что будет на выводе при вводе команд 

curl http://localhost:8080/hello

curl http://localhost:8080/user

curl http://localhost:8080/health

<img width="974" height="373" alt="image" src="https://github.com/user-attachments/assets/6d267d44-b0a3-4e13-a9e3-7e6ad54ee5a7" />


<img width="974" height="410" alt="image" src="https://github.com/user-attachments/assets/cec293ec-9bd1-4951-a64f-637ace0f055c" />


<img width="974" height="409" alt="image" src="https://github.com/user-attachments/assets/9833c9cd-26f6-43dc-b452-14440ae28112" />

## 4. Код-стайл и базовые проверки
Отформатируем и проверим код стандартными инструментами Go:

go fmt ./...

go vet ./...

<img width="827" height="161" alt="image" src="https://github.com/user-attachments/assets/990e5683-8192-4555-891c-00c5935c3f47" />

Ошибок нет:)

## 5. Запуск на другом порту

$env:APP_PORT="8081"

go run ./cmd/server

теперь сервер слушает :8081

<img width="974" height="143" alt="image" src="https://github.com/user-attachments/assets/ade4f4a8-6a60-45c4-a84f-0637cc1cc3fd" />
