# Widgetario Kubernetes Hackathon Project

## 📦 Overview

This project demonstrates the deployment of a multi-component application called *Widgetario* on Kubernetes. It covers essential Kubernetes concepts such as Deployments, Services, ConfigMaps, Secrets, Ephemeral and Persistent Storage using `emptyDir` and StatefulSets.

This submission includes **Parts 1 to 5** of the lab work.

---

## 🗂️ Repository Structure

All YAML files are placed at the root level and named clearly to indicate their role:

| File                           | Purpose                                      |
|--------------------------------|----------------------------------------------|
| `products-api-deployment.yaml` | Deploy the products API (Spring Boot)        |
| `products-api-service.yaml`    | Service for products API                     |
| `stock-api-deployment.yaml`    | Deploy the stock API (Go service)            |
| `stock-api-service.yaml`       | Service for stock API                        |
| `web-deployment.yaml`          | Deploy the web UI (.NET Core)                |
| `web-service.yaml`             | Service for web frontend                     |
| `products-db-deployment.yaml`  | Initial products DB deployment               |
| `products-db-service.yaml`     | Service for products DB                      |
| `products-db-statefulset.yaml` | StatefulSet for persistent DB setup          |
| `postgres-statefulset.yaml`    | Alternative or main PostgreSQL StatefulSet   |
| `postgres-pvc.yaml`            | PersistentVolumeClaim for DB storage         |
| `products-api-config.yaml`     | ConfigMap for the products API               |
| `products-api-secret.yaml`     | Secret for DB credentials                    |
| `api.json`                     | Sample API data (if needed)                  |

---

## 🎯 Project Objectives

- Deploy multi-service apps using Kubernetes              
- Use Services for inter-component communication                             
- Apply ConfigMaps and Secrets for secure configuration                             
- Implement `emptyDir` (ephemeral) and PVC-based storage for persistence              
- Replace stateless DB deployments with StatefulSets
- Build resilience using replicas and readiness/liveness probes

---

## 🔧 Setup Instructions

### Prerequisites

- Docker
- Kubernetes cluster (e.g., Minikube, kind, Docker Desktop, etc.)
- `kubectl` CLI installed and configured

---

### 🚀 Run the Project

1. **Clone the repository**:

   ```bash
   git clone https://github.com/itsonlytinega/Hackathon_assignment.git
   cd Hackathon_assignment
