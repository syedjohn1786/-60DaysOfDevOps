

1. In Docker, the applications are deployed as containers. But in Kubernetes, the applications are deployed in containers as Pods.

2. The basic difference is, In Docker we run commands through command-line whereas in Kubernetes we run through YAML files.

3. A Pod may contain single container or multiple containers.

4. By placing multiple containers in a single pod, the advantage we get is the containers can communicate each other over a shared network, use shared storage.

Containers within a pod can communicate with each other using localhost, as they share the same network namespace.

5. IP Addresses are allocated for the Pods (which are known as Cluster IP Address) through which we can access the applications inside the pods.

Note : Kubeproxy is responsible for giving IP addresses.

6. In Docker to run commands we use "DockerCLI"
   In Kubernetes, we use "kubectl"

7. Kubectl is command line tool for Kubernetes.


Installation of Kubectl and Minikube for Kubernetes practice on Windows
================================================================================

1. Install kubectl, minikube
2. Put in one folder and paste that folder path in Environment variables section of Windows.
3. check whether kubectl is installed properly by running command "kubectl version"
4. check whether minikube is installed properly by running command "minikube start"

Commands i came across
===============================

1. kubectl get nodes => used to list the nodes
2. kubectl get pods => used to list the pods
3. Kubectl create -f <yaml file_name> => used for creating pods
4. kubectl get pods -o wide => which is used for getting full information of pods
5. kubectl delete pod <pod_name> => used for deleting pod
6. kubectl logs <pod_name> => used to get logs of the pod
7. Kubectl describe pod <pod_name> => used to get full details about pod (we can use this command to debug a pod so that we get information like status of pod , if any error in the pod etc)

