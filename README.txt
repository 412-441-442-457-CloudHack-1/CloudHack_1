to execute this :
-- Install Docker
-- Enable Kubernetes
-- Install minikube (do through administrator mode)
-- Enable hardware virtualization (if not enabled)
-- Enable HYPER-V if demanded by minikube

Executing (commands in administrator mode in cmd):
-- minikube start driver=docker (ensure kubernetes , minikube is running)
-- minikube status (verify minikube is running) 
-- minikube ip (gives you the ip)
-- kubectl apply -f mongo-config.yaml (deploying pod)
-- kubectl apply -f mongo-secret.yaml 
-- kubectl apply -f mongo.yaml 
-- kubectl apply -f webapp.yaml
   (Ensure all are running by command : kubectl get all)
-- kubectl get pods (See all the running pods)

Open Browser :
in address bar type
minikube_ip_obtained_above:30100

-- Here 30100 referes to port number through which its accessible