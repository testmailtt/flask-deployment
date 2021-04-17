# Steps for full deployment
```
kubectl apply -f .\pods\pods.yaml
kubectl apply -f .\services\services.yaml
kubectl get all
kubectl exec api -- python manage.py create_db
```

# Deploy pods

```
kubectl apply -f .\pods\pods.yaml
```

# Deploy services

```
kubectl apply -f .\services\services.yaml
```

# Get pods

```
kubectl get pods
```

# Get services

```
kubectl get services
```

# Get all 

```
kubectl get all
```


# Exec in a pod

```
kubectl -it exec api sh
```


# Describe pod

```
kubectl decribe pod api
```

# Minikube ip

```
minikube ip
```

# kubectl delete

```
kubectl delete --all pods
kubectl delete --all services
```


# Migrate db
```
kubectl exec api -- python manage.py create_db
```