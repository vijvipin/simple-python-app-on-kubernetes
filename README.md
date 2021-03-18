# hello-python
Very simple hello world python Flask application.

## Containerizing an application

### Create a Dockerfile

### Create an image

```
docker build -f Dockerfile -t hello-python:latest .

```
This will perform those seven steps listed in Dockerfile to create the image. To verify the image was created, run the following command:

```
docker image ls
```

### Running in Docker

Before jumping into Kubernetes, let’s verify it works in Docker. Run the following command to have Docker run the application in a container and map it to port 5001:

```
docker run -p 5001:5000 hello-python
```

Now lets jump to kubernetes. 

Go to folder /kubernetes. Here we have deployment.yaml

```
kubectl apply -f deployment.yaml
```

