# EduardDzhagaev_microservices
EduardDzhagaev microservices repository

ДЗ №22
##### Kubernetes-4 #####

Установлен Helm, Tiller и затем позже Helm3
Написаны chart
Реализованы управления зависимостями
Установлен helm2 tiller plugin
Установлен Gitlab из Omnibus
Сделан запуск проекта в Gitlab
Написание pipeline в Gitlab
Deploy


ДЗ №21
##### Kubernetes-3 #####

Проверено отключение kube-dns
Опробован service типа NodePort
Опробован service типа LoadBalancer
Установлен Ingress Controller и опробован Ingress
Включение TLS termination
Настроен Network Policy
Добавлен и настроен volume


ДЗ №20
##### Kubernetes-2 #####

Инсталлировал Minikube на Debian11
Частично изучены параметры конфигуарционного файла для Minikube
Созданы файлы с описанием Deployments, Services, namespace
Опробовал Dashboard для Minikube
Протестировал создание компонентов в отдельном namespace "dev" 
Создал на YandexCloud K8s cluster
Протестировал разворачивание приложения на K8s cluster в YandexCloud в namespace "dev"


ДЗ №19
##### Kubernetes-1 #####

Развернул Kubernetes на Debian11 при помощи "kubeadm"
В ходе инсталяции была произведена: 
- настройка UFW  на нодах
- установка среды выполнения контейнера CRI-O
- установка пакетов k8s - kubeadm, kubelet, kubectl
- Инсталяция network plugin "Calico"
Затем были составлены и опробованы манифесты в k8s



ДЗ №18
##### Logging-1 #####

Построил EFK через docker compose
Многократно и последовательно составлены Dockerfile и fluent.conf
Собрали image для fluentd
Добавил logging-драйвер в docker-compose.yml
Опробованы фильтры для сбора структурированных логов
Опробованы фильтры для сбора неструктурированных логов
Опробован "Zipkin" для просмотра трейсов


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
