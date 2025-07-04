# Симулятор диспетчера вызовов

**Симулятор диспетчера вызовов** — программа для управления и мониторинга вызовов на карте.

## Возможности программы

 Для старта нажмите "Запустить симуляцию".
 
- Отображение карты с вызовами:
  - Метки вызовов отображаются красным цветом.
  - **Двойные вызовы** — можно назначить две бригады.
  - **Одиночные вызовы** — можно назначить только одну бригаду.
- Состояния вызовов на карте:
  - 🔴 Красный — новый вызов.
  - 🟡 Желтый — бригада занята, вызов в работе.
  - 🔵 Синий — бригада в пути.
  - 🟠 Оранжевый — бригада на месте.
  - 🟢 Зеленый — вызов выполнен, работа завершена.
- Удаление меток вызовов с карты после их завершения.

## Работа с базой данных

- Используется **PostgreSQL**.
- В файле [`Commands.txt`](./Commands.txt) содержатся SQL-команды для создания таблиц и функций базы данных.
- Для подключения используется **DBeaver** или другой клиент PostgreSQL.
- Библиотеки для работы программы находятся в папке [`PG_Libs`](./PG_Libs).
- Примеры работы программы — в папке [`Examples_work`](./Examples_work).

## Дополнительные возможности

- Подключение/отключение к базе данных.
- Просмотр статистики и различных графиков.
- Сохранение состояния вызовов: при закрытии и повторном запуске программы данные вызовов сохраняются и продолжают работать.
- Чтобы всё удалить, нужно в настройках подключения выбрать пункт "Очистить данные" и заново подключиться к базе данных.
  
## Требования

- PostgreSQL (для работы с базой данных)
- Клиент для работы с PostgreSQL (например, DBeaver)
