# 🛍️ SmartShopService

**SmartShopService** — это микросервисный проект, демонстрирующий взаимодействие трех сервисов с использованием Docker и RabbitMQ. Проект включает:

- Django-сервис (`sales_django`)
- Flask-сервис (`orders_flask`)
- RabbitMQ-сервис обработки сообщений (`repair_rabbit`)
- Брокер сообщений RabbitMQ с веб-интерфейсом

## 🌐 Сервисы и порты

🧠 Django (sales): http://localhost:8000

📦 Flask (orders): http://localhost:5000

📨 RabbitMQ Management: http://localhost:15672

Логин: guest

Пароль: guest

Очереди: во вкладке Queues

📝 Заметки
Каждый сервис использует собственный Dockerfile и requirements.txt.
Сервис orders_flask и repair_rabbit используют RabbitMQ для обмена сообщениями.
Все сервисы монтируются в контейнеры, что упрощает локальную разработку.
