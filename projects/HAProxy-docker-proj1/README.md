# HAProxy using Docker, Prometheus and Grafana

This app uses the _open source versions_ of the following tools:
- [Prometheus](https://prometheus.io/) as a metric aggregator.
- [Grafana](https://grafana.com/) for visualisation.
- [HA Proxy](https://www.haproxy.com/) as a reverse proxy.


## Prerequisites
 
- You'll need to have [Docker](https://docs.docker.com/engine/install/) installed. This project uses `docker-compose` to bring the backend components up.

## How to start the app

- Clone this repo and `cd` into the cloned directory.
- Simply run `docker-compose -p monitoring up -d` to bring up the monitoring stack along with the services to be monitored. 
- Once all the containers are up, Open `http://IP_ADDRESS:3000` in a browser window to load Grafana.
- Add a Prometheus data source. The Prometheus url is `http://prometheus:9090`. Hit `Save & Test` to add the data source
- Import the dashboard by uploading the `grafana-dashbord-haproxy.json` file.
- URLs:
Prometheus `http://IP_ADDRESS:11000`
Grafana: `http://IP_ADDRESS:3000`
