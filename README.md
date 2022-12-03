# K8S-Final-Task

Create an ingress that directs the traffic to the correct service:
  -  One that represent Bitcoin Price
  -  Second one that represents Ynet news

First We had to Dockerize previous homeworks and push the images into DockerHub

![alt text](https://github.com/Samer99Najjar/K8S-FinalTask/blob/main/dockerhubimg.PNG)

# Run Locally

## Clone the project

 > git clone https://github.com/Samer99Najjar/K8S-FinalTask.git
  
## Go to the project directory

 > cd K8S-FinalTask
  
## Apply the yml Files 

 > kubectl apply -f .

## Check if all the servers are running

> kubectl get po,svc

You should get similar status to that of mine :

![alt text](https://github.com/Samer99Najjar/K8S-FinalTask/blob/main/runningimg.PNG)

## Deploy enginx
> minikube start

> minikube addons enable ingress

> minikube tunnel
 
## Open Ynet LocalHost 
> localhost/ynet

![alt text](https://github.com/Samer99Najjar/K8S-FinalTask/blob/main/pic1k8stask.PNG)

> localhost/bitcoin

![alt text](https://github.com/Samer99Najjar/K8S-FinalTask/blob/main/pick2k8stask.PNG)
