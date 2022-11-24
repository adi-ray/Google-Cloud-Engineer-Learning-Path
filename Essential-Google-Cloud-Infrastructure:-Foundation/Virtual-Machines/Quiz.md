## Quiz Questions

#### Q1. Which statement is true of Virtual Machine Instances in Compute Engine?

- [ ] Compute Engine uses VMware to create Virtual Machine Instances.
- [ ] All Compute Engine VMs are single tenancy and do not share CPU hardware.
- [ ] A VM in Compute Engine always maps to a single hardware computer in a rack.
- [x] In Compute Engine, a VM is a networked service that simulates the features of a computer.


**Explanation:**  VMs in Compute Engine are a collection of networked services which includes persistent disks that are network-attached. In some cases the Google Cloud VM behaves unlike hardware or other kinds of virtual machines, for example, when a multi-tenant virtual CPU "bursts", using excess capacity beyond the VM spec.

#### Q2. Which statement is true of persistent disks?

- [ ] Persistent disks are physical hardware devices connected directly to VMs.
- [ ] Once created, a persistent disk cannot be resized.
- [x] Persistent disks are encrypted by default.
- [ ] Persistent disks are always HDDs (magnetic spinning disks).

**Explanation:**  Persistent Disks are not physical disks, they are a virtual-networked service. Each persistent disk remains encrypted either with system-defined keys or with customer-supplied keys.

#### Q3. What are sustained use discounts?

- [ ] Purchase commitments for specific resources you know you will use
- [ ] Per-second billing that starts after a 1 minute minimum
- [ ] Discounts you receive by using preemptible VM instances
- [x] Automatic discounts that you get for running specific Compute Engine resources for a significant portion of the billing month

**Explanation:** Sustained use discounts are automatic discounts that you get for running specific Compute Engine resources (vCPUs, memory, GPU devices) for a significant portion of the billing month. To take advantage of the full 30% discount, create your VM instances on the first day of the month, because discounts reset at the beginning of each month.
