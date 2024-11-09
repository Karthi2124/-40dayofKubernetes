# What is Kubernetes #

    Kubernetes is an open-source platform that helps manage, deploy, and scale containerized applications: 

    Automation: Kubernetes automates tasks like deploying applications, scaling, and monitoring. 

Portability: Kubernetes makes workloads portable. 
Scalability: Kubernetes allows applications to scale up or down to meet changing needs. 
Extensibility: Kubernetes helps build more extensible applications. 
Load balancing: Kubernetes incorporates load balancing. 
Resource allocation: Kubernetes tracks resource allocation. 
Self-healing: Kubernetes enables apps to self-heal. 

What is Kubernetes and How It Works - Quobyte
Kubernetes is often called "k8s" or "k-eights", where the 8 stands for the number of letters between the “K” and the “s”. The word "Kubernetes" comes from ancient Greek and means "helmsman" or "pilot". 
Kubernetes was developed by Google engineers in 2014 and is now managed by the Cloud Native Computing Foundation (CNCF). It's widely adopted by companies of all sizes, including half of the Fortune 100. 

# Kubernetes – Architecture #

Kubernetes Cluster mainly consists of Worker Machines called Nodes and a Control Plane. In a cluster, there is at least one worker node. The Kubectl CLI communicates with the Control Plane and the Control Plane manages the Worker Nodes. In this article, we are going to discuss in detail the architecture of Kubernetes.

## Table of Content ##

    Kubernetes – Cluster Architecture
    Kubernetes Components
    Control Plane Components
    Node Components
    Addons Plug-in
    Commands for Kubectl

Kubernetes – Cluster Architecture

Kubernetes comes with a client-server architecture. It consists of master and worker nodes, with the master being installed on a single Linux system and the nodes on many Linux workstations. The master node, contains the components such as API Server, controller manager, scheduler, and etcd database for stage storage. kubelet to communicate with the master, the kube-proxy for networking, and a container runtime such as Docker to manage containers.
Kubernetes Components

Kubernetes is composed of a number of components, each of which plays a specific role in the overall system. These components can be divided into two categories:

    nodes: Each Kubernetes cluster requires at least one worker node, which is a collection of worker machines that make up the nodes where our container will be deployed.
    Control plane: The worker nodes and any pods contained within them will be under the control plane. 

Kubernetes Architecture

Kubernetes automates the deployment and management of containerized applications. To dive deeper into Kubernetes architecture and its role in DevOps, the DevOps Engineering – Planning to Production course provides a comprehensive guide to setting up and managing Kubernetes clusters.
Control Plane Components

It is basically a collection of various components that help us in managing the overall health of a cluster.  For example, if you want to set up new pods, destroy pods, scale pods, etc. Basically, 4 services run on Control Plane:
1. Kube-API server

The API server is a component of the Kubernetes control plane that exposes the Kubernetes API. It is like an initial gateway to the cluster that listens to updates or queries via CLI like Kubectl. Kubectl communicates with API Server to inform what needs to be done like creating pods or deleting pods etc. It also works as a gatekeeper. It generally validates requests received and then forwards them to other processes. No request can be directly passed to the cluster, it has to be passed through the API Server.
2. Kube-Scheduler

When API Server receives a request for Scheduling Pods then the request is passed on to the Scheduler. It intelligently decides on which node to schedule the pod for better efficiency of the cluster.
3. Kube-Controller-Manager

The kube-controller-manager is responsible for running the controllers that handle the various aspects of the cluster’s control loop. These controllers include the replication controller, which ensures that the desired number of replicas of a given application is running, and the node controller, which ensures that nodes are correctly marked as “ready” or “not ready” based on their current state.
4. etcd 

It is a key-value store of a Cluster. The Cluster State Changes get stored in the etcd. It acts as the Cluster brain because it tells the Scheduler and other processes about which resources are available and about cluster state changes.
Node Components

These are the nodes where the actual work happens. Each Node can have multiple pods and pods have containers running inside them. There are 3 processes in every Node that are used to Schedule and manage those pods.

The following are the some of the components related to Node:
1. Container runtime
   A container runtime is needed to run the application containers running on pods inside a pod. Example-> Docker

2. kubelet
   kubelet interacts with both the container runtime as well as the Node. It is the process responsible for starting a pod with a container inside.

3. kube-proxy
   It is the process responsible for forwarding the request from Services to the pods. It has intelligent logic to forward the request to the right pod in the worker node.
Node Components
Addons Plug-in

Kubernetes add-ons are plug-ins that enhance the cluster’s functionality, often installed as Kubernetes resources like DaemonSets, Deployments, and more. These add-ons are typically deployed within the kube-system namespace, providing cluster-level capabilities and extending the native features of Kubernetes.
Key Add-ons

    CoreDNS: A flexible, extensible DNS server that provides name resolution services for Kubernetes clusters, ensuring efficient service discovery and network routing.
    KubeVirt: Allows the running of virtual machines alongside containers, providing a unified management platform for both VMs and containerized applications.
    ACI (Application Containerization Interface): Facilitates the integration and management of containers across different environments, improving the portability and scalability of applications.
    Calico: A network policy engine that provides secure, high-performance networking for Kubernetes clusters, supporting both network policy enforcement and advanced routing capabilities.

