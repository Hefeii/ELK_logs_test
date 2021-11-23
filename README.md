# Elastic Stack with Docker
#### Testing how Elastic Stack works in Docker environment
Using [apache-http-logs](https://github.com/ocatak/apache-http-logs.git) and [Student Performance in Exams](https://www.kaggle.com/spscientist/students-performance-in-exams) 

### Steps:
1. Clone repository
2. Start Elastic Stack containers using:
- "docker-compose up -d" (use with "--build" while starting for the first time)
- or "docker swarm init" -> "docker stack deploy -c docker.stack.yml elk" (to run as a swarm)
![swarm](/images/swarm.png)
3. Create index pattern in Kibana for chosen index ("logs" or "datasets")
4. Analyze data in Discovery tab or create Dashboard with visualizations
![kibana_discover](/images/kibana_discover.png)
5. Open Jupyter Notebook -> http://localhost:8888/
