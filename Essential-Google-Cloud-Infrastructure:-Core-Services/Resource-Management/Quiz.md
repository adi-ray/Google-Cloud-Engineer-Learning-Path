## Quiz Questions

#### Q1. How do quotas protect Google Cloud customers?

- [x] By preventing uncontrolled consumption of resources.
- [ ] By preventing resource use by unknown users.
- [ ] By preventing resource use of too many different Google Cloud services.
- [ ] By preventing resource use in too many zones in a region.


**Explanation:** Quotas are established at reasonable defaults for common cloud usage and proof of concept activities. If you are planning to scale up a production cloud solution you may need to request that the quotas be raised. This is a reasonable checkpoint to verify that actions that might result in a large consumption of resources are reviewed.

#### Q2. A budget is set at $500 and an alert is set at 100%. What happens when the full amount is used?

- [ ] Nothing. There is no point in sending a notification when there is no budget remaining.
- [x] A notification email is sent to the Billing Administrator.
- [ ] You have a 4-hour courtesy period before Google shuts down all resources.
- [ ] Everything in the associated project will be suspended because there is no more budget to spend.


**Explanation:** Budgets in Google Cloud are not a way to prevent spending or stop resources. They are a tool for raising awareness about the consumption of resources so that a business can implement its own consumption management processes.

#### Q3. No resources in Google Cloud can be used without being associated with...

- [x] A project.
- [ ] A virtual machine.
- [ ] A bucket.
- [ ] A user.


**Explanation:**  All resources in Google Cloud are tracked and their consumption is logged against a project. A project relates resources to a billing method.
