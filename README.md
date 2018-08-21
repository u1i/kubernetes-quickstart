kubectl run uhello --image=u1ih/hello --port=8080

kubectl expose deployment uhello --type=NodePort

minikube service uhello --url
