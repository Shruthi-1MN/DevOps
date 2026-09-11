

Architecture

Docker has container runtime which is supported by only dockershim
docker has docker engine/docker shim to run containers

Kubernetes 
Pod - smallest level deployment , wraper over your container with advance capabilities
Kubelet - runs pods  like docker engine 



workflow


Master Node - Request always go through Master called Control Plane
On worker - Kublet run container runtime which is supported by containerd, cri-o, dockershim, any other container run time implements.

Networking
Docker default network is bridge network, here 
Kuberenetes is managed by Kube-proxy, it ensure every container gets IP address. Load balancing capabilities is done. It uses IP tables in the machine(Linux).

Worker Node components
1 Kubelet
2 Kube-Proxy
3 container run time

Master
API Server - 
Scheduler
Etcd
controllers
cloud controller manager

Cons
* Cluster
* Healing
* Scaling
* Enterprise support




