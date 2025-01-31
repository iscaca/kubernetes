# kubernetes
kubectl create deployment --image=nginx nginx --replicas=4 --dry-run=client -o yaml > nginx-deployment.yaml

# Namespaces
kubectl get pods --namespace=prod
kubectl get pods --all-namespaces
# Swith Namespace
kubectl config set-context $(kubectl config current-context) --namespace=dev
When we run kubectl get pods, we will see the pods under dev namespace