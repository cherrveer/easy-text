# easyText
это программное обеспечение, спроектированное для распознавания текста с сайтов

# Учасники проекта: 
Ерохин Андрей, Тимошенко Василий, Аванесов Артем, Артищев Роман, Аюпов Арсен, Артюхович Иван

# Документация к проекту

## Диаграмма последовательностей
![](readme_assets/Диаграмма_последовательностей.png)

## ERD диаграмма
![](readme_assets/database-entity-relation-diagram.jpg)

## Запуск
```bash
git clone https://github.com/cherrveer/easy-text.git
cd easyText
docker system prune -fa --volumes # удалить прошлые билды
docker compose up --build --force-recreate # создать новый билд
Ctrl-C # после запуска закрыть
docker compose up # запустить заново
# сделать один запрос чтобы установились адблоки
```
