## Diagnostic Questions

#### Q1.  Which of the scenarios below is an example of a situation where you should use a service account?

- [ ] For interactive analysis
- [x] For individual GKE pods
- [ ] For development environments
- [ ] To directly access user data

**Explanation:** When configuring access for GKE, you set up dedicated service accounts for each pod. You then use workload identity to map them to dedicated Kubernetes service accounts.


#### Q2. You are trying to assign roles to the dev and prod projects of Cymbal Superstore’s e-commerce app but are receiving an error when you try to run set-iam policy. The projects are organized into an ecommerce folder in the Cymbal Superstore organizational hierarchy. You want to follow best practices for the permissions you need while respecting the practice of least privilege. What should you do?

- [ ] Ask your administrator for the roles/resourcemanager.organizationAdmin for Cymbal Superstore
- [ ] Ask your administrator for the roles/iam.securityAdmin role in IAM.
- [x] Ask your administrator for the roles/resourcemanager.folderIamAdmin for the ecommerce folder
- [ ] Ask your administrator for resourcemanager.projects.setIamPolicy roles for each project

**Explanation:** This choice gives you the required permissions while minimizing the number of individual resources you have to set permissions for.


#### Q3.  You have a custom role implemented for administration of the dev/test environment for Cymbal Superstore’s transportation management application. You are developing a pilot to use Cloud Run instead of Cloud Functions. You want to ensure your administrators have the correct access to the new resources. What should you do?

- [ ] Copy the existing role, add the new permissions to the copy, and delete the old role
- [ ] Create a new role with needed permissions and migrate users to it.
- [ ] Delete the custom role and recreate a new custom role with required permissions
- [x] Make the change to the custom role locally and run an update on the custom role

**Explanation:** There is a recommended process to update an existing custom role. You get the current policy, update it locally, and write the updated policy back into Google Cloud. The gcloud commands used in this process include the get and update policy subcommands.


#### Q4. Which Cloud Audit log is disabled by default with a few exceptions?

- [ ] System Event audit logs
- [ ] Policy Denied audit logs
- [x] Data Access audit logs
- [ ] Admin Activity audit logs

**Explanation:** Data Access audit logs are disabled by default except for BigQuery.


#### Q5.  Cymbal Superstore is implementing a mobile app for end users to track deliveries that are en route to them. The app needs to access data about truck location from Pub/Sub using Google recommended practices. What kind of credentials should you use?

- [ ] Environment provided service account
- [x] Service account key
- [ ] OAuth 2.0 client
- [ ] API key

**Explanation:**  Service account keys are used for accessing private data such as your Pub/Sub truck information from an external environment such as a mobile app running on a phone.


#### Q6.  Outline where Cloud Audit logs can be accessed: in the logging tab of the operations interface Link: https://cloud.google.com/storage/docs/audit-logging You are configuring audit logging for Cloud Storage. You want to know when objects are added to a bucket. Which type of audit log entry should you monitor?

- [ ] DATA_READ log entries
- [ ] ADMIN_READ log entries
- [ ] Admin Activity log entries
- [x] DATA_WRITE log entries

**Explanation:** DATA_WRITE log entries include information about when objects are created or deleted.


#### Q7. You need to configure access to Cloud Spanner from the GKE cluster that is supporting Cymbal Superstore’s ecommerce microservices application. You want to specify an account type to set the proper permissions. What should you do?

- [x] Assign permissions through service account referenced by the application
- [ ] Assign permissions through a Cloud Identity account referenced by the application
- [ ] Assign permissions through a Google Workspace account referenced by the application
- [ ] Assign permissions to a Google account referenced by the application

**Explanation:** A service account uses an account identity and an access key. It is used by applications to connect to services.
