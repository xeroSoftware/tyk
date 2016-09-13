GIT CLONE OF https://github.com/quorak/tykio-kubernetes-deployment

# tykio-kubernetes-deployment


Kubernetes Pod and Service description to quickly deploy tyk.io on your Cluster. 
Its using the official tyk.io docker containers and the config files from conf/ .
Clone this repo and edit you conf files

´´´´
kubectl create -f k8s/tykio-kubernetes-deployment/tyk-deployment.yaml --namespace=prod
kubectl create -f k8s/tykio-kubernetes-deployment/tyk-service.yaml --namespace=prod
kubectl create -f k8s/tykio-kubernetes-deployment/tyk-volume.yaml --namespace=prod
´´´´
