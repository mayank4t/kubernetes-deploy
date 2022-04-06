# testgcp-kubernetes-deploy

Kubernetes Deployment configuration steps
Update deployment.yaml file for externIP with the IP of your loadbalancer :- externalIPs:
  - 34.131.22.182

Jenkins file :- credential required for git, Docker and config file for Kubernetes
Plugins :- kubernetes

download token from master

gcloud compute ssh --zone "asia-south2-a" "master"  --project "kubernetestestmayank" --command "sudo cat /etc/kubernetes/admin.conf" > admin.conf
