#Deploy Local K8s cluster through minikube on vagrant cloud

# Pre-Requiste #

#Setup linux ubuntu OS on vagrant cloud
>vagrant up

>vagrant ssh

#Created Kubertness Architecture of 2cpu shown in Vagrantfile

#Install Docker

# Cluster Creation #

#Step 1: Install Minikube

>curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 

>sudo install minikube-linux-amd64 /usr/local/bin/minikube

#Step 2: Start the Minikube cluster
>minikube start

#Step 3: Install Kubectl
>sudo snap install kubectl --classic

#Step 4: Verify the minikube pods running

>minikube kubectl -- get pods -A

#Step 5: Pull the Nginx Image

>docker pull nginx:latest

#Step 6: Create, deploy & expose Deployment application of Nginx Server

>vim deployment.yaml

>kubectl apply -f deployment.yaml 

>kubectl expose deployment deployment --type=NodePort

#Step 7: Verify the Pods and services of the application status

>kubectl get pods 

>kubectl get services

#Step 8: Check the minikube arctitecture is created and running before access the application

>minikube start

>minikube stop

Troubleshoot if there any unexpected error occure while controlplane restoration or running check 

The Nodeport will be checked through -kubectl get services command

The Minikube IP will be find through -minikube ip  command

#Step 9: Access the application by

> curl -L Minikube-ip:Nodeport   ,

Replace the minikube-ip and nodeport as defined in particular architecture.

![Screenshot 2024-03-27 175231](https://github.com/Rajil101/Accuknox/assets/86475883/1d9bba66-0790-4ffd-98a6-8ba971915a14)


# Git Integration #

#Install the git 

>sudo apt-get install git -y 

>git remote add origin https://github.com/Rajil101/DE-Task.git

>git branch -M main

>git push origin main

The authentication will be done through access token.



 
