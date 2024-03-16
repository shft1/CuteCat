[![Main Kitty workflow](https://github.com/shft1/kittygram_final/actions/workflows/main.yml/badge.svg)](https://github.com/shft1/kittygram_final/actions/workflows/main.yml)

## О проекте:
Проект Kittygram предоставляет площадку для размещению своих любимых животных

## Стек технологий:
- Djando
- React
- Docker
- Postgres

## Как развернуть проект:
- Установить Docker
- Заполнить файл env
- Запустить docker compose 

## Как заполнить файл env ?:
- POSTGRES_DB - имя базы данных 
- POSTGRES_USER - имя пользователя с правами к базе
- POSTGRES_PASSWORD - пароль пользователя
- DB_NAME - имя контейнера, в котором запущена СУБД
- DB_PORT - порт, на котором работает контейнер с СУБД
- SQLITE - для использования базы данных sqlite надо передать значение True/true
- SECRET_KEY - для секретного ключа
- DEBUG - что включения режима отладки значение True/true
- ALLOWED_HOSTS - разрешенные хосты

## Что нужно сделать

Настроить запуск проекта Kittygram в контейнерах и CI/CD с помощью GitHub Actions

## Как проверить работу с помощью автотестов

В корне репозитория создайте файл tests.yml со следующим содержимым:
```yaml
repo_owner: ваш_логин_на_гитхабе
kittygram_domain: полная ссылка (https://доменное_имя) на ваш проект Kittygram
taski_domain: полная ссылка (https://доменное_имя) на ваш проект Taski
dockerhub_username: ваш_логин_на_докерхабе
```

Скопируйте содержимое файла `.github/workflows/main.yml` в файл `kittygram_workflow.yml` в корневой директории проекта.

Для локального запуска тестов создайте виртуальное окружение, установите в него зависимости из backend/requirements.txt и запустите в корневой директории проекта `pytest`.

## Чек-лист для проверки перед отправкой задания

- Проект Taski доступен по доменному имени, указанному в `tests.yml`.
- Проект Kittygram доступен по доменному имени, указанному в `tests.yml`.
- Пуш в ветку main запускает тестирование и деплой Kittygram, а после успешного деплоя вам приходит сообщение в телеграм.
- В корне проекта есть файл `kittygram_workflow.yml`.

## Автор 
Алексей
[Ссылка на гитхаб](https://github.com/shft1)
