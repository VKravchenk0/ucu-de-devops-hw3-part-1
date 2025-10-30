```bash

minikube start --kubernetes-version=v1.32.0 

kubectl create namespace hw3-postgres-pgadmin
kubectl config set-context --current --namespace=hw3-postgres-pgadmin

kubectl apply -f . --recursive

sudo --preserve-env=HOME minikube tunnel
```

http://localhost