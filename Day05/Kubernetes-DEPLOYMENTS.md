Kubernetes Deployment
================================

1. If you can deploy your application on kubernetes as pod, then why we need kubernetes deployment ?
2. First let us learn the difference between Container ||  Pod 
3. Container : generaaly to run a container on docker we use the command line and run the following command => Docker run -it <image>
4. Pod : In Kubernetes pods, instead of running commands we use manifest files called yaml files which contains image name, container port, volume specifications etc. So you can think like pod yaml files are just running specification of a docker container.

So Why we are going for Kubernetes Deployment
===============================================

1. The most important reason why we are moving from docker to kubernetes is "Auto Scaling" and "Auto Healing"
2. Pod do not have the capacity to handle Auto Scaling and Auto Healing. You can think pod like a docker container in simple terms.
3. These kind of things can be done in kubernetes by deployment. Therefore we need to deploy our applications on kubernetes as deployment but not as a pod.


How Auto-Healing done in Kubernetes Deployment (in simple terms)
===================================================================
1. When you write yaml manifest file of kind : deployment, internally what happens is firstly it will create ReplicaSet which is a kubernetes Controller. Next is the ReplicaSet(which is a Kubernetes Controller) rollout the pods (based on count of replicas. if replicas : 2, it will rollout 2 pods).

2. Now we have 2 pods. If anyone deletes 1 pod accidentally, then also Kubernetes ensures there are 2 pods. This is because we written a kubernetes deployment manifest and configured replicas : 2 , Replication controller always ensures there are 2 pods running. This is also known as "Auto-Healing".

End process
=================

Deployment Manifest => ReplicaSet => pods

commands i came across
================================

1. kubectl get deploy  =>  which lists the no of deployments
2. kubectl get rs  => which lists the replica sets
3. kubectl get pods -w  => w stands for watch, this command is used to watch the process of pods creation, deletion and lifecycle of    pods.
4. 

