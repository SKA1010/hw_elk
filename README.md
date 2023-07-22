# Домашнее задание к занятию «ELK»
### Задание 1. Elasticsearch 

Установите и запустите Elasticsearch, после чего поменяйте параметр cluster_name на случайный. 

*Приведите скриншот команды 'curl -X GET 'localhost:9200/_cluster/health?pretty', сделанной на сервере с установленным Elasticsearch. Где будет виден нестандартный cluster_name*.

---

### Решение 1. Elasticsearch 

Домашнее задание выполнялось в Docker Compose. Все компоненты "раскиданы" по контейнерам.

Констейнер с Elasticsearch работает:

![1](https://github.com/SKA1010/hw_elk/assets/125235217/425379a7-5170-41f7-9823-49d424317b4d)

---

### Задание 2. Kibana

Установите и запустите Kibana.

*Приведите скриншот интерфейса Kibana на странице http://<ip вашего сервера>:5601/app/dev_tools#/console, где будет выполнен запрос GET /_cluster/health?pretty*.

---

### Решение 2. Kibana

Контейнер с Kibana работает: 

![2](https://github.com/SKA1010/hw_elk/assets/125235217/48854f90-55a6-44b1-a934-c90faae3cd09)

---

### Задание 3. Logstash

Установите и запустите Logstash и Nginx. С помощью Logstash отправьте access-лог Nginx в Elasticsearch. 

*Приведите скриншот интерфейса Kibana, на котором видны логи Nginx.*

---

### Решение 3. Logstash

Доставка лога из Logstash работает:

![3-1](https://github.com/SKA1010/hw_elk/assets/125235217/ebc420ed-bf94-4e67-aac4-00ec09ad339e)

---

### Задание 4. Filebeat. 

Установите и запустите Filebeat. Переключите поставку логов Nginx с Logstash на Filebeat. 

*Приведите скриншот интерфейса Kibana, на котором видны логи Nginx, которые были отправлены через Filebeat.*
---

### Решение 4. Filebeat. 

Контейнер с Filebeat передает данные:

![4-3](https://github.com/SKA1010/hw_elk/assets/125235217/9e93cbdd-7401-4946-aee0-116aff1d6f55)

---

