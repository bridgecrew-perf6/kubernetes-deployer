## Create DockerHub credential

```
kubectl --kubeconfig=D:\VKE\test.yaml create secret docker-registry dockerhub-registry --docker-username=<USERNAME> --docker-password=<PASSWORD> --docker-email=<EMAIL>
```

## Build and push to DockerHub

```
docker build . -t <YOUR_DOCKER_HUB_ID>/app-name
docker tag app-name <YOUR_DOCKER_HUB_ID>/app-name:latest
docker push <YOUR_DOCKER_HUB_ID>/app-name:latest
```
