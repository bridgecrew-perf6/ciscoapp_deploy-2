# ciscoapp_deploy

## deploy.yaml

```
kubectl apply -f .
sleep 1
kubectl get deployments -n mbarbhui-ns
sleep 2 
kubectl get podd,svc,ingress -n mbarbhui-ns
```
