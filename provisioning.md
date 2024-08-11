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
{: #provisioning-with-console}

Provision from the console by specifying the following parameters:

### Resource configuration
{: #resource-configuration}

- **Service name**: The name can be any string and is the name that is used to identify the new deployment.
- **Resource group**: If you are organizing your services into [resource groups](https://cloud.ibm.com/docs/account?topic=account-account_setup), specify the resource group in this field. Otherwise, you can leave it as Default. For more information, see [Managing resource groups](https://cloud.ibm.com/docs/account?topic=account-rgs).
- **Plan Size**: The size of the deployment. Available sizes will differ based on the plan selected for the deployment.

    | Critical Plan Size | vCPUs for DB Server | Estimated Number of Users per Hour | Estimated Peak Transactinos per Minute | Standard Storage             | Max Storage |
    | ------------------ | ------------------- | ---------------------------------- | -------------------------------------- | ---------------------------- | ----------- |
    | X-Small            | 8                   | 200                                | 480                                    | 1 TB of 5 IOPs Block Storage | 1.5 TB      |
    | Small              | 16                  | 500                                | 960                                    | 2 TB of 5 IOPs Block Storage | 3 TB        |
    | Medium             | 32                  | 1000                               | 1920                                   | 4 TB of 5 IOPs Block Storage | 6 TB        |
    | Large              | 48                  | 2000                               | 3840                                   | 7 TB of 5 IOPs Block Storage | 9.6 TB      |
    | X-Large            | 64                  | 5000                               | 3840                                   | 8 TB of 5 IOPs Block Storage | 9.6 TB      |
    {: row-headers}
    {: class="simple-tab-table"}
    {: caption="Table 1. ServiceNow on IBM Cloud Critical Plans" caption-side="bottom"}
    {: #plansservicenowonibmcloud}
    {: tab-title="ServiceNow on IBM Cloud Critical Plans"}
    {: tab-group="PLANSNOW"}

    | Non-Critical Plan Size | vCPUs for DB Server | Estimated Number of Users per Hour | Estimated Peak Transactinos per Minute | Standard Storage             | Max Storage |
    | ---------------------- | ------------------- | ---------------------------------- | -------------------------------------- | ---------------------------- | ----------- |
    | X-Small                | 8                   | 200                                | 240                                    | 1 TB of 5 IOPs Block Storage | 1.5 TB      |
    | Small                  | 16                  | 500                                | 480                                    | 2 TB of 5 IOPs Block Storage | 3 TB        |
    | Medium                 | 32                  | 1000                               | 960                                    | 7 TB of 5 IOPs Block Storage | 9.6 TB      |
    | Large                  | 48                  | 2000                               | 1440                                   | 8 TB of 5 IOPs Block Storage | 9.6 TB      |
    {: row-headers}
    {: class="simple-tab-table"}
    {: caption="Table 1. ServiceNow on IBM Cloud Non-Critical Plans" caption-side="bottom"}
    {: #plansservicenowonibmcloud}
    {: tab-title="ServiceNow on IBM Cloud Non-Critical Plans"}
    {: tab-group="PLANSNOW"}

- **Additional Storage (GB)**: Additional storage to provision for your deployment. Value must be specified in GB. Value must be greater than or equal to 0, and less than 50% of the base plan size volume.

    | Plan Size | Max Additional Storage (TB) | Max Additional Storage (GB) |
    | --------- | --------------------------- | --------------------------- |
    | X-Small   | 0.5 TB                      | 500 GB                      |
    | Small     | 1 TB                        | 1000 GB                     |
    | Medium    | 2 TB                        | 2000 GB                     |
    | Large     | 3.5 TB                      | 3500 GB                     |
    | X-Large   | 4 TB                        | 4000 GB                     |
    {: caption="Table 2. Additional Storage Options" caption-side="bottom"}

- **On Demand Services**: Select as many as desired. Services that can be provided upon request along with the deployment. These services include:

    - **ServiceNow plugin activation**, a one-time fee to activate a new plugin to an existing ServiceNow instance
    - **Installation of one ServiceNow store application**, a one-time fee to install a ServiceNow Store Application to an existing ServiceNow instance
    - **Capacity Increase**, a one-time fee to add one additional node to an existing ServiceNow instance
    - **Instance cloning**, a one-time fee to close a ServiceNow instance to a new or target instance
    - **Storage upgrade**, a one-time fee to add additional storage
    - **On-demand database backup**, a one-time fee to backup a database on-demand for a single ServiceNow instance
    - **On-demand database restoration**, a one-time fee to restore a database on-demand for a single ServiceNow instance

- **Additional Comments**: Provide any additional details or comments you would like shared with the provisioning team.

After you select the appropriate settings, click **Create** to start the provisoning process.
