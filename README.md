![Docker Automated build](https://img.shields.io/docker/automated/aishwaryasarath/pythonk8s?style=plastic)
# Deploy python app to Kuberbetes demo
A Simple python flask hello world app containerization and orchestration demo.

## Requirements
```python
pip install flask
```

## Docker build
```docker
docker build -t pythonk8s .
docker run -p 5003:5003 pythonk8s

```

## Docker-compose Build & Push
```docker-compose
docker-compose up
docker-compose push

```

## Deploy the app in Kubernetes
```Kubernetes deployment 
kubectl apply -f kubernetes/deployment/deployment.yaml
kubectl get deploy
kubectl get pods
```
```enable network traffic, expose and loadbalancing
kubectl apply -f kubernetes/services/service.yaml
kubectl get svc

```

## Validate application
```
browse live application exposed through a load balancer http://localhost:8080
```
