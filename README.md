
# VMs with RDMs Dashboard for vRealize Operations Cloud
---------

Use this [vRealize Operations](https://www.vmware.com/products/vrealize-operations.html) dashboard to view all VMs with RDMs.  View the details of each vmdk attached to the VM including details about bus sharing.  Please note that this dashboard uses properties that are disabled by default and must be enabled in policy.

## Screenshots
![Dashboard](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-vms_with_rdms/main/images/Dashboard.png)

## Installation
1. This dashboard uses properties that are disabled by default and must be enabled in policy. To enable the necessary properties, navigate to `Configure` / `Policies`.
1. Edit the default policy, which is marked with a D in the Priority column.
![Default Policy](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-vms_with_rdms/main/images/Policy_Default.png)
1. Enable the properties and set instanced state according to the [Metrics section](#Metrics) below. ![Import View](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-vms_with_rdms/main/images/Policy_Metrics.png)
1. Import the views at `Visualize` / `Views` / `Manage` / `...` / `Import`
![Import View](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-vms_with_rdms/main/images/View_Import.png)
1. Click `Browse...` then select the file named [Views.zip](https://github.com/notoriousbdg/vrops-dashboard-vms_with_rdms/raw/main/Views.zip)
1. The included views are listed in the [Views section](#Views)
1. Import the dashboard at `Visualize` / `Dashboards` / `Manage` / `...` / `Import`
![Import Dashboard](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-vms_with_rdms/main/images/Dashboard_Import.png)
1. Click `Browse...` then select the file named [Dashboards.zip](https://github.com/notoriousbdg/vrops-dashboard-vms_with_rdms/raw/main/Dashboards.zip)
1. The included dashboards are listed in the [Dashboards section](#Dashboards)

## Dashboards
| Dashboard Name | Dashboard Path |
|--|--|
| VMs with RDMs | Shared Dashboards (GBrandon)/Configuration |

## Views
| View Name | Dashboard | Name on Dashboard | View Type |
|--|--|--|--|
| VMDK Details Including Bus Sharing and RDM Info | VMs with RDMs | VMDKs for the Selected VM | List |

## Metrics
| Object Type | Metric or Property | Metric Name | Instanced State |
|--|--|--|--|
| Virtual Machine | Property | Virtual Disk&#124;Compatability Mode | Enabled |
| Virtual Machine | Property | Virtual Disk&#124;Disk Mode | Enabled |
| Virtual Machine | Property | Virtual Disk&#124;File Name | Enabled |
| Virtual Machine | Property | Virtual Disk&#124;SCSI Bus Sharing | Enabled |
| Virtual Machine | Property | Virtual Disk&#124;Virtual Device Node | Enabled |
| Virtual Machine | Property | Virtual Disk&#124;SCSI Controller Type | Enabled |
| Virtual Machine | Property | Virtual Disk&#124;Virtual Disk Sharing | Enabled |

## Support

This dashboard requires vRealize Operations Cloud.

Please open an [issue](https://github.com/notoriousbdg/vrops-dashboard-vm_operations/issues) for feedback.

## Changelog
2022-06-06
* Initial release
