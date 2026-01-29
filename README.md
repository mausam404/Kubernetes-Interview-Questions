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
Ans:
