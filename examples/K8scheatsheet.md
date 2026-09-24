After deployment.yaml

run cmd
kubectl apply -f deployment.yml
kubectl get pods
kubectl get pods -o wide
kubectl get pods -v=9 # is the maximum verbose point

kubectl delete pod sample-python-app-345359353
kubectl get pods

minikube ssh

kubectl apply -f service.yaml
kubectl get svc -v=9

how to get node ip
minikube ip
curl -L http://192.168.64.10:30007/demo

kubectl edit svc python-django-sample-app


 




