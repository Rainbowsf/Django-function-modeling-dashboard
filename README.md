# 70ec15bf614ceec61b217f3addfa4ebaes
Начинающий Python разработчик

Дэшборд моделирования функций

Тестовое задание от компании Alytics


О проекте:

  1. Для моделирования графиков используется matplotlib и numpy. Сам процес производится через ассинхронные задачи Celery
  2. Количество функций которые можно вбить ограничивается стандартной библиотекой + numpy(sin, log etc.)
  3. Для более быстрой подгрузки изображений графиков было принято решение поставить Redis как систему кеширования
  

Для корректной работы:

  1. Поменять настройки базы данных
  2. Все что устанавливать > pip install -r req.txt
  3. cd schedules
  4. python manage.py runserver
  5. Команда для celery worker > celery -A schedules worker -l INFO


P.S. Не успел за выходные запихнуть все в докер-композ, хотя имею тыкательный опыт работы с ним.
