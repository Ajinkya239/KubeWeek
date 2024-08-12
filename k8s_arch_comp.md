# Kubernetes Architecture and Components
## Overview
 - Kubernetes is a powerful, open-source platform designed for automating the deployment, scaling, and management of containerized applications. This repository provides detailed information and resources about Kubernetes architecture and its core components, offering a comprehensive guide to understanding how Kubernetes works and how its components interact.

## Introduction
- Kubernetes is a container orchestration platform that simplifies the deployment, scaling, and management of containerized applications. It is designed to manage clusters of containers across multiple hosts, providing high availability and scalability.

## Architecture Overview
- Kubernetes architecture is composed of several key components that work together to manage containerized applications. The architecture is divided into two main types of nodes: Master Nodes and Worker Nodes.
<img width="1147" alt="Kubernet architechture.JPG" src="https://github.com/Ajinkya239/KubeWeek/blob/main/Kubernet%20architechture.JPG">


## Master Node Components
1. **API Server**:  Acts like the main gatekeeper for the cluster. It listens for requests to manage the cluster (like adding or updating applications) and makes sure everything is running smoothly by talking to other components.
   
2. **etcd**: A special storage system. Think of it as a big notebook where Kubernetes keeps all the important information about your cluster, like what apps are running and where they are.
   
3. **Scheduler**: Decides which computer (node) should run new applications. When you have new apps or services to run, the scheduler figures out the best computer to run them based on what’s available and what the apps need.
   
4. **Controller Manager**: Makes sure everything is working as expected. It checks that the apps and services are running correctly and fixes any issues, like starting new instances if some fail or ensuring the right number of copies are running.
   
5. **Cloud Controller Manager**: Handles cloud-specific tasks. If your cluster is running in a cloud service (like AWS or Google Cloud), this component takes care of things related to the cloud, such as managing virtual machines and network settings.
   

## Worker Node Components
1. **Kubelet**: Manages the containers (apps) on each node. It ensures that the containers (apps) are running on the nodes and makes sure they are behaving as they should.
   
2. **Kube-Proxy**: Manages network connections. It handles the network traffic to ensure that requests to your services get to the right place.
   
3. **POD**: A pod is like a box that holds one or more containers. Containers are like small packages that run your applications. These containers share the same network namespace and storage, so they can easily communicate with each other and share data.


