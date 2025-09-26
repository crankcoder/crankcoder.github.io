# Minkube

## Installation
[Official documentation](https://minikube.sigs.k8s.io/docs/start/?arch=%2Fwindows%2Fx86-64%2Fstable%2F.exe+download)

### Hyper-V 
[How to use hyperv with minikube](https://minikube.sigs.k8s.io/docs/drivers/hyperv/)


## Commands
[Minikube command reference](https://minikube.sigs.k8s.io/docs/commands/)

### Start cluster
```bash
minikube start
# or
minikube start --memory=16384 --cpus=4 --kubernetes-version=v1.26.1
```

### Stop cluster
```bash
minikube stop
```

### Delete clusters
```bash
minikube delete --all --purge
```