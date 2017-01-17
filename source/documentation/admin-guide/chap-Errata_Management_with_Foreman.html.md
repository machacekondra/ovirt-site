# Chapter 14: Errata Management with Foreman

oVirt can be configured to view errata from Foreman in the oVirt Engine. This enables the administrator to receive updates about available errata, and their importance, for hosts, virtual machines, and the Engine once they have been associated with a Foreman provider. Administrators can then choose to apply the updates by running an update on the required host, virtual machine, or on the Engine.

oVirt 4.0 supports errata management with Foreman 6.1.

**Important:** The Engine, hosts, and virtual machines are identified in the Foreman server by their FQDN. This ensures that external content host IDs do not need to be maintained in oVirt.

The Foreman account used to manage the Engine, hosts and virtual machines must have Administrator permissions and a default organization set.

**Configuring oVirt Errata**

To associate a Engine, host, and virtual machine with a Foreman provider first the Engine must be associated with a provider. Then the host is associated with the same provider and configured. Finally, the virtual machine is associated with the same provider and configured.

1. Associate the Engine by adding the required Foreman server as an external provider.

    **Note:** The Engine must be registered to the Foreman server as a content host and have the katello-agent package installed.

2. Optionally, configure the required hosts to display available errata.

3. Optionally, configure the required virtual machines to display available errata. The associated host needs to be configured prior to configuring the required virtual machines. See [Configuring Red Hat Satellite Errata Management for a Virtual Machine](https://access.redhat.com/documentation/en/red-hat-virtualization/4.0/single/virtual-machine-management-guide#Configuring_Satellite_Errata) in the *Virtual Machine Management Guide* for more information.

**Viewing oVirt Engine Errata**

1. Select the **Errata** entry in the tree pane.

2. Click the **Security**, **Bugs**, or **Enhancements** checkboxes to view only those errata types.

For more information on viewing available errata for hosts see [Viewing Host Errata](Viewing_Host_Errata) and for virtual machines see [Viewing Red Hat Satellite Errata for a Virtual Machine](https://access.redhat.com/documentation/en/red-hat-virtualization/4.0/single/virtual-machine-management-guide#Viewing_Satellite_Errata) in the *Virtual Machine Management Guide*.

**Prev:** [Chapter 13: Backups and Migration](../chap-Backups_and_Migration)<br>
**Next:** [Chapter 15: Users and Roles](../chap-Users_and_Roles)