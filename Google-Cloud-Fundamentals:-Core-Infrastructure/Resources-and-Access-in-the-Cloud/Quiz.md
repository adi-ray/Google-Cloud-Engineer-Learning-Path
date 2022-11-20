## Quiz Questions

#### Q1. Select the option that displays IAM roles from general to specific.

- [ ] Predefined roles, custom roles, basic roles
- [x] Basic roles, predefined roles, custom roles
- [ ] Custom roles, predefined roles, basic roles


#### Q2. Your company has two Google Cloud projects and you want them to share policies. What is the least error-prone way to set this up?

- [ ] Create shared resource policies on the common resources that are used in both projects.
- [ ] Define the new shared policy in the organization node.
- [ ] Duplicate all the policies from one project onto the other.
- [x] Place both projects into a folder, and define the policies on that folder.



#### Q3. Consider a single hierarchy of Google Cloud resources. Which of these situations is possible? (Choose 3 responses.)

- [x] There is an organization node, and there are no folders.
- [x] There is an organization node, and there is at least one folder.
- [ ] There are two or more organization nodes.
- [x] There is no organization node, and there are no folders.
- [ ] There is no organization node, but there is at least one folder.


#### Q4. How does the resource hierarchy control how IAM policies are inherited?

- [ ] IAM policies are only implemented at the project level; they cannot be amended by lower levels of the resource hierarchy.
- [ ] IAM policies that are implemented higher in the resource hierarchy deny access that is granted by lower-level policies.
- [x] IAM policies that are implemented by lower-level policies can override the policies defined at a higher level.


#### Q5. Which way of accessing Google Cloud lets you control services through the code you write?

- [x] APIs
- [ ] The Cloud Console mobile app
- [ ] The Cloud Console
- [ ] The Cloud SDK and Cloud Shell



#### Q6. When would you choose to have an organization node? (Select two)

- [x] When you want to centrally apply organization-wide policies
- [ ] There’s no choice; organization nodes are mandatory.
- [x] When you want to create folders
- [ ] When you want to organize resources into projects

**Explanation:**  Organization nodes let you apply policies centrally. Folders require an organization node

#### Q7. Which statement best describes how Google Cloud resources are associated within the resource hierarchy?

- [ ] All Google Cloud resources are associated with an organization.
- [ ] Google Cloud resources are not associated with the resource hierarchy.
- [x] All Google Cloud resources are associated with a project.
- [ ] All Google Cloud resources are associated with a folder.

**Explanation:**  All Google Cloud resources are associated with a project.


#### Q8. What is the difference between Identity and Access Management (IAM) basic roles and IAM predefined roles?

- [ ] Basic roles only apply to the owner of the Google Cloud project. Predefined roles can be associated with any user.
- [ ] Basic roles can only be granted to single users. Predefined roles can be associated with a group.
- [ ] Basic roles only allow viewing, creating, and deleting resources. Predefined roles allow any modification.
- [x] Basic roles affect all resources in a Google Cloud project. Predefined roles apply to a specific service in a project.

**Explanation:**  Organization nodes let you apply policies centrally. Folders require an organization node
