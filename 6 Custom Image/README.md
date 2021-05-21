
# Build and Run

```bash
docker build -t helloflask .
docker run -p 9000:5000 --name mikescoolapp -t helloflask 
```
---

# Create a repository
[Create Repository](https://cloud.docker.com/repository/create)

---
# push local image to repository
```sh
docker login

docker tag helloflask [☢️️name of registry☢️]:v1
docker push [☢️️name of registry☢️]:v1
```


# Create a repository
[Create Repository](https://cloud.docker.com/repository/create)

---
# push local image to repository
```sh
docker login

docker tag helloflask microshak/helloflask:v1
docker push microshak/helloflask:v1
```
---

# Deploy from repository
```bash
kubectl create deployment helloflask --image=helloflask microshak/helloflask:v1

kubectl expose deployment helloflask --type=LoadBalancer --port=8080

kubectl get services
```