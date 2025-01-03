# Minikube

**Link for minikube cluster installation/management on local system**: https://minikube.sigs.k8s.io/docs/start/?arch=%2Flinux%2Fx86-64%2Fstable%2Fbinary+download

- You can create production ready cluster with **kubeadm**.
- But if you want to create cluster for developer or for testing application then you can create this with **minikube**. minikube will create cluster on **single vm/localmachine** etc.

for installing minikube on vm/local system follow above link..

remember: minikube ki installation sa phily apky ps vm/localsystem ma docker install hona chahye, or apka user docker group add hona chahye.. other wise error aye ga.. at the time of **minikube start**.

- Verify the minikube cluster once it get started with this command **minikube status**.
- You can also open kubernetes dashboard with command **minikube dashboard  or minikube dashboard --url**. One will open the dashboard directory or other will give you the dashboard url. Use this url to get the dashboard
- Also download **kubectl** with **minikube kubectl -- get po -A**
- for alaise **alias kubectl="minikube kubectl --"**
- for stopping the cluster **minikube stop**


## Manage your cluster
  
  Pause Kubernetes without impacting deployed applications:
  
  **minikube pause**

  Unpause a paused instance:
  
  **minikube unpause**
  
  Halt the cluster:
  
  **minikube stop**
  
 Change the default memory limit (requires a restart):
  
  **minikube config set memory 9001**
  
  Browse the catalog of easily installed Kubernetes services:
  
  **minikube addons list**
  
  Create a second cluster running an older Kubernetes release:
  
  **minikube start -p aged --kubernetes-version=v1.16.1**
  
  Delete all of the minikube clusters:
  
  **minikube delete --all**
  
 

