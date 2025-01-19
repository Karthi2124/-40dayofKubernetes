# Kubernetes Overview

Kubernetes is an open-source platform for automating the deployment, scaling, and management of containerized applications. Developed by Google engineers in 2014 and now maintained by the Cloud Native Computing Foundation (CNCF), Kubernetes helps manage workloads in containers across multiple environments.

It automates tasks such as deploying applications, scaling them based on need, and providing self-healing capabilities. Kubernetes ensures portability and extensibility for workloads, load balancing, and efficient resource allocation.

## Table of Contents

1. [What is Kubernetes?](#what-is-kubernetes)
2. [Kubernetes Architecture](#kubernetes-architecture)
3. [Control Plane Components](#control-plane-components)
4. [Node Components](#node-components)
5. [Add-ons and Plugins](#addons-and-plugins)
6. [Kubernetes Commands](#kubernetes-commands)

## What is Kubernetes?

Kubernetes, often referred to as **k8s** (where 8 stands for the number of letters between "K" and "s"), is a powerful tool that automates the deployment and scaling of containerized applications. It provides the following features:

- **Automation**: Automates deployment, scaling, and management.
- **Portability**: Ensures workloads are portable.
- **Scalability**: Scales applications based on demand.
- **Extensibility**: Supports extensible architecture for more advanced applications.
- **Load Balancing**: Efficiently balances loads across applications.
- **Resource Allocation**: Monitors and allocates resources.
- **Self-Healing**: Allows applications to recover from failures.

## Kubernetes Architecture

Kubernetes operates on a **client-server** architecture, consisting of two main components:

1. **Control Plane**: Manages the overall health and state of the cluster.
2. **Worker Nodes**: These nodes run the applications inside containers.

The master node, also known as the control plane, contains components like the API server, controller manager, scheduler, and etcd database. The worker nodes run the kubelet and kube-proxy processes that manage and schedule pods.

### Key Components of Kubernetes

#### 1. **Control Plane Components**
   - **Kube-API Server**: Serves as the initial gateway for all requests to the cluster. It validates and processes requests, then forwards them to the appropriate services.
   - **Kube-Scheduler**: Decides where to place newly created pods based on resource availability.
   - **Kube-Controller-Manager**: Manages controllers that handle replication, node states, and more.
   - **etcd**: A key-value store for managing the cluster's configuration and state information.

#### 2. **Node Components**
   - **Container Runtime**: Runs containers in pods. For example, Docker.
   - **kubelet**: Ensures containers are running and are in the desired state.
   - **kube-proxy**: Manages network routing and forwards requests to the appropriate pods.

## Add-ons and Plugins

Kubernetes supports the use of add-ons that enhance its functionality. These add-ons are typically deployed in the `kube-system` namespace and provide additional features such as DNS, networking, and more.

### Key Add-ons:
   - **CoreDNS**: Provides DNS services to Kubernetes clusters.
   - **KubeVirt**: Runs virtual machines alongside containers, providing unified management.
   - **Calico**: Provides network policy enforcement and advanced routing capabilities.

## Kubernetes Commands

Here are some of the key commands used to interact with Kubernetes:

- **kubectl get pods**: Lists all pods in the cluster.
- **kubectl create -f pod.yaml**: Creates a pod from the specified YAML file.
- **kubectl scale deployment app-name --replicas=3**: Scales the application to the desired number of replicas.
- **kubectl delete -f pod.yaml**: Deletes a pod from the cluster.

## Conclusion

Kubernetes is a powerful and flexible platform for managing containerized applications at scale. Its modular architecture, along with its automation and self-healing capabilities, makes it a go-to solution for modern cloud-native applications.
