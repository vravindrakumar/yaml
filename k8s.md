1.Kubernets Cluster :
    -Set of Worker machines (Nodes)
	
2.Master Node (Control plane):
    -API server (server the kubernets API)
	
	-ectd ( A Distributed key-value store)
	
	-Controller Manager (Runs Controller Processes)
	
	-Scheduler (Assings Workloads to Nodes)
	

3.Worker Node:
 
   -Kubelet  (Primary agent on each mode)
   
   -kube-proxy (Network Proxy)
   
   -Container Run time (Responsible  for Running containers)
   -Docker 
   -Containerd
   -CRI-O
   
4.Additional Components:
   -Pods :The smallest deployable units in Kubernets
   
   
   -ReplicateSets:Ensure a specified nuumber of pods replicas are running at any
    one time

   Deployments :

   services:

   ConfigMaps and secrets:   
  