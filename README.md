# EduardDzhagaev_microservices
EduardDzhagaev microservices repository

ДЗ №17
##### Monitoring-1 #####

Установка Prometheus в docker
Добавление targets для сбора метрик
Заполнение "docker-compose.yml" для поднятия контейнеров
Проверил мониторинга при выключении контейнера приложения
Добавление "node-экспортёра" в "docker-compose.yml"
Проверка мониторинга после добавления "node-экспортёра"

Repo for "docker hub" c моими images:
https://hub.docker.com/repositories/schtrauch

docker pull schtrauch/prometheus
docker pull schtrauch/post
docker pull schtrauch/comment
docker pull schtrauch/ui 

ДЗ №16
##### Gitlab-ci-1 #####

Установил Gitlab-СI на vm в варианте инсталляции Omnibus
Выполнил первоначальную настройку GitLab. Cоздал group и project. 
Установил и зарегистрировал GitLab-Runner
В ".gitlab-ci.yml" написан код pipeline
Протестировал создание окружений


ДЗ №15
##### Docker-4 #####

Изучил 3 разных типа сетей в Docker - none, host, bridge
Выполнил практическую часть по разворачиванию контейнеров в разных типах сетей
Изучил и опробовал инструмент "docker-compose" для описания сервиса из множества контейнеров

Узнайте как образуется базовое имя проекта. Можно ли его задать? Если можно то как? Ответ добавьте в Readme.md данного ДЗ

docker-compose
-p, --project-name NAME     Specify an alternate project name
                                  (default: directory name)

По умолчанию берется имя папки из которой создаются сервисы.


ДЗ №13
##### Docker-3 #####

Установил "linter" для проверки и подсказок при создании Dockerfile
Скопировал архив и распаковал его в src/ в этом репозитории
Cоздал 3 Dockerfile
Делал проверку при помощи "linter" для проверки Dockerfile. Часть подсказок была использована.
Создал images из этих Dockerfile.
Создал bridge reddit с возможностью разрешать хосты в пределах сети.
Запустил docker контейнеры и проверка приложения по адресу 
http://<public_IP>:9292.


ДЗ №12
##### Docker-2 #####

В рамках обучения было выполнено:

Изучены основные базовые команды docker.
Создан контейнер для приложения reddit.
Развернут docker-host через docker-machine
Push image на docker hub и его проверка
