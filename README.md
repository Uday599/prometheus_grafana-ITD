
# Prometheus and Grafana
This is a collection of configuration files for docker compose stacks for Prometheus, node-exporter, CAdvisor, AlertManager and Grafana.
It becomes handy when you want to run a stack of docker containers and you don't want to run many command.

# Installation

### 1. Install Docker
```bash
curl -s https://raw.githubusercontent.com/jaintpharsha/install/main/docker | sudo bash
```
### 2. Clone Prometheus-grafana setup repo 
```bash
git clone https://github.com/harshaprakash100/prometheus_grafana.git && cd ./prometheus_grafana
```

### 3. Run promethes grafana CAdvisor alertmanager node-exporter
```bash    
docker compose up -d 
```
### 4. Add new scrap_configs in prometheus/prometheus.yml
   Restart the prometheus container to apply new scrap configurations

## Demo

**To access Prometheus Dashboard:** <public_ip>:9090
    
**To check all the prometheus scraps targets:** <public_ip>:9090/targets 
    
**To access Grafana Dashboard:** <public_ip>:3000 <br/>
  **Note:** username and password configuration file: grafana/config.monitoring
