# How To

## Prerequisites
1. AKS Cluster
2. Lens (Because I like it)

## Docker Build
> docker build -t ytimocin/go-hello-world:latest .

## Docker Run
> docker run -d -p 8080:8080 ytimocin/go-hello-world:latest
> docker run -it --rm -p 3000:8080 ytimocinacr.azurecr.io/ytimocin/go-hello-world

## Docker Tag (docker and acr login needed)
> docker tag ytimocin/go-hello-world ytimocinacr.azurecr.io/ytimocin/go-hello-world

## ACR Push (docker and acr login needed)
> docker push ytimocinacr.azurecr.io/ytimocin/go-hello-world:latest

## Deploy to Kubernetes
> kubectl apply -f deployment.yaml

## Link to the Deployed Application
http://20.88.166.53/