# ArgoCD
### Login
```
kubectl port-forward svc/argocd-server -n argocd 8080:443
argocd admin initial-password -n argocd
export ARGOCD_OPTS='--port-forward-namespace argocd'
argocd login 127.0.0.1:8080
```

### Configuration
```
kubectl patch svc argocd-server -n argocd -p '{"spec": {"type": "LoadBalancer"}}'
```