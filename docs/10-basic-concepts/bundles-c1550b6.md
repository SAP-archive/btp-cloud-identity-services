<!-- loioc1550b658990455cacf52d4fd7ce13ac -->

# Bundles

A bundle is a group of preconfigured products and services which are sold together.

SAP Cloud Identity Services refer to a bundle as a group of preconfigured SAP cloud solutions and Cloud Identity Services. You purchase the cloud solution and get the services free of charge. The reason for bundling is to offer you out-of-the-box integration between SAP solutions.

> ### Note:  
> As a customer, you need at least one licensed SAP cloud solution which triggers SAP Cloud Identity Services tenant delivery.

The bundling process results in provisioning an SAP Cloud Identity Services tenant to your organization, where Identity Authentication and Identity Provisioning are preconfigured for the relevant SAP cloud solution. In the majority of cases, this means that in the SAP Cloud Identity Services admin console, a bundled application is created and connected to the cloud solution, where your users will log on. The trust between Identity Authentication and the given solution is established. For Identity Provisioning, this means that communication and authentication with the provisioning system is set up. You are ready to schedule and run jobs to synchronize your users and groups.

For more information, see [Get Your Tenant](../20-getting-started/get-your-tenant-0a7313e.md) and [How to Use Bundle Tenants](https://help.sap.com/docs/identity-provisioning/identity-provisioning/bundle-tenants-and-connectors?version=Cloud#how-to-use-bundle-tenants).



<a name="loioc1550b658990455cacf52d4fd7ce13ac__section_b1k_php_ryb"/>

## SAP Cloud Solutions Bundled with Cloud Identity Services

The following SAP cloud solutions bundle with SAP Cloud Identity Services which come preconfigured for the given cloud solutions:


<table>
<tr>
<th valign="top">

SAP \(A-F\)

</th>
<th valign="top">

SAP \(G-Z\)

</th>
</tr>
<tr>
<td valign="top">

-   SAP Build Work Zone, advanced edition

-   SAP Business Ecology Management

-   SAP Business Technology Platform

-   SAP Central Business Configuration

-   SAP Cloud Identity Access Governance

-   SAP Commerce Cloud

-   SAP Commissions

-   SAP Concur

-   SAP Fieldglass




</td>
<td valign="top">

-   SAP Integrated Business Planning for Supply Chain

-   SAP Jam Collaboration

-   SAP Marketing Cloud

-   SAP Market Communication for Utilities

-   SAP S/4HANA Cloud

-   SAP SuccessFactors

-   SAP SuccessFactors Learning

-   Sales Cloud – Analytics & AI




</td>
</tr>
</table>

> ### Note:  
> Some SAP cloud solutions bundle with Identity Authentication only. There could be various reasons for that. For example, the solution may not have a local user store and therefore doesn't need to bundle with Identity Provisioning for managing identity lifecycle. Or the provisioning service doesn't offer a connector to the given SAP cloud solution.

