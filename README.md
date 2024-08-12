# Online-Banking-WebApp-Kubernetes

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
