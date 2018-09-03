minikube config set memory 12288

minikube config set disk-size 50GB

minikube start

kubectl cluster-info

kubectl run uhello --image=u1ih/hello --port=8080

kubectl expose deployment uhello --type=NodePort

minikube service uhello --url

kubectl scale deployments/uhello --replicas=4

kubectl autoscale deployment uhello --min=2 --max=10 --cpu-percent=80

minikube dashboard --- http://localhost:30000/


