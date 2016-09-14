GIT CLONE OF https://github.com/quorak/tykio-kubernetes-deployment

# tykio-kubernetes-deployment


Kubernetes Pod and Service description to quickly deploy tyk.io on your Cluster. 
Its using the official tyk.io docker containers and the config files from conf/ .
Clone this repo and edit you conf files

´´´´
kubectl create -f tyk-deployment.yaml --namespace=prod
kubectl create -f tyk-service.yaml --namespace=prod
kubectl create -f tyk-volume.yaml --namespace=prod
´´´´

Use setup.sh
remplace 130.211.71.127 by the ip of external service

and 
test

curl -H "Authorization: null" http://130.211.71.127:8080/hotelpro4u-api/

curl -H "Authorization: null" http://130.211.71.127:8080/test-api/get