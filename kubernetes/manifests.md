# Kubernetes Manifests

### Manifests?
Manifest is a description that Kubernetes API Server can read and execute instructions. 
Kubernetes manifests are the instructions set of creating, modifying and deleting resources such 
Mainly manifests are in form of `.yaml` files and can be sent to the Kubernetes API Server. 

Example of Manifest
```yml
apiVersion: apps/v1 ## Kubernetes Api Version
kind: Deployment ## Kind of the Manifest
spec:
  replicas: 3 ## Number of instances
    spec:
      containers:
      - name: simple-server ## Name of the Deployment
        image: jmalloc/echo-server ## Docker images name
        ports:
        - containerPort: 80 ## Port-forwarding from inside the dokcer 
```

To send a manifest to the Kubernetes API, execute this command 
```bash
 kubectl apply -f my-file.yaml -n holokube
```
