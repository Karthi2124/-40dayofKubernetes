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
Frequently asked questions:
I've been overwhelmed by the fantastic response to my new YouTube series on the Certified Kubernetes Administrator (CKA) exam! But with all the excitement came some questions, and I'm here to address them head-on.

1) 𝐈 𝐜𝐚𝐧𝐧𝐨𝐭 𝐚𝐟𝐟𝐨𝐫𝐝 𝐭𝐡𝐞 𝐂𝐊𝐀 𝐞𝐱𝐚𝐦 𝐢𝐭'𝐬 𝐭𝐨𝐨 𝐞𝐱𝐩𝐞𝐧𝐬𝐢𝐯𝐞. 𝐒𝐡𝐨𝐮𝐥𝐝 𝐈 𝐬𝐭𝐢𝐥𝐥 𝐟𝐨𝐥𝐥𝐨𝐰 𝐚𝐥𝐨𝐧𝐠?
The content of this playlist is based on the exam curriculum because it provides a well-organized learning path. You don't have to worry about the roadmap; you can focus on learning. Even if you are not taking the exam now, you are still gaining the hands-on knowledge that a Kubernetes administrator should have; that's good enough!

𝟐) 𝐖𝐡𝐚𝐭 𝐚𝐫𝐞 𝐭𝐡𝐞 𝐩𝐫𝐞𝐫𝐞𝐪𝐮𝐢𝐬𝐢𝐭𝐞𝐬 𝐟𝐨𝐫 𝐭𝐡𝐢𝐬 𝐜𝐨𝐮𝐫𝐬𝐞?
The only prerequisites are basic Linux understanding; all the other prerequisites are already covered in this series. Check out the GitHub repo below for the course content. Yes, it is absolutely free for anyone to join and follow along.

𝟑) 𝐖𝐡𝐢𝐜𝐡 𝐂𝐥𝐨𝐮𝐝 𝐩𝐫𝐨𝐯𝐢𝐝𝐞𝐫 𝐚𝐫𝐞 𝐰𝐞 𝐮𝐬𝐢𝐧𝐠 𝐟𝐨𝐫 𝐭𝐡𝐞 𝐝𝐞𝐦𝐨?
We will not be using any Cloud as the focus is on Kubernetes. Using a cloud service would mean the cloud provider manages the control plane, limiting learning. We will use a local Kubernetes installation on a Kind cluster and a Kubeadm installation on virtual machines.

𝟒) 𝐀𝐫𝐞 𝐰𝐞 𝐝𝐨𝐢𝐧𝐠 𝐚𝐧𝐲 𝐫𝐞𝐚𝐥-𝐭𝐢𝐦𝐞 𝐩𝐫𝐨𝐣𝐞𝐜𝐭𝐬 𝐢𝐧 𝐭𝐡𝐢𝐬 𝐬𝐞𝐫𝐢𝐞𝐬?
Yes, there will be a couple of real-time projects at the end of this series. We cannot do real-time full-fledged projects in Kubernetes without completing all the essential topics. That is why I added the projects at the end and hands-on tasks in almost every video.

5) 𝐇𝐨𝐰 𝐦𝐚𝐧𝐲 𝐯𝐢𝐝𝐞𝐨𝐬 𝐰𝐢𝐥𝐥 𝐛𝐞 𝐩𝐮𝐛𝐥𝐢𝐬𝐡𝐞𝐝 𝐞𝐯𝐞𝐫𝐲 𝐰𝐞𝐞𝐤?
I have finished recording the entire series and am editing the last few videos. I plan to publish 3 to 4 weekly videos every Monday through Thursday. I have chosen not to publish daily so that viewers following the series have time to understand the concepts, practice hands-on, document their learning, and not feel left behind.

6) 𝐖𝐡𝐚𝐭 𝐢𝐟 𝐰𝐞 𝐚𝐫𝐞 𝐬𝐭𝐮𝐜𝐤 𝐬𝐨𝐦𝐞𝐰𝐡𝐞𝐫𝐞 𝐚𝐧𝐝 𝐧𝐞𝐞𝐝 𝐚𝐬𝐬𝐢𝐬𝐭𝐚𝐧𝐜𝐞?
You can comment on the video by providing complete details about the issue/query, or you can open a new thread in the discord channel of help-cka-2024, and someone will help you. I also plan to host a live Q&A session every weekend.
