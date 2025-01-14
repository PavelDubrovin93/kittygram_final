![badge for review](https://github.com/PavelDubrovin93/kittygram_final/actions/workflows/main.yml/badge.svg)

# Это Kittygram: учебный проект! Что бы смотреть на чужих котов и хвастаться своими! а так же ознакомить студентов со следующим стеком техноголгий:

 - Django Rest Framework
 - PostgreSQL
 - GitHub Actions
 - Docker

## Проектов много, но мой - один!

 - Для деплоя проекта требуется:
    - Копировать содержимое файла **kittygram_workflow.yml** в /.github/worflows/main.yml.
    - настроить для репозитория следующие секреты:
     - DOCKER_LOGIN
     - DOCKER PASSOWORD
     - HOST (IP сервера)
     - USER (Имя пальзователя на сервере)
     - SSH_KEY
     - SSH_PHASSPHRASE
     + опционально, для работы оповещений в Телеграме:
     - TELEGRAM_TO (ID юзера, которому должно прийти оповещение)
     - TELEGRAM_TOKEN (токен бота, который должен отправить оповещение)
    - запушить проет на ветку main.

 - Для корректной работы потребуется разместить в корневой директории файл **.env** со следующими переменными:
    - POSTGRES_DB=exemple_db_name
    - POSTGRES_USER=exemple_user
    - POSTGRES_PASSWORD=exemple_password
    - DB_HOST=db 
    - DB_PORT=5432
    - DEBUG_MODE=false
    - SECRET_KEY=exemple_secret_key
    - ALLOWED_HOSTS= ip.of.your.host, your-own-domain.exemple.ru, localhost

### В разработе учавствовали [Дубровин Павел](https://github.com/PavelDubrovin93),[Игорь Шкода](https://github.com/Port-tf) и [Андрей Дубинчик](https://github.com/evi1ghost). При вспомоществовании Яндекс.Практиум