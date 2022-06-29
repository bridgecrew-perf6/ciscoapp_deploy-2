# ciscoapp_deploy

## deploy.yaml

```
kubectl apply -f .
sleep 1
kubectl get deployments -n mbarbhui-ns
sleep 2 
kubectl get podd,svc,ingress -n mbarbhui-ns

## apply autoscale in mbarbhui-ns
# appling autoscaling 
kubectl  autoscale  deployment  mbarbhui-cisco-app --min=3 --max=10 --cpu-percent 70 -n mbarbhui-ns
sleep 1

kubectl get hpa -n mbarbhui-ns
```
