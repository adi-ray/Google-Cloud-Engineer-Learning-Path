## Quiz Questions

#### Q1. When configuring storage for stateful applications, what steps must you take to provide file system storage inside your containers for data from your applications that will not be lost or deleted if your Pods fail or are deleted for any reason?

- [ ] You must create Volumes using local Storage on the Nodes and mount the Volumes inside your containers to provide durable storage.
- [ ] You must export the data from your applications to a remote service that preserves your data.
- [ ] You must mount NFS Volumes on each container in the Pod that requires durable storage.
- [x] You must create Volumes using network based storage to provide durable storage remote to the Pods and specify these in the Pods.


#### Q2. You need to ensure that the production applications running on your Kubernetes cluster are not impacted by test and staging deployments. Which features should you implement and configure to ensure that the resources for your production applications can be prioritized?

- [x] Configure Namespaces for Test, Staging and Production and configure specific Kubernetes resource quotas for the test and staging Namespaces.
- [ ] Configure labels for Test, Staging and Production and configure specific Kubernetes resource quotas for the Production Namespace.
- [ ] Configure resource requests for Test, Staging and Production and configure specific Kubernetes resource quotas for the Production Namespace.
- [ ] Configure Namespaces for Test, Staging and Production and configure specific Kubernetes resource quotas for the Production Namespace.

**Explanation:**  Resource quotas are used to limit usage in specific Namespaces, and do not need to be configured for all Namespaces, only those you need to limit.


#### Q3. You want to deploy multiple copies of your application, so that you can load balance traffic across them. How should you deploy this application's Pods to the production Namespace in your cluster?

- [ ] Create a Service manifest for the LoadBalancer that specifies the number of replicas you want to run.
- [ ] Deploy the Pod manifest multiple times until you have achieved the number of replicas required.
- [x] Create a Deployment manifest that specifies the number of replicas that you want to run.
- [ ] Create separate named Pod manifests for each instance of the application and deploy as many as you need.


#### Q4. Which Kubernetes component does the kubectl command connect to in order to carry out operations on a cluster?

- [x] kube-apiserver
- [ ] kube-controller-manager
- [ ] kube-scheduler
- [ ] kube-dns


#### Q5. You have a new logging and auditing utility that you need to deploy on all of the nodes within your cluster. Which type of controller should you use to handle this task?

- [ ] ReplicaSet
- [ ] StatefulSet
- [ ] Deployment
- [x] DaemonSet


#### Q6. You are designing an application, and you want to ensure that the containers are located as close to each other as possible, in order to minimize latency. Which design decision helps meet this requirement?

- [ ] Give the containers the same labels.
- [ ] Place the containers in the same Namespace.
- [ ] Place the containers in the same cluster.
- [x] Place the containers in the same Pod.

**Explanation:**  Placing containers in the same Pod ensures they are scheduled together on the same node, minimizing latency.

#### Q7. You have deployed a new Google Kubernetes Engine regional cluster with four machines in the default pool for the first zone and left the number of zones at the default. How many Compute Engine machines are deployed and billed against your account?

- [ ] Sixteen. (Four nodes are deployed in primary and secondary zones in two regions, for a total of 4 zones and 16 nodes. A control plane node is deployed in each zone but it is not billed to your account.)
- [x] Twelve. (Four nodes are deployed in each of three zones. A control plane node is deployed in each zone but it is not billed against your account.)
- [ ] Fifteen. (Four nodes and a single control plane are deployed to each of the three zones. A control plane node is deployed in each zone and it is billed against your account.)
- [ ] Ten. (Four nodes are deployed in the first zone and three nodes are deployed in two other zones because you selected the defaults.)

**Explanation:**  GKE Regional clusters are deployed across multiple zones in a single region. Google also deploys GKE control plane nodes in each zone.
