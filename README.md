 ./install.sh

gcloud init

gcloud auth list

gcloud config list

docker run busybox date

docker build -t simple-nginx .

gcloud auth configure-docker

docker tag simple-nginx eu.gcr.io/ssil1-258911/simple-nginx:tag1

docker push eu.gcr.io/ssil1-258911/simple-nginx:tag1

gcloud components install kubectl

gcloud container clusters create --machine-type n1-standard-2 --num-nodes 2  --zone europe-west2-b --cluster-version latest test-cluster

kubectl get nodes

kubectl create deployment simple-nginx --image=eu.gcr.io/ssil1-258911/simple-nginx:tag1

kubectl get deployments

kubectl expose deployment simple-nginx --type LoadBalancer --port 80 --target-port 80

kubectl get pods

kubectl get service simple-nginx

kubectl get services

kubectl apply -f k8s-simple-nginx.yml