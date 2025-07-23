# docker-compose-dev-env

This repository includes docker-compose and relevant files to build docker based tech stack on your computer.


**Tech stack **

* Monitoring
  * Prometheus
  * Grafana
* Database
  * PostgreSQL
  * MongoDB
* Message Queue
  * RabbitMQ
* Streaming
  * Pulsar
* Search
  * ElasticSearch
* Log Management
  * To be defined


**Installation**

Following installation steps would make the stack ready. Please find docker-compose.yml for the composing details and following descriptions tohave insight about each tech component details such as open ports, volumes, networking etc...



Network : Unlike installations in production environment, all the components in development environment resides in the same network. Network name is "backend-network"

Volume : Only one directory in the filesytem is to be mounted as a volume where each components will have own subdirectories. Volume name is "devenv-volume"

Monitoring...



Building and composing images
docker-compose up --d

Stopping container : docker-compose stop

These methods should be run under the same directory of composition file.
