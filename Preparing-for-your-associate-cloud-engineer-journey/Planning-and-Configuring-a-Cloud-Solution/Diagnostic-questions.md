## Diagnostic Questions

#### Q1. Cymbal Superstore decides to migrate their supply chain application to Google Cloud. You need to configure specific operating system dependencies. What should you do?

- [ ] Implement an application using containers on Google Kubernetes Engine.
- [x] Implement an application using virtual machines on Compute Engine.
- [ ] Implement an application using containers on Cloud Run.
- [ ] Implement an application using code on App Engine.

**Explanation:** Compute Engine gives you full control over operating system choice and configuration.


#### Q2. The projected amount of cloud storage required for Cymbal Superstore to enable users to post pictures for project reviews is 10 TB of immediate access storage in the US and 30 TB of storage for historical posts in a bucket located near Cymbal Superstore’s headquarters. The contents of this bucket will need to be accessed once every 30 days. You want to estimate the cost of these storage resources to ensure this is economically feasible. What should you do?

- [ ] Use the pricing calculator to estimate the price for 10 TB of multi-region Standard storage, 30 TB for regional Coldline storage, and ingress charges for posts to the bucket.
- [ ] Use the pricing calculator to estimate the costs for 10 TB of regional Standard storage, 30 TB of regional Coldline storage, and egress charges for reads from storage.
- [x] Use the pricing calculator to estimate the price for 10 TB of multi-region Standard storage, 30 TB for regional Nearline, and egress charges for reads from the bucket.
- [ ] Use the pricing calculator to estimate the price for 10 TB of regional Standard storage, 30 TB of regional Nearline storage, and ingress charges for posts to the bucket.

**Explanation:** Data storage pricing is based on the amount of data and storage type. Standard storage is immediately available. Nearline storage is for data accessed roughly every 30 days. Egress is the amount of data read from the bucket and is also chargeable.


#### Q3. Cymbal Superstore needs to analyze whether they met quarterly sales projections. Analysts assigned to run this query are familiar with SQL. What data solution should they implement?

- [ ] Cloud Spanner
- [ ] Cloud Firestore
- [x] BigQuery
- [ ] Cloud SQL

**Explanation:** BigQuery is Google Cloud’s implementation of a modern data warehouse. BigQuery analyzes historical data and uses a SQL query engine.

#### Q4. Cymbal Superstore is piloting an update to its ecommerce app for the flagship store in Minneapolis, Minnesota. The app is implemented as a three-tier web service with traffic originating from the local area and resources dedicated for it in us-central1. You need to configure a secure, low-cost network load-balancing architecture for it. How do you proceed?

- [x] Configure a standard tier proxied external https load balancer connected to the web tier as a frontend and a regional internal load balancer between the web tier and the backend.
- [ ] Configure a proxied SSL load balancer connected to the web tier as the frontend and a standard tier internal TCP/UDP load balancer between the web tier and the backend.
- [ ] Implement a premium tier pass-through external https load balancer connected to the web tier as the frontend and a regional internal load balancer between the web tier and backend.
- [ ] Implement a proxied external TCP/UDP network load balancer connected to the web tier as the frontend and a premium network tier ssl load balancer between the web tier and the backend.

**Explanation:** A standard tier proxied external load balancer is effectively a regional resource. A regional internal load balancer doesn’t require external IPs and is more secure.

#### Q5. Cymbal Superstore decides to pilot a cloud application for their point of sale system in their flagship store. You want to focus on code and develop your solution quickly, and you want your code to be portable. How do you proceed?

- [ ] Implement a deployment manifest and run kubectl apply on it in Google Kubernetes Engine.
- [ ] Code your solution in Cloud Functions.
- [ ] SSH into a Compute Engine VM and execute your code.
- [x] Package your code to a container image and post it to Cloud Run.

**Explanation:** Cloud Run provides serverless container management. It lets you focus on code and you can deploy your solution quickly.

#### Q6. An application running on a highly-customized version of Ubuntu needs to be migrated to Google Cloud. You need to do this in the least amount of time with minimal code changes. How should you proceed?

- [ ] Deploy your application in a container image to Cloud Run.
- [ ] Implement a Kubernetes cluster and create pods to enable your app.
- [x] Create Compute Engine Virtual Machines and migrate the app to that infrastructure.
- [ ] Deploy the existing application to App Engine.

**Explanation:** Compute Engine is a great option for quick migration of traditional apps. You can implement a solution in the cloud without changing your existing code.

#### Q7. Which Google Cloud load balancing option runs at Layer 7 of the TCP stack?

- [ ] Global TCP Proxy
- [ ] Regional Network
- [x] Global http(s)
- [ ] Global SSL Proxy

**Explanation:** https(s) is an application protocol, so it lives at layer 7 of the TCP stack.

#### Q8. Cymbal Superstore’s supply chain application frequently analyzes large amounts of data to inform business processes and operational dashboards. What storage class would make sense for this use case?

- [ ] Nearline.
- [x] Standard.
- [ ] Archive.
- [ ] Coldline

**Explanation:** Standard storage is best for data that is frequently accessed ("hot" data) and/or stored for only brief periods of time. In addition, co-locating your resources by selecting the regional option maximizes the performance for data-intensive computations and can reduce network charges

#### Q9. You want to deploy a microservices application. You need full control of how you manage containers, reliability, and autoscaling, but don’t want or need to manage the control plane. Which compute option should you use?

- [x] Google Kubernetes Engine
- [ ] Compute Engine
- [ ] Cloud Run
- [ ] App Engine

**Explanation:** Google Kubernetes Engine gives you full control of container orchestration and availability.

#### Q10. Cymbal Superstore has a need to populate visual dashboards with historical time-based data. This is an analytical use-case. Which two storage solutions could they use? 

- [ ] Cloud Firestore
- [ ] Cloud SQL
- [x] BigQuery
- [x] Cloud Bigtable
- [ ] Cloud Storage

**Explanation:** BigQuery is a data warehouse offering optimized to query historical time-based data. BigQuery can run queries against data in its own column-based store or run federated queries against data from other data services and file stores.

Cloud Bigtable is a petabyte scale, NoSQL, column family database with row keys optimized for specific queries. It is used to store historic, time-based data and answers the need for this requirement.
