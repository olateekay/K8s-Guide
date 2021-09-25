## Kubernetes – The Beginners guide to orchestration

In this article we will be looking at the some of the basic concepts of Kubernetes, the Kubernetes architecture, problems Kubernetes solve and the tasks of an orchestration tool.

Learning Kubernetes is not a walk in the park, it can be overwhelming at first however this guide will show how to get up and running with Kubernetes as soon as possible.

### TABLE OF CONTENTS

-	What is Kubernetes?
-	Prerequisites
-	Key Kubernetes concept
-	Kubernetes Architecture 
-	Conclusion
-	Further reading

### WHAT IS KUBERNETES?
Kubernetes is an Open-source orchestration framework that aims to manage containers. It automates the deployment, scaling and management of containerized applications in different environments like physical machines, virtual machines, or cloud environments.
The purpose of Kubernetes is to host our containers in an automated way so that we can easily deploy as many instances of our application as required and easily enable communication between different services within our application. With Kubernetes, there is scalability , greater fault tolerance and also decoupling of resources which is very important in production environment.

### PREREQUISITES
Before starting with Kubernetes, an in depth knowledge of a container technology like Docker is required.


### KEY KUBERNETES CONCEPTS

**CONTAINER:** A container is an isolated unit that houses a software component and its environment, dependencies, and configuration. It is a form of operating system virtualization.

**NODE:** A Node is a worker machine in Kubernetes and may be either a virtual or a physical machine, depending on the cluster. It is the host that the container runs on.

**POD:** A pod is a single instance of an application. It consists of one or more containers which share an IP address, access to storage and namespace.

**REPLICASET:** A replicaSet helps to run multiple instances of a single pod in the Kubernetes cluster thus providing high availability. It ensures that a specified number of pods are running at any given time.

**DEPLOYMENT:** A Deployment provides the capability to upgrade instances using rolling updates

**SERVICE:** This is an abstract way to expose an application running on a set of Pods as a network service. Services enables communication between various components within and outside the application. There are 3 types of available services ;

-	NodePort
-	ClusterIp
-	LoadBalancer

**NB:**  The Kubernetes resources are created in a declarative way, thus making use of YAML files. Kubernetes resources, such as pods, services, and deployments are created by using the YAML files


### KUBERNETES ARCHITECTURE
Here's the diagram of a Kubernetes cluster with all the components tied together.

![k8s diagram](https://github.com/olateekay/K8s-Guide/blob/main/k8s-arc.png)
 


**These steps illustrate the basic Kubernetes process.**

-	An administrator creates and places the desired state of an application into a YAML file.
-	The file is provided to the Kubernetes API Server using a CLI or UI. Kubernetes’ default command-line tool is called kubectl.
-	Kubernetes stores the file (an application’s desired state) in a database called the Key-Value Store (etcd).
-	Kubernetes then implements the desired state on all the relevant applications within the cluster.
-	Kubernetes continuously monitors the elements of the cluster to make sure the current state of the application does not vary from the desired state.

### CONCLUSION
“Kubernetes – The Beginners Guide to Orchestration”, gives you have an overview on some concepts you need to understand when starting off with Kubernetes.
Kubernetes is the King of Container Orchestration, It’s the clear choice for managing modern container deployments in an efficient, flexible, and business-friendly way.



**FURTHER READING**

https://www.freecodecamp.org/news/

https://the-kubernetes-handbook/

https://kubernetes.io/docs/home/
