# Online-Banking-WebApp-Kubernetes

Deployed a simple web application for an online banking system alongside a MongoDB database in a Kubernetes cluster.
- **Web Application:** An online banking webapp containerized with Docker, using the image `nolita26/online-banking-app:v1.0`, accessible externally via `banking.mybankingapp.com`.
- **MongoDB Database:** Deployed as a container with credentials managed through Secrets.
- **Configuration Management:** Used ConfigMaps for non-sensitive configuration and Secrets for sensitive data like database credentials and application secrets.
- **Networking:** Exposed the web application through a Kubernetes Service of type LoadBalancer and configured an Ingress resource to handle external traffic and route it to the application.

##### Start Minikube and check status
    minikube start --vm-driver=hyperkit 
    minikube status

##### Get minikube node's ip address
    minikube ip

##### Get basic info about k8s components
    kubectl get node
    kubectl get pod
    kubectl get svc
    kubectl get all

##### Get extended info about components
    kubectl get pod -o wide
    kubectl get node -o wide

##### Get detailed info about a specific component
    kubectl describe svc {svc-name}
    kubectl describe pod {pod-name}

##### Get application logs
    kubectl logs {pod-name}
    
##### Stop your Minikube cluster
    minikube stop
