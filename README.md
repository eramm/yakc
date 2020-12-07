# yakc

## Yet Another Kubernetes Course

High level concepts
1. Why you need Kubernetes and what can it do ?
2. What Kubernetes is not? ( emphasize HA misconceptions)
3. Where do containers fit in with this ?
4. Do they need to be microservices ?
5. How do monolith’s work on Kubernetes ?
* Kubernetes Architecture

**concepts

-High Availability

-Failover

**Describe the elements that make up the control plane

-kube-apiserver

-ii. kube-controller-manager

-iii. kube-scheduler

-ETCD

-cloud manager


**Node processes

-Kublet

-Kube-proxy

-docker


**K8s networking concepts

-Port forwarding
-Networks
-Firewalls

**Kubernetes Objects

-(scheme)
-Pod
 -- resources
 -- limits
 -- requests
 -- labels (metadata
 -- ports
 -- annotations
 -- affinity
-Service
 -- Cluster ip
 -- Node port
 -- Load balancer
 -- External name
-Volumes
 -- init container
  --persistant storage 
-Namespace
-secrets
-K8S Volumes
-Ingress / (api Gw /reverse proxy )
-Deployment
-DaemonSet
-StatefulSet
-ReplicaSet / replication controller
-config map
-Job
-Networking
-Difference between pod and replica
-(security ) RBAC/ABAC
-K8S StateLess and Stateful applications
-Working with the various certificates and understanding them

**Troubleshooting

-Troubleshoot application failure
-Troubleshoot control plane failure
-Troubleshoot worker node failure
-Troubleshoot networking
-See what’s running and who is talking to who
-Understanding my cluster from an OS level

**Logging / Monitoring

-Understand how to monitor all cluster components
-Understand how to monitor applications
-Manage cluster component logs
-Manage application logs

**Working and installing K8s with Kubespray

-Understand what Kubespray is doing behind the scenes
-What problems does Kubespray solve and what do you need to still take care of ?
-Install K8s with Kubespray
-Install a simple app (NGINX with Hello world page) that takes advantage of K8s

**Using Kubectl

-Getting around with Kubectl / managing multiple configs
-Getting info about my cluster / app with Kubectl
-Starting / stopping pods from the cli
-Understanding resource usage in K8s what should I look for
-Discovering namespaces and switching between them
-What info should you have before you ask for help and how to get it

**Installing Helm

-why do we need helm
-hat is helm and its parts
-Building our first Chart
-Deploying charts
-Museum

**Command commands from Ignite that the Ignite team asked that Support be familiar with:

kubectl version
kubectl apply
kubectl create
kubectl top
kubectl cordon
kubectl drain
kubectl cp
kubectl cluster-info
kubectl exec
kubectl api-resources (for being familiar with all the cluster resources and what kind of resources
coupled to namespaces and the opposite )
kubectl edit
kubectl delete
kubectl logs
kubectl get ( po / ds / sts / ing / deploy / svc / no / csinodes / csidrivers / sc / pvc / pv / jobs / ev / hpa /
roles / clusterroles / clusterrolebindings / cm / ns / ep / crd / cj / sa )
kubectl describe ( po / ds / sts / ing / deploy / svc / no / csinodes / csidrivers / sc / pvc / pv / jobs / ev /
hpa / roles / clusterroles / clusterrolebindings / cm / ns / ep / crd / cj / sa )
