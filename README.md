# Elastic Stack with Docker
#### Testing how Elastic Stack works in Docker environment
#### Using [apache-http-logs](https://github.com/ocatak/apache-http-logs.git) and [Student Performance in Exams](https://www.kaggle.com/spscientist/students-performance-in-exams) 

### Steps:
#### 1) Clone repository
#### 2) Use "docker-compose up -d --build" to build and run Elastic Stack containers
#### 2.5) Or use "docker swarm init" and "docker stack deploy -c docker-stack.yml elk" to run ELK as a swarm
![swarm](/images/swarm.png)
#### 3) Create index pattern in Kibana for chosen index (logs or datasets)
#### 4) Analyze collected data in Discovery tab
![kibana_discover](/images/kibana_discover.png)

### TODO:
#### 1) Kibana dashboards
