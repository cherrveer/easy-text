# easyText
это парсинговое веб-приложение с возможностью регистрации и входа для копирования информации с сайтов, запрещающих это. Веб-приложение использует нейросеть.

# Учасники проекта: 
Ерохин Андрей, Тимошенко Василий, Аванесов Артем, Артищев Роман, Аюпов Арсен, Артюхович Иван

# Презентация проекта:
![](readme_assets/1.png)
![](readme_assets/2.png)
![](readme_assets/3.png)
![](readme_assets/4.png)
![](readme_assets/5.png)
![](readme_assets/6.png)

# Инструкция для пользователя 
Видео по ссылке: https://disk.yandex.ru/d/8oWdGRe6NmNNyA

# Документация к проекту:

## Макет сайта в FIGMA
https://www.figma.com/file/p9YTG2X5x22UNVpuqrenmi/easyText?type=design&node-id=0%3A1&mode=design&t=5iYq4lMzGLEpwFoJ-1

## User story
Клиент заходит на главную страницу сайта. Клиент регистрируется или входит в аккаунт на сайте. Клиент ознакамливается с информацией на сайте. Клиент нажимает на кнопку "easyText" и видит интерфейс нейросети. Вставляет ссылку в поле "URL-ссылка". Клиент нажимает на кнопку "Анализировать". Клиент получает исходный текст со страницы по ссылке, которую он вставил. Клиент может скопировать весь текст или нужный ему фрагмент. По завершении, клиент может повторить процесс для других ссылок или покинуть сайт.

## Диаграмма последовательностей
![](readme_assets/последовательностей.png)

## DFD (Процесс работы функционала)
![](readme_assets/erd.png)

## Диаграмма состояний (Процесс работы веь-приложения)
![](readme_assets/Use_case(Веб-приложение).png)

## Алгаритм работы нейросети 
![](readme_assets/Алгаритм_работы_нейросети.png)

## Use case
![](readme_assets/Состояния.png)

## ERD диаграмма
![](readme_assets/database-entity-relation-diagram.jpg)

## API swagger
![](readme_assets/screencapture-editor-next-swagger-io-2024-05-22-11_17_43.png)

# Инструкция для администратора
```bash
git clone https://github.com/cherrveer/easy-text.git
cd easyText
docker system prune -fa --volumes # удалить прошлые билды
docker compose up --build --force-recreate # создать новый билд
Ctrl-C # после запуска закрыть
docker compose up # запустить заново
# сделать один запрос чтобы установились адблоки
```
