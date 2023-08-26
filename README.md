# Docker Compose
### Monitoring with 
- Grafana 10
- Prometheus 2.46
- Alertmanager 0.26
- Node-exporter 1.6.1
- Cadvisor 0.36
- Pushgateway 1.6.0
---
### Run
```
docker compose up -d
```
### Stop
```
docker compose down
```

---
### Steps Stack Monitoring
Access Grafana at http://localhost:3000 with User: admin and Password: admin
![Step 1](screens/1.png "Step 1")

Set a new password for the administrator
![Step 2](screens/2.png "Step 2")

Add new source data
![Step 3](screens/3.png "Step 3")

Select Prometheus data source
![Step 4](screens/4.png "Step 4")

Enter the http address (name) and port of the Prometheus service as configured in the docker-compose.yml file then click the Save and Test button
![Step 5](screens/5.png "Step 5")

Now add a new dashboard
![Step 6](screens/6.png "Step 6")

Add new visualization
![Step 7](screens/7.png "Step 7")

As an example let's add the source "-- Grafana --"
![Step 8](screens/8.png "Step 8")

You can get more information on how to create dashboard at: https://grafana.com/docs/grafana/latest/getting-started/build-first-dashboard/
![Step 9](screens/9.png "Step 9")

To access Phometheus just go to url http://localhost:9090
![Step 10](screens/10.png "Step 10")

To access Alertmanager just go to url http://localhost:9093
![Step 11](screens/11.png "Step 11")

To access Node-Exporter just go to url http://localhost:9100
![Step 12](screens/12.png "Step 12")

To access cAdvisor just go to url http://localhost:8080
![Step 13](screens/13.png "Step 13")

To access Pushgateway just go to url http://localhost:9091
![Step 14](screens/14.png "Step 14")

