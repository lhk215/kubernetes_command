# Kubernetes Commands

## Basic Commands
- `kubectl get node` : list nodes
- `kubectl get pods` : list all pods in default namespace
- `kubectl get pods --all-namespaces` : list all running pods across all the namspaces
- `kubectl get namespace` : list all configured namespaces
- `kubectl get nodes -o=wide` : list details on nodes
- `kubectl get service` : list all services

## Deployment Commands
- `kubectl create deployment --image nginxdemos/hello web1`
- `kubectl describe deploy web1`
- `kubectl scale deployment --replicas 20 web1`
- `kubectl expose deployment web1 --port=80 --type=LoadBalancer`
- `minikube service web1`
- `kubectl get deploy web1 -o=yaml`
- `kubectl delete deployment web1`
- `kubectl run nginx --image=nginx`
- `kubectl apply -f`
