## Create a Pod and pull nginx image

```bash
 kubectl create deployment my-nginx --image=nginx:latest
 ```

## Check deployed application

```bash
kubectl get deployments
```

## Check Pod status

```bash
kubectl get pods
```

## Run dashboard 

```bash
minikube dashboard
```

## Expose out application to outside world

```bash
kubectl expose deployment my-nginx --port=80 --type=LoadBalancer
```

## Check

```bash
kubectl get services
```

## Tell minikube about this

```bash
minikube service my-nginx
```