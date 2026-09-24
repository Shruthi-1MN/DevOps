1. What is the difference docker and kubernetes?
   Docker is a container platform where as k8 is a container orchestration env that offeres capabilities like auto healing, auto scaling, clustering and enterprose level support like load balancing
   
 2. What are the main components of k8s architecture?
 On a broad level, you can divide the k8 components in two parts
 * Control Plane(API Server, Scheduler, Controller Manager, CCM, ETCD)
   * Data Plane(Kubelet, Kube-proxy, Container Runtime)

3. what are the main difference Docker swarm and Kubernetes?
 K8s is better suited for large organizations as it offers more scalability, networking capabilities like policies and huge third party ecosystem support.

4. what is the difference between docker container and a k8s pod?
    A pod in kuberentes is a runtime specification of a container more declarative way of defining using YAML and you can run more than one container in a pod

5. what is a namespace in k8s?
In k8s namespace is a logical isolation of resources, network policies, rbac and everything. For ex, there are two projects can use ns1 and other project can use ns2 without any overlap and authentication problems

6. what is the role of kube proxy?
 Kube-proxy works by maintaining a set of network rules on each node in the cluster, which
 are updated dynamically as services are added or removed. When a client sends a req to service,
 the request is intercepted by kube-proxy on the node where it was received. Kube-proxy then looks
 up the destination endpoint for hte service and routes the request accordingly.

Kube-proxy is an essential component of a k8s cluster, as it ensures that services can
communicate with each other.

7. What are the difference types of services within K8s?
  There are 3 different types of service that a user can create
  1. Cluster IP Mode
  2. Node PortMode
  3. Load Balancer Mode
8. What is the difference between NodePort and LoadBalancer type Service?
  When a service is created a Nodeport type, the kube-proxy updates the IP Tables with
Node IP address and port that is chosen in the service configuration to access the pods
Where as if you create a service as type loadbalancer, he cloud control manager creates
a external load balancer IP using the underlying cloud provider logic in the C-CM.
Users can access services using the external IP.

9. What is the roleof Kubelet?
  Kubelet manages the containers that are scheduled to run on that node, IT ensures that the
containers are running and healthy, and that the resources they need are available.

Kubelet communicates with the K8s API server to get information about the containers that
should be running on the node, and then starts and stops the containers as needed to
maintain the desired state. It also monitors the containers to ensure that they
are running correctly and restarts them if necessary.

10. Day to Day activities on K8s?
    
12. 
13. 
 
