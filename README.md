Kitchen App - Production Kubernetes Deployment

Overview
A Kitchen Orders application deployed on Kubernetes with full monitoring and CI/CD.

 Stack
- API: Node.js + Express + MongoDB
- Container: Docker
- Orchestration: Kubernetes (Docker Desktop)
- Monitoring: Prometheus + Grafana
- CI/CD: GitHub Actions

 Quick Start
```bash
kubectl apply -f k8s/namespace.yaml
kubectl apply -f k8s/db/statefulset.yaml
kubectl apply -f k8s/api/deployment.yaml
kubectl apply -f k8s/web-ui/deployment.yaml
kubectl apply -f k8s/monitoring/prometheus-config.yaml
kubectl apply -f k8s/monitoring/grafana-dashboard.yaml
kubectl apply -f k8s/monitoring/grafana-deployment.yaml
```

 Access
- API: http://localhost:30000
- Web UI: http://localhost:30080
- Prometheus: http://localhost:30090
- Grafana: http://localhost:30300 (admin/kitchenadmin)
