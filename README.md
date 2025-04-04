# Device monitoring stack
This project is meant to help you monitor your devices within your network (router, switch, any other device with SNMP protocol) with a simple setup configuration and easy maintainability using top tier technologies, such as Docker, Grafana, Prometheus and a minimal Go app.

This stack is meant to be used within a private network and a limited access server.

# Getting started
In order to start this project, simply fill in the .env.example files, add switch data in the csv file provided, then create a specific external network (in some cloud servers, if you dont create an external network, it may cause problems with your ssh connection):
docker network create switch-monitoring-network

Finally, run:
docker compose up --build -d

To stop the project, simply run:
docker compose down

# Stack architecture
