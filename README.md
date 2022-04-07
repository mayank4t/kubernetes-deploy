****#Simple kubernetes deployment ****

This is a simple Python-based code to print time.

This code is used to test Jenkins with Kubernetes (Service and Deployment)

Pipeline steps:- Git Clone, build Docker image, Push docker image to Hub, and Deploy to Kubernetes using hub image.

Docker File:- Python version 3.7 with flask

Prerequisite:- 

Update deployment.yaml for external Ip for loadbalancer,

Jenkins file:- credential required for git, Docker, and Kubernetes 

Install Plugin for Jenkins:- Kubernetes

download admin.conf from master using below command, to cloudshell for the Jenkins connection with the K8 :- 
gcloud compute ssh --zone "asia-south2-a" "master" --project "kubernetestestmayank" --command "sudo cat /etc/kubernetes/admin.conf" > admin.conf
