# Kubernetes Client

There are several ways you can install kubernetes client `kubectl` you can find all documentation in [google cloud docs](https://kubernetes.io/docs/tasks/tools/install-kubectl/)

### Recommend

It is recommended to first install gcloud and then kubernetes. Also with gcloud install it will be easier to setup and install `kubectl` from [google cloud docs](https://kubernetes.io/docs/tasks/tools/install-kubectl/#download-as-part-of-the-google-cloud-sdk)

```bash
gcloud components install kubectl
```

### 1. Linux
##### Install using native package management 

 ```bash
sudo apt-get update && sudo apt-get install -y apt-transport-https gnupg2
curl -s https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -
echo "deb https://apt.kubernetes.io/ kubernetes-xenial main" | sudo tee -a /etc/apt/sources.list.d/kubernetes.list
sudo apt-get update
sudo apt-get install -y kubectl
``` 