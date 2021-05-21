```
kubectl create secret generic secret-appsettings --from-file=./appsettings.secrets.json

kubectl create -f deployment.yaml

kubectl expose deployment hello-node --type=LoadBalancer --port=8080

```