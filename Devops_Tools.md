# Devops_Tools

## Docker

## Kubernetes

## Observability & Monitoring
### Observability : 
- Observability is the ability to understand the internal state of a system by observing its outputs. In the context of microservices, observability is achieved by collecting and analyzing data from a variety of sources, such as metrics, logs, and traces.
The three pillars of observability are:
  - Metrics: Metrics are quantitative measurements of the health  of a system. They can be used to track things like CPU usage, memory usage, and response times.
  - Logs: Logs are a record of events that occur in a system. They can be used to track things like errors, exceptions, and other unexpected events.
  - Traces: Traces are a record of the path that a request takes through a system. They can be used to track the performance of a request and to identify bottlenecks.
### Monitoring:
- Monitoring in microservices involves checking the telemetry data available for the application and defining alerts for known failure states. This process collects and analyzes data from a system to identify and troubleshoot
problems, as well as track the health of individual microservices and the overall health of the microservices network.

### Observability vs Monitoring
![image](https://github.com/user-attachments/assets/18d79f2c-8db9-4b05-a10f-1b235388c9f9)
In other words, monitoring is about collecting data and observability is about understanding data. Monitory is reacting to problems while observavility is fixing them in real time.

### Logging: 
- Logs are discrete records of events that happen in software applications over time. They contain a timestamp that indicates when the
event happened, as well as information about the event and its context. This information can be used to answer questions like "What
happened at this time?" "Which thread was processing the event?" or "Which user/tenant was in the context?"

#### Grafana, Loki & Promtail
##### Grafana : 
- Grafana is an open-source analytics and interactive visualization web application. It provides charts,graphs, and alerts for the web when connected to supported data sources. It can be easily installed using Docker or Docker Compose.
Grafana is a popular tool for visualizing metrics, logs, and traces from a variety of sources. It is used by organizations of all sizes to monitor their applications and infrastructure.
##### Loki :
- Grafana Loki is a horizontally scalable, highly available, and cost-effective log aggregation system. It is designed to be easy to use and to scale to meet the
needs of even the most demanding applications.
##### Promtail
- Promtail is a lightweight log agent that ships logs from your containers to Loki. It is easy to configure and can be used to collect logs from a wide variety of sources.
- Together, Grafana Loki and Promtail provide a powerful logging solution that can help you to understand and troubleshoot your applications.
- Grafana provides visualization of the log lines captured within Loki.
