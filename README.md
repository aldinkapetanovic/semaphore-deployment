# semaphore

## docker
```sh
docker compose up -d
```


## k8s
```sh
kubectl create -f semaphore-postgres-persistentvolumeclaim.yaml
kubectl create -f postgres-deployment.yaml
kubectl create -f semaphore-deployment.yaml
kubectl create -f semaphore-service.yaml
```

```sh
kubectl port-forward -n semaphore svc/semaphore 3000:3000
```

## access

http://localhost:3000

``admin:changeme``