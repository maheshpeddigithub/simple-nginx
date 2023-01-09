Docker: <br>
------- <br>
docker build -t simple-nginx . <br>
docker tag simple-nginx cloudmahesh/simple-nginx:tag1 <br>
docker push cloudmahesh/simple-nginx:tag1<br>

Minikube: <br>
--------- <br>
minikube start <br>
minikube tunnel <br>

K8S: <br>
---- <br>
kubectl get nodes <br>
kubectl create deployment simple-nginx --image=cloudmahesh/simple-nginx:tag1 <br>
kubectl get deployments <br>
kubectl expose deployment simple-nginx --type LoadBalancer --port 80 --target-port 80 <br>
kubectl get pods <br>
kubectl get service simple-nginx <br>
kubectl get services <br>

K8S-Manifast: <br>
------------- <br>
kubectl apply -f k8s-simple-nginx.yml <br>