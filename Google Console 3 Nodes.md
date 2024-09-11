1. Create cluster in GCP console with 3 nodes
 
2. Connect cluster using Google Cloud SDK shell with cluster address
 
3. To check the number of nodes in the cluster 
>kubectl get nodes
 
4. To check the number of pods in the cluster 
>kubectl get nodes
 
5. To check the number of deployments in the cluster 
>kubectl get deploy
or
>kubectl get deployments
 
6. To check the number of services in the cluster
>kubectl get svc
 
7. Create namespace
>kubectl create namespace ingress-nginx
 
8. Create nginx ingress controller
>kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.2.1/deploy/static/provider/cloud/deploy.yaml
 
9. To get nginx ingress controller full details
>kubectl get all -n ingress-nginx
 
10. Navigate to your yml file directory path in Google Cloud SDK shell/ Powerhsell
 
11. Before create pod,application deployments and services run below commands to check already present or not
 
>kubctl get pods
>kubctl get deploy
>kubctl get svc
 
12. Deploy nginx application using below command
>kubctl apply -f .\<deployment yml file name>
 
To Verify deployment is success or not run below commands
>kubctl get pods
>kubctl get deploy
>kubctl get svc
 
13. Deploy httpd application using below command
>kubctl apply -f .\<deployment yml file name>
 
To Verify deployment is success or not run below commands
>kubctl get pods
>kubctl get deploy
>kubctl get svc
 
14. Deploy ingress resources 
>kubctl apply -f .\<deployment yml file name>
 
To Verify deployment is success or not run below commands
>kubectl get ingress
 
Note: Wait for couple of minutes and check same command to get IP address of app-ingress
 
15. Check application is able to access with help of app-ingress IP address/<application name>
 
Ex:
http://35.225.132.189/nginx
http://35.225.132.189/httpd


http://35.232.24.118/nginx