---
copyright:
  years: 2024
lastupdated: "2024-05-01"

subcollection: servicenow
---

{{site.data.keyword.attribute-definition-list}}

# Provisioning
{: #provisioning}

Provision a ServiceNow on IBM Cloud deployment through the [catalog](https://test.cloud.ibm.com/catalog/services/servicenow-on-ibm-cloud).
{: shortdesc}

## Provisoning through the IBM Cloud console

Provision from the console by specifying the following parameters:

### Resource configuration

- **Service name**: The name can be any string and is the name that is used to identify the new deployment.
- **Resource group**: If you are organizing your services into [resource groups](https://cloud.ibm.com/docs/account?topic=account-account_setup), specify the resource group in this field. Otherwise, you can leave it as Default. For more information, see [Managing resource groups](https://cloud.ibm.com/docs/account?topic=account-rgs).
- **Plan Size**: The size of the deployment. Available sizes will differ based on the plan selected for the deployment.

  | Plan              | Available Sizes                        |
  | ----------------- | -------------------------------------- |
  | Critical Plan     | X-Small, Small, Medium, Large, X-Large |
  | Non Critical Plan | X-Small, Small, Medium, Large          |

- **Additional Storage (GB)**: Additional storage to provision for your deployment. Value must be specified in GB. Value must be greater than or equal to 0, and less than 50% of the base plan size volume.

  | Plan Size | Max Additional Storage |
  | --------- | ---------------------- |
  | X-Small   | 1 TB = 1000 GB         |
  | Small     | 2 TB = 2000 GB         |
  | Medium    | 4 TB = 4000 GB         |
  | Large     | 7 TB = 7000 GB         |
  | X-Large   | 8 TB = 8000 GB         |

- **On Demand Services**: Services that can be provided upon request along with the deployment. These services include: a ServiceNow plugin activation, the Installation of one ServiceNow store application, a Capacity Increase (limited to one additional node), Instance cloning, Storage upgrade, On-demand database backup, and On-demand database restoration. Select as many as desired.
- **Additional Comments**: Provide any additional details or comments you would like shared with the provisioning team.

After you select the appropriate settings, click **Create** to start the provisoning process.
