Разверачиваем Prometheus Stack включающий в себя:
- Prometheus,
- Grafana,
- Node Exporter,
- Blackbox Exporter,
- AlertManager.

Настроен сбор метрик с сайта через Blackbox.
Также собераются метрики с вашего сервера через Node Exporter.

Добавлены оповещения в AlertManager через Telegram на следующие события:
- изменился статус-код сайта;
- задержка превышает 5 секунд;
- сервер перезагрузился.

### Настройка
Для работы оповещения в Telegram необходимо создать файл .env и указать ваши TELEGRAM_ADMIN и TELEGRAM_TOKEN.
В первом нужно указать id вашего профиля, который можно узнать у @my_id_bot, второй — это токен бота, который создан через @BotFather.
