# Kubernetes-Interview-Questions
(1) What is the difference between Docker and Kubernetes?

Ans: Docker is a container platform where as Kubernetes is a container orchestration environment that offers capabilities like Auto Scaling, Auto healing, Clustering and Enterprise level support like Load Balancing.

(2) What are the main components of Kubernetes architecture?

Ans: On a broad level, you can divide the kubernetes components in two parts.

(i) Control Plane (API Server, Scheduler, Controll Manager, C-CM, etcd)

(ii) Data Plane (Kubelet, Kube-proxy, Container Runtime)

(3) What are the main difference between the Docker Swarm and Kubernetes?

Ans: Kubernetes is better suited for large organizations as it offers more scalability, networking capabilities like policies and huge third party ecosystem support.

(4) What is the difference between Docker Container and a Kubernetes pod?

Ans: A pod in kubernetes is a runtime specification of a container in docker. A Pod provides more declarative way of defining using YAML and you can run more than one container in a pod.

(5) What is a namespace in Kubernetes?

Ans: In Kubernetes namespace is a logical isolation of resources, network policies, rbac and everything. For example, there are two projects using same k8s cluster. One project can use namespace1 and other project can use namespace2 without and overlap and authentication problems.

(6) What is the role of kube proxy?

Ans: Kube-proxy works by maintaining a set of network rules on each node in the cluster, which are updated dynamically as services are added or removed. When a client sends a request to a service, the request is intercepted by kube-proxy on the node where it was received. Kube-proxy then looks up the destination endpoint for the service and routes the request accordingly.

Kube-proxy is an essential component of a kubernetes cluster, as it ensures that services can communicate with each other.

(7) What are the different types of services within Kubernetes?

Ans: There are three different types of services that a user  can create.

(1) Cluster IP Mode

(2) Node Port Mode

(3) Load Balancer Mode


(8) What is the difference between NodePort and LoadBalancer type service?

Ans: When a service is created a NodePort type, the kube-proxy updates the IPtables with node IP address and port that is choosen in the service configuration to access the pods.

Where as if you create a Service as type LoadBalancer, the cloud control manager creates a external load balancer IP using the underlying cloud provider logic in the C-CM. Users can access servicesusing the external IP.

(9) What is the role of Kubelet?

Ans: Kubelet manages the containers that are scheduled to run on that node. It ensures that the containersare running and healthy, and that the resources they need are avaible.

Kubelet communicates with the Kubernetes API server to get information about the containers that should be running on the node, and then starts and stops the containers as needed to maintain the desired state. It also monitors the containers to ensure that they are running correctly, and restarts them if necessary.

(10) Day to Day activities on Kubernetes?
