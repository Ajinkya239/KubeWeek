# Kubernetes Architecture and Components
## Overview
 - Kubernetes is a powerful, open-source platform designed for automating the deployment, scaling, and management of containerized applications. This repository provides detailed information and resources about Kubernetes architecture and its core components, offering a comprehensive guide to understanding how Kubernetes works and how its components interact.

## Introduction
- Kubernetes is a container orchestration platform that simplifies the deployment, scaling, and management of containerized applications. It is designed to manage clusters of containers across multiple hosts, providing high availability and scalability.

## Architecture Overview
- Kubernetes architecture is composed of several key components that work together to manage containerized applications. The architecture is divided into two main types of nodes: Master Nodes and Worker Nodes.
<img width="1147" alt="Kubernet architechture.JPG" src="https://github.com/Ajinkya239/KubeWeek/blob/main/Kubernet%20architechture.JPG">


## Master Node Components
1. **API Server**:  The API server is the front-end for the Kubernetes control plane. It exposes the Kubernetes API and serves as the gateway for all API requests.
2. **Controller Manager**: The controller manager runs controllers that regulate the state of the cluster, ensuring that the desired state matches the actual state.
3. **Scheduler**: The scheduler is responsible for assigning pods to available nodes based on resource requirements and constraints.
4. **etcd**: etcd is a distributed key-value store that holds the configuration data and state of the Kubernetes cluster.
5. **Cloud Controller Manager**: The cloud controller manager interacts with the cloud provider to manage resources such as load balancers and storage volumes.

## Worker Node Components
1. **Kubelet**: The kubelet is an agent that runs on each worker node. It ensures that containers are running as expected by managing pod lifecycles.
2. **Kube-Proxy**: Kube-proxy maintains network rules on each node to allow for communication between pods and services.
3. **Container Runtime**: The container runtime is responsible for running containers. Examples include Docker, containerd, and CRI-O.
4. **Cluster Networking**: Kubernetes networking provides the ability to communicate between pods and services across the cluster.

