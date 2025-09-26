# Istio
### Install
```
istioctl install --set profile=demo

# Install Kubernetes API Gateway CRD
kubectl get crd gateways.gateway.networking.k8s.io &> /dev/null || \
{ kubectl kustomize "github.com/kubernetes-sigs/gateway-api/config/crd?ref=v1.2.0" | kubectl apply -f -; }

```
### Uninstall
```
kubectl delete -f samples/addons
istioctl uninstall -y --purge
kubectl delete namespace istio-system

```

### links
* [Istio API Reference](https://istio.io/latest/docs/reference/config/)
* [Virtual Service API Ref](https://istio.io/latest/docs/reference/config/networking/virtual-service/)
* [Destination Rule API Ref](https://istio.io/latest/docs/reference/config/networking/destination-rule/)
* [Service Entry API Ref](https://istio.io/latest/docs/reference/config/networking/service-entry/)
* [Sidecar API Ref](https://istio.io/latest/docs/reference/config/networking/sidecar/)