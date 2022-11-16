## Diagnostic Questions

#### Q1. Cymbal Superstore has a subnetwork called mysubnet with an IP range of 10.1.2.0/24. You need to expand this subnet to include enough IP addresses for at most 2000 new users or devices. What should you do?

- [ ] gcloud networks subnets expand-ip-range mysubnet --region us-central1 --prefix-length 
- [x] gcloud compute networks subnets expand-ip-range mysubnet --region us-central1 --prefix-length 21
- [ ] gcloud compute networks subnets expand-ip-range mysubnet --region us-cetnral1 --prefix-length 22
- [ ] gcloud compute networks subnets expand-ip-range mysubnet --region us-central1 --prefix-length 20

**Explanation:** This command gives a total of 2046 addresses available and meets the requirement.


#### Q2. You have a Cloud Run service with a database backend. You want to limit the number of connections to your database. What should you do?

- [x] Set Max instances.
- [ ] Set CPU Utilization.
- [ ] Set Concurrency settings.
- [ ] Set Min instances.

**Explanation:** Max instances control costs, keeping you from starting too many instances by limiting your number of connections to a backing service.



#### Q3. What is the declarative way to initialize and update Kubernetes objects?

- [ ] kubectl create
- [ ] kubectl replace
- [ ] kubectl run
- [x] kubectl apply

**Explanation:** kubectl apply creates and updates Kubernetes objects in a declarative way from manifest files.


#### Q4. You have a scheduled snapshot you are trying to delete, but the operation returns an error. What should you do to resolve this problem?

- [ ] Delete the object the snapshot was created from.
- [x] Detach the snapshot schedule before deleting it.
- [ ] Restore the snapshot to a persistent disk before deleting it.
- [ ] Delete the downstream incremental snapshots before deleting the main reference.

**Explanation:** You can’t delete a snapshot schedule that is still attached to a persistent disk.


#### Q5. Cymbal Superstore’s supply chain management system has been deployed and is working well. You are tasked with monitoring the system’s resources so you can react quickly to any problems. You want to ensure the CPU usage of each of your Compute Engine instances in us-central1 remains below 60%. You want an incident created if it exceeds this value for 5 minutes. You need to configure the proper alerting policy for this scenario. What should you do?

- [ ] Choose resource type of VM instance and metric of CPU utilization, condition trigger all time series violates, condition is above, threshold is .60 for 5 minutes.
- [ ] Choose resource type of VM instance, and metric of CPU utilization, condition trigger if any time series violates, condition is below, threshold is .60 for 5 minutes.
- [x] Choose resource type of VM instance and metric of CPU utilization, condition trigger if any time series violates, condition is above, threshold is .60 for 5 minutes.
- [ ] Choose resource type of VM instance and metric of CPU load, condition trigger if any time series violates, condition is below, threshold is .60, for 5 minutes.

**Explanation:** All the values of this statement match the scenario.


#### Q6. What Kubernetes object provides access to logic running in your cluster via endpoints that you define?

- [ ] Pods
- [x] Services
- [ ] Deployments
- [ ] Pod templates

**Explanation:** Service endpoints are defined by pods with labels that match those specified in the service configuration file. Services then specify how those pods are exposed.


#### Q7. Which of the following tasks are part of the process when configuring a managed instance group? (Pick two).

- [x] Providing Number of instances
- [ ] Configuring the operating system
- [ ] Specifying Persistent disks
- [ ] Choosing instance Machine type
- [x] Defining Health checks

**Explanation:** Number of instances is part of your managed instance group configuration.
Health checks are part of your managed instance group configuration.


#### Q8. You want to view a description of your available snapshots using the command line interface (CLI). What gcloud command should you use?

- [ ] gcloud snapshots list
- [ ] gcloud compute snapshots get
- [ ] gcloud compute list snapshots
- [x] gcloud compute snapshots list

**Explanation:** gcloud commands are built with groups and subgroups, followed by a command, which is a verb. In this example, Compute is the Group, snapshots is the subgroup, and list is the command.


#### Q9. You want to implement a lifecycle rule that changes your storage type from standard to nearline after a specific date. What conditions should you use? (Pick two).

- [x] CreatedBefore
- [ ] NumberofNewerVersions
- [x] MatchesStorageClass
- [ ] IsLive
- [ ] Age

**Explanation:** CreatedBefore lets you specify a date.
MatchesStorageClass is required to look for objects with a standard storage type.


#### Q10. Cymbal Superstore’s GKE cluster requires an internal http(s) load balancer. You are creating the configuration files required for this resource. What is the proper setting for this scenario?

- [ ] Configure your service object with a type: LoadBalancer.
- [x] Annotate your service object with a neg reference.
- [ ] Implement custom static routes in your VPC.
- [ ] Annotate your ingress object with an ingress.class of “gce”.

**Explanation:** This is correct because an internal http(s) load balancer can only use NEGs.
