# Devops_Tools

# Table of contents

- [Devops_Tools](#devops_tools)
  - [Docker](#docker)
  - [Kubernetes](#kubernetes)
  - [Observability & Monitoring](#observability--monitoring)
    - [Observability :](#observability-)
    - [Monitoring:](#monitoring)
    - [Observability vs Monitoring](#observability-vs-monitoring)
    - [Logging:](#logging)

## Docker

## Kubernetes
In Kubernetes, **Persistent Volumes (PVs)** are used to provide a way for containers to retain data, even after the pod or container is deleted or recreated. Unlike regular volumes, which are ephemeral and tied to the lifecycle of a pod, persistent volumes exist beyond the lifespan of a single pod and allow data to persist across different pods.

#### Key Concepts in Persistent Volumes:

1. **Persistent Volume (PV):**  
   A Persistent Volume is a piece of storage in the cluster that has been provisioned by an administrator or dynamically provisioned using Storage Classes. It is independent of any pod's lifecycle.

2. **Persistent Volume Claim (PVC):**  
   A Persistent Volume Claim is a request for storage by a user. Pods use PVCs to access persistent storage. The PVC specifies how much storage is required and the access mode (e.g., ReadWriteOnce, ReadOnlyMany).

3. **Storage Classes:**  
   Storage Classes define different types of storage offered in a cluster (e.g., SSD, HDD). It helps in dynamically provisioning Persistent Volumes. When a PVC is created with a Storage Class, Kubernetes automatically provisions a PV that matches the requested storage class and size.

#### How Persistent Volumes Work:
1. **PV Creation:**  
   An admin can manually create a Persistent Volume by defining it in a YAML file, specifying the storage type (NFS, AWS EBS, etc.), capacity, and access modes.

2. **PVC Request:**  
   A user creates a PVC to request a certain amount of storage. Kubernetes will look for a matching PV (or dynamically create one) that satisfies the claim.

3. **Pod Binding:**  
   Once a PV is bound to a PVC, a pod can use that storage by specifying the PVC in its configuration. The pod can now access the data stored in the PV, and this data persists even if the pod is deleted or restarted.

4. **Access Modes:**
   - **ReadWriteOnce (RWO):** The volume can be mounted as read-write by a single node.
   - **ReadOnlyMany (ROX):** The volume can be mounted as read-only by multiple nodes.
   - **ReadWriteMany (RWX):** The volume can be mounted as read-write by many nodes simultaneously.

5. **Retain, Recycle, and Delete Policies:**
   - **Retain:** Keeps the data in the PV even after the PVC is deleted.
   - **Recycle:** Deletes the data but keeps the volume (usually just for testing).
   - **Delete:** Deletes both the data and the PV when the PVC is deleted.

### Example of Persistent Volume and Persistent Volume Claim:

**Persistent Volume (PV) YAML:**
```yaml
apiVersion: v1
kind: PersistentVolume
metadata:
  name: pv-storage
spec:
  capacity:
    storage: 1Gi
  accessModes:
    - ReadWriteOnce
  persistentVolumeReclaimPolicy: Retain
  nfs:
    path: /mnt/data
    server: 192.168.1.100
```

**Persistent Volume Claim (PVC) YAML:**
```yaml
apiVersion: v1
kind: PersistentVolumeClaim
metadata:
  name: pvc-storage
spec:
  accessModes:
    - ReadWriteOnce
  resources:
    requests:
      storage: 1Gi
```

**Pod YAML:**
```yaml
apiVersion: v1
kind: Pod
metadata:
  name: pod-using-pvc
spec:
  containers:
  - name: my-container
    image: nginx
    volumeMounts:
    - mountPath: "/usr/share/nginx/html"
      name: storage
  volumes:
  - name: storage
    persistentVolumeClaim:
      claimName: pvc-storage
```

In this example:
- The Persistent Volume (PV) is an NFS volume with 1GiB of storage.
- The Persistent Volume Claim (PVC) requests 1GiB of storage with `ReadWriteOnce` access.
- The pod then mounts the storage from the PVC into its container at the specified path.

### Use Cases for Persistent Volumes:
- **Databases:** Storing database files that need to persist across pod restarts.
- **File Storage:** Shared files that need to be accessed by multiple pods.
- **Backup and Restore:** Persistent storage for application data that is backed up or restored regularly.

### Dynamic Provisioning:
Kubernetes can dynamically provision PVs using a **StorageClass**. When a PVC requests a PV, Kubernetes will automatically create one that matches the requirements if there is no existing PV available.

**StorageClass YAML Example:**
```yaml
apiVersion: storage.k8s.io/v1
kind: StorageClass
metadata:
  name: fast
provisioner: kubernetes.io/aws-ebs
parameters:
  type: gp2
  zone: us-west-2a
```

By leveraging persistent volumes, Kubernetes enables stateful applications and ensures that data is not lost when pods or containers are rescheduled or restarted.
### Kubernetes Components:

### Helm:

### Ingress:
![image](https://github.com/user-attachments/assets/d1513f92-c74b-4a5f-8b62-86a2fd147c18)

### Service Mesh (Istio):

![image](https://github.com/user-attachments/assets/f8303a41-00e9-4050-aec7-26ce9814f003)
![image](https://github.com/user-attachments/assets/a1f36730-fdac-4f07-8f5d-1fb55fd1ef31)
![image](https://github.com/user-attachments/assets/f365fed2-9687-434c-a3a8-d50588ccc1ea)



![image](https://github.com/user-attachments/assets/68e84088-90f7-49ff-b388-c40aa2e7c4d2)
![image](https://github.com/user-attachments/assets/8edfcdb6-db6f-4299-847a-991eb86fcf0c)

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

![image](https://github.com/user-attachments/assets/db232440-3f09-4e38-9083-65cc228dba0b)

#### Metrics & monitoring with Spring Boot Actuator, Micrometer, Prometheus & Grafana
##### Metrics: 
- Metrics are numerical measurements of an application's performance, collected and aggregated at regular intervals. They can be used to monitor the application's health and performance, and to set alerts or notifications when thresholds are exceeded.
##### Actuator:
- Actuator is mainly used to expose operational information about the running application — health, metrics, info, dump, env, etc. It uses HTTP endpoints or JMX beans to enable us to interact with it.

##### Micrometer:
- Micrometer automatically exposes /actuator/metrics data into something your monitoring system can understand. All you need to do is include that vendor-specific micrometer dependency in your application. Think SLF4J, but for metrics.

##### Prometheus:
- The most common format for exporting metrics is the one used by Prometheus, which is "an open-source systems monitoring and alerting toolkit". Just as Loki aggregates and stores event logs, Prometheus does the same with metrics.

##### Grafana:
- Grafana is a visualization tool that can be used to create dashboards and charts from Prometheus data.

![image](https://github.com/user-attachments/assets/461fade0-a1eb-47c5-a9d5-19027e818d6c)

#### Distributed Tracing [Distributed tracing with OpenTeIemetry, Tempo & Grafana]
##### OpenTelemetry
- Usuing OpenTeIemetry generate traces and spans automatically. OpenTelemetry also known as OTel for short, is a vendor-neutral open-source Observability framework for instrumenting, generating, collecting, and exporting telemetry data such as traces, metrics,logs.
##### Tempo
- Index the tracing information using Grafana Tempo. Tempo is an open-source, highly scalable, and cost-effective distributed tracing backend designed for observability in cloud-native environments. It is a part of the Grafana observability stack and provides a dedicated solution for efficient storage, retrieval, and analysis of trace data.
##### Grafana
- Using Grafana, we can connect to Tempo as a datasource and see the distributed tracing in action with the help of visuals. We can integrate Loki and Tempo as well, so that we can jump to tracing details directly from logs inside Loki
![image](https://github.com/user-attachments/assets/a92b7687-2841-4a43-96af-c0da6379aab9)

















