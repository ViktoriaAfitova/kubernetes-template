# React application using Kubernetes

## Commands to know

### Installation 

- [minikube start](https://minikube.sigs.k8s.io/docs/start/?arch=%2Fmacos%2Fx86-64%2Fstable%2Fbinary+download)

- [kubectl](https://kubernetes.io/docs/tasks/tools/)

### Start your cluster

```shell
minikube start
```

```shell
kubectl
```

```shell
kubectl cluster-info
```

```shell
kubectl get nodes
```

```shell
kubectl get pod
```

```shell
kubectl get service
```

or

```shell
kubectl get svc
```

```shell
kubectl get deployment
```

or

```shell
kubectl get deploy
```

```shell
kubectl get pod --all-namespaces
```

```shell
kubectl get svc --all-namespaces
```

```shell
kubectl get deploy --all-namespaces
```

```shell
kubectl get namespace
```

### Create pod just for study

```shell
kubectl run nginx-pod --image=nginx:latest --port=80
```

```shell
kubectl expose pod nginx-pod --type=NodePort --port=80
```

```shell
minikube service nginx-pod
```

### Deleting

```shell
kubectl delete pod/nginx-pod
```

```shell
kubectl delete svc/nginx-pod
```

### Manifest file (create pod, service)

- /cd manifest

```shell
kubectl apply -f nginx-pod.yaml
```

```shell
kubectl apply -f nginx-service.yaml
```

```shell
minikube service nginx-service
```

### Stop your cluster

```shell
minikube stop
```
