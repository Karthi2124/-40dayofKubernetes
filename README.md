Day 1: Docker Fundamentals
What is Docker?
How is it different from Virtual Machines
Docker Architecture
Docker flow
Docker commands

Day 2 : Dockerize an application
What is Dockerfile, and how do you write it?
docker pull , push, tag etc

Day3 : Docker Multi-Stage Builds
How to write a dockerfile for multistage build
Benefits of multi-stage builds
Other docker best practices

Day 4 : Why do We need Kubernetes?

Day 5 : Kubernetes Architecture
Control plane VS Worker Nodes
Overview of control plane components

Day 6 : Install Kubernetes Cluster locally
Install Kind cluster locally
How to access the cluster

Day7 : Pods in Kubernetes
What are pods in Kubernetes?
Containers VS Pods
Imperative VS Declarative way for creating Kubernetes resources
Create a sample pod using the imperative way
Create a sample pod using the declarative way
Inspect the pods

Day8 : Replicasets and Deployments in Kubernetes:
Replication Controller
ReplicaSet
Deployments
How to perform Rolling updates/rollback
Scale the deployment

Day9 : Services in Kubernetes:
What are services in Kubernetes, and why do we need them?
Node port, ClusterIP, and LoadBalancer

Day 10 : Namespaces:
NameSpaces
Services and namespaces

Day 11 : Multi-container Pods
What are multi-container pods
Multi-container pods pattern - sidecar/init etc
Environment variables in Kubernetes

Day 12 : Daemonset, Cronjob, and job
What are Daemonset, cronjobs and Jobs
Cron fundamentals with examples

Day13 : Static Pods
What are static pods
Labels and selectors
Manual Scheduling

Day14 : Taints and Tolerations

Day15 : Node Affinity

Day16 : Resource Requests and Limits

Day17 : Autoscaling in Kubernetes
Horizontal VS Vertical Autoscaling
HPA, VPA, Cluster autoscaling, NAP
Metrics server

Day18 : Probes in Kubernetes
Liveness VS Readiness Probes
HTTP/TCP/Command-based health checks

Day19 : Config maps and Secrets
concept and demo

Day 20 : How SSL/TLS works
Symmetric VS Asymmetric encryption
SSL certificates and Certificate Authority

Day 21 : TLS in Kubernetes
How TLS works in Kubernetes
Why we need TLS in Kubernetes
Private key and public certificates

Day 22 : Authorization in Kubernetes
Authorization VS Authentication
Authorization types, ABAC, RBAC, Node, Webhook
Kubeconfig

Day 23 : Role-based access control (RBAC)
Role and role binding
Generate and approve the certificate
grant access to the user

Day 24 : Cluster role and cluster role binding
concept and demo

Day 25 : Service Account
What are service accounts, and why do we use them?
Create a service account and grant access to it

Day26 : Network Policies
Network policy concept
CNI installation
enforce network policy by creating the object

Day27 : Use Kubeadm to install a Kubernetes cluster
Provision underlying infrastructure to deploy a Kubernetes cluster
Setup Master Node to deploy Kubernetes components
Setup multiple worker nodes and join the master node

Day28 : Docker storage fundamentals
Why do we need storage in docker containers
persistent docker storage

Day29 : Storage in Kubernetes
How storage works in Kubernetes
hostpath volumes in Kubernetes
Persistent volumes and Persistent volume claims
Volume modes, Access modes, and reclaim policies for volumes
Storage classes and provisions

Day30 : How does DNS work?
What happens when you type a website address in your browser
different components involved in DNS
End-to-end flow
Important files and resources

Day31 : DNS in kubernetes
How DNS works in Kubernetes
Core-DNS

Day32 : Kubernetes Networking
CNI , Network Add-on
Containerd vs runc , container runtime

Day 33 : Ingress controller and Ingress resources

Day 34 : Perform a version upgrade on a Kubernetes cluster using Kubeadm

Day 35 : Implement etcd backup and restore

Day 36 : Monitoring, Logging and Alerting
Monitor Cluster components, Evaluate cluster and node logging
Understand how to monitor applications, metric server
Manage container stdout & stderr logs

Day 37 : Troubleshoot application failure

Day 38 : Troubleshoot cluster component failure

Day 39 : Network Troubleshooting
Worker node failure
cordon, uncordon and drain (maintenance)\
Day 40 : JSONPath, advance kubectl commands
JSON for beginners
JSON v/s YAML
JSONPATH basics
Multiple JSONPATH queries to fetch details
Day 41 Mission CKA
Exam Pattern
Pre-requisites
Last-minute preparation
Tips and Tricks
Sample questions
Day 42 : Realtime project: Host your own container registry on Kubernetes
This project will include multiple Kubernetes topics with real-time implementation.
