Commands for Application deploy in K8s:
1. How to get nodes information?
 
>kubectl get nodes
 

2. How to get pods information?
 
>kubectl get pods
 
3. How to get deployment information?
 
>kubectl get deployments
or 
>kubectl get deploy
 
4. How to svc information?
 
>kubectl get svc
 
5. How to create a namespace?
 
Syn:
 
>kubectl create namespace <namespace name>
 
Ex:
 
>kubectl create namespace ingress-nginx
 
6. Deploy through raw path?
 
>kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.2.1/deploy/static/provider/cloud/deploy.yaml
 
7. Get all the information about the namespace?
 
>kubectl get all -n ingress-nginx
 
8. How to deploy your application using yaml file?
 
Syn:
 
>kubectl apply -f <path of yaml file>
 
Ex:
 
>kubectl apply -f .\dep_1.yml
 
9. How to deploy igress resource?
 
>kubectl apply -f ingress_resource.yml
 
10. How to check ingress resources?
 
>kubectl get ingress