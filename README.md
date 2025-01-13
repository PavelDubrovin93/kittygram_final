![badge for review](https://github.com/PavelDubrovin93/kittygram_final/actions/workflows/main.yml/badge.svg)
#  Как работать с репозиторием финального задания

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

# Это мой проект! Что бы смотреть на чужих котов и хвастаться своими!

## Проектов много, но мой - один!

 - Проект приспособлен для работы с Docker.
 - Для деплоя проекта нужно ознакомиться с информацией по [ссылке](https://practicum.yandex.ru/learn/backend-developer/courses/79e74b86-a425-4a5b-b5c1-a7793c64cfd5/sprints/263913/topics/e54b8d80-9610-4b01-90bf-4c19ca27a6b1/lessons/5add92f2-5936-45b3-b5c2-d961ac9bfee1/#6a404504-6c58-4eb7-80d7-c3ca917e80e9)
 - Для корректной работы потребуется развестить в корневой директории файл **.env** со следующими переменными:
    - POSTGRES_DB=exemple_db_name
    - POSTGRES_USER=exemple_user
    - POSTGRES_PASSWORD=exemple_password
    - DB_HOST=db 
    - DB_PORT=5432
    - 
    - DEBUG_MODE=false
    - SECRET_KEY=exemple_secret_key
    - ALLOWED_HOSTS= ip.of.your.host, your-own-domain.exemple.ru, localhost