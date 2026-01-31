# deploying-wordpess-and-mysql-using-PV
# Wordpress and mysql on Kubernetes(Microk8s) using PV 
This project demostrate deploying a stateful Wordpress application on Kubernetes using:
## Components 
Kubernetes Deployments
Services (ClustreIP)
PersistentVolumeClaims
Secrets for credentials 
Nginx Ingress Controller 
## Architecture 
User -> Wordpres service -> Wordpress Pod -> Mysql service -> Mysql Pod 
## Steps to Deploy 
```bash
kubectl apply -f secret.yaml
kubectl apply -f mysql-deployment.yaml
kubectl apply -f wordpress-deployment.yaml
kubectl apply -f ingress.yaml 
