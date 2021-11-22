# Elastic Stack with Docker
#### Testing how Elastic Stack works in Docker environment
Using [apache-http-logs](https://github.com/ocatak/apache-http-logs.git) and [Student Performance in Exams](https://www.kaggle.com/spscientist/students-performance-in-exams) 

### Steps:
1. Clone repository
2. Build docker containers using "docker-compose build"
3. Start Elastic Stack containers using:
- "docker-compose up -d"
- "docker swarm init" -> "docker stack deploy -c docker.stack.yml elk" (to run as a swarm)
![swarm](/images/swarm.png)
4. Create index pattern in Kibana for chosen index ("logs" or "datasets")
5. Analyze data in Discovery tab or create Dashboard with visualizations
![kibana_discover](/images/kibana_discover.png)

### TODO:
1.  Kibana dashboards
