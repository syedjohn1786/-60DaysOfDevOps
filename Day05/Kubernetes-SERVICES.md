Kubernetes Services
======================================

1. Consider you given replicas : 3 in your deployment yaml manifest file. So there will be total of 3 pods.
2. Suppose due to some reason pod1(which has ip address : a.b.c.d) goes down. As we know kubernetes has "Auto-Healing" capacity, so even before the pod1 goes down a new pod is getting created in background. Condider this newly created pod as pod1_new.
3. We know that pod1_new comes in place of pod1, but if other teams use the same ip address of pod1 to access the application it wont work. The reason is pod1_new has different ip address(w.x.y.z) and your application is now available in pod1_new. So you need to use pod1_new ip address to access the application. (As other teams wont know that pod1 is down, they still use the ip address of pod1)


4. All this confusion is due to change of IP Adresses. So what kubernetes offers is to create a Service on top of deployment.
5. This service acts as a Load Balancer and it uses a component in kubernetes called "kube-proxy".
6. So we can ask/advice other teams to access the application through service name instead of accessing through IP address.

This is the main problem if we dont have "Services" in kubernetes.

7. Service doesnt keep track of IP addresses but it tracks "Labels & Selectors". So service identifies the pods with the help of Labels because Labels of the pods wont change even the Pods goes down or ip addresses of the pods changes.

This mechanism is called as "Service Discovery" which uses the concept of Labels & Selectors.

8. Generally as of now, we used the IP address of the pod to access the application. But we cant tell user to login to kubernetes cluster and ssh into ip address of pod and access the application. we cant tell like that right.

9. So , what Service offers is to expose the application to outside world i.e allow kubernetes cluster to outside world.

10. So how can service expose the application to outside world ?

While creating Service YAML Manifest file, service can be created mainly of 3 types

A) Cluster IP
B) Node Port
C) Load Balancer

11. Cluster IP type : this is the default service type and your application will be accessible inside the kubernetes cluster only (nothing beneficial , it will be like same)

12. Node Port type : this service type allows the application accessible to only yhr teams inside your organization.(they will have access to worker nodes)

13. Load Balancer type : this service type allows the application accessible to outside world. 