# Dev-зона для базовой разработки на 1С-Битрикс: Управление сайтом

Конфигурации служб nginx, apache, mysql взяты из bitrix-env. Таким образом размещенная копия 1С-Битрикс проходит все проверки "Проверка системы"

## Установка
1. Склонировать репозиторий
2. Создать файл .env и определить в нем переменные окружения `cp .env.copy .env`
3. Скачать актуальный инсталятор `curl https://www.1c-bitrix.ru/download/scripts/bitrixsetup.php --output bitrix/bitrixsetup.php`
4. С помощью docker-compose развернуть инфраструктуру `docker-compose up --build -d`
5. Запустить в браузере http://127.0.0.1/bitrixsetup.php (настройка битрикс)
