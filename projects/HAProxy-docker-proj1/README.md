# HAProxy using Docker, Prometheus and Grafana

This app uses the _open source versions_ of the following tools:
- [Prometheus](https://prometheus.io/) as a metric aggregator.
- [Grafana](https://grafana.com/) for visualisation.
- [HA Proxy](https://www.haproxy.com/) as a reverse proxy.


## Prerequisites
 
- You'll need to have [Docker](https://docs.docker.com/engine/install/) installed. 

## How to start the app - Using Docker

## Create backend app. (this is only for validating or testing haproxy local)
docker container run --name app -p 8080:8080 -d -t -i spaceuptech/greeter
#check if 

## build image and Run HAProxy container
cd haproxy


