# 1 

[https://hub.docker.com/r/alllexk/some-content-nginx](https://hub.docker.com/r/alllexk/some-content-nginx)

docker pull alllexk/some-content-nginx

![nginx](https://github.com/alllexk/DEVSYS23-05-virt-03-docker-Kozlovsky-Aleksander/blob/main/images/Nginx.png)

# 2

Высоконагруженное монолитное java веб-приложение - Физический сервер, т.к. монолит - нет микросервисной архитектуры и потому, что высоконагруженное.

Nodejs веб-приложение - Docker, т.к. в этом случае можно организовать микросервисную архитектуру.

Мобильное приложение c версиями для Android и iOS - Docker, также возможно на виртуальных машинах, зависит от типа приложения.

Шина данных на базе Apache Kafka - на виртуальные сервера, из-за высоконагруженности и для удобства выделения новых узлов;

Elasticsearch кластер для реализации логирования продуктивного веб-приложения - три ноды elasticsearch, два logstash и две ноды kibana; - можно запустить и на VM, но предпочтительнее все же использовать докер, если проект строится на миеросервисах.

Мониторинг-стек на базе Prometheus и Grafana; - докер, если в микросервисной архитектуре, vm вне ее.

MongoDB, как основное хранилище данных для java-приложения; - виртуальная машина.

Gitlab сервер для реализации CI/CD процессов и приватный (закрытый) Docker Registry. - на данный момент выбрал бы контейнеризацию. При необходимости на виртуальной машине.

# 3

![nginx](https://github.com/alllexk/DEVSYS23-05-virt-03-docker-Kozlovsky-Aleksander/blob/a6e0e010959d1d52a1ad854769683c433c79ddf0/images/3.png)
