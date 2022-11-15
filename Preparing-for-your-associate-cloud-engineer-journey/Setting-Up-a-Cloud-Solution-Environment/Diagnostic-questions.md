## Diagnostic Questions

#### Q1. How are resource hierarchies organized in Google Cloud?

- [x] Organization, Folder, Project, Resource
- [ ] Project, Organization, Folder, Resource
- [ ] Resource, Folder, Organization, Project
- [ ] Organization, Project, Resource, Folder

**Explanation:** Organization sits at the top of the Google Cloud resource hierarchy. This can be divided into folders, which are optional. Next, there are projects you define. Finally, resources are created under projects.


#### Q2. How are billing accounts applied to projects in Google Cloud? (Pick two).

- [ ] A project and its resources can be tied to more than one billing account.
- [x] A billing account can be linked to one or more projects.
- [ ] Set up Cloud Billing to pay for usage costs in Google Cloud projects and Google Workspace accounts.
- [x] A project and its resources can only be tied to one billing account.

**Explanation:** A billing account can handle billing for more than one project.
 A project can only be linked to one billing account at a time.
 
 
#### Q3. Stella is a new member of a team in your company who has been put in charge of monitoring VM instances in the organization. Stella will need the required permissions to perform this role. How should you grant her those permissions?

- [ ] Assign Stella compute.instances.get permissions on all of the projects she needs to monitor.
- [x] Add Stella to a Google Group in your organization. Bind that group to roles/compute.viewer.
- [ ] Assign the “viewer” policy to Stella.
- [ ] Assign Stella a roles/compute.viewer role.

**Explanation:** Best practice is to manage role assignment by groups, not by individual users.
 
 
 #### Q4. Fiona is the billing administrator for the project associated with Cymbal Superstore’s eCommerce application. Jeffrey, the marketing department lead, wants to receive emails related to budget alerts. Jeffrey should have access to no additional billing information. What should you do?

- [x] Use Cloud Monitoring notification channels to send Jeffrey an email alert.
- [ ] Add Jeffrey and Fiona to the budget scope custom email delivery dialog.
- [ ] Send alerts to a Pub/Sub topic that Jeffrey is subscribed to.
- [ ] Change the budget alert default threshold rules to include Jeffrey as a recipient.

**Explanation:** You can set up to 5 Cloud Monitoring channels to define email recipients that will receive budget alerts.


#### Q5. Pick two choices, from the options below, that provide a command line interface to Google Cloud.

- [ ] REST-based API
- [x] Cloud Shell
- [ ] Cloud Mobile App
- [x] Cloud SDK
- [ ] Google Cloud console

**Explanation:**  Cloud Shell provides a cloud-based CLI environment.
The Cloud SDK provides a local CLI environment.
 
 #### Q6. What Google Cloud project attributes can be changed?

- [x] The Project Name.
- [ ] The Project Number.
- [ ] The Project Category.
- [ ] The Project ID.

**Explanation:** Project name is set by the user at creation. It does not have to be unique. It can be changed after creation time.


#### Q7. You need to add new groups of employees in Cymbal Superstore’s production environment. You need to consider Google’s recommendation of using least privilege. What should you do?

- [ ] Grant the least restrictive basic roles to most services and grant predefined and custom roles only when necessary.  
- [x] Grant predefined and custom roles that provide necessary permissions and grant basic roles only where needed.
- [ ] Grant custom roles to individual users and implement basic roles at the resource level.
- [ ] Grant the most restrictive basic role to most services, grant predefined or custom roles as necessary.

**Explanation:** Basic roles are broad and don’t use the concept of least privilege. You should grant only the roles that someone needs through predefined and custom roles.
 
 #### Q8. You want to use the Cloud Shell to copy files to your Cloud Storage bucket. Which Cloud SDK command should you use?

- [ ] gcloud
- [ ] Cloud Storage Browser
- [ ] bq
- [x] gsutil

**Explanation:**  Use gsutil to interact with Cloud Storage via the Cloud SDK.


#### Q9. The Operations Department at Cymbal Superstore wants to provide managers access to information about VM usage without allowing them to make changes that would affect the state. You assign them the Compute Engine Viewer role. Which two permissions will they receive?

- [x] compute.images.get
- [ ] computer.images.update
- [ ] compute.images.create
- [x] compute.images.list
- [ ] compute.images.setIAM

**Explanation:** Get is read-only. Viewer has this permission.
Viewers can perform read-only actions that do not affect state.


#### Q10. Jane will manage objects in Cloud Storage for the Cymbal Superstore. She needs to have access to the proper permissions for every project across the organization. What should you do? 
- [ ] Assign Jane the roles/viewer on each project and the roles/storage.objectCreator for each bucket.
- [ ] Assign Jane the roles/editor at the organizational level.
- [x] Add Jane to a group that has the roles/storage.objectAdmin role assigned at the organizational level.
- [ ] Assign Jane the roles/storage.objectCreator on every project.

**Explanation:** This would give Jane the right level of access across all projects in your company.
