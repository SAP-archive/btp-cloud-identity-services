<!-- loioe52769f1a7ee4d548f2e9e617cab2433 -->

# Tenants

A tenant refers to your \(customer-specific\) instance of SAP Cloud Identity Services. It's delivered to you as part of a bundle with an SAP cloud solution or as part of a self-service request in SAP BTP cockpit.

When SAP Cloud Identity Services are bundled with an SAP cloud solution, you are entitled to one productive and one test tenant preconfigured with the SAP cloud solution. If you get another solution that also bundles SAP Cloud Identity Services, you don't get additional tenant. Your existing one is reused. When your tenant is created as a result of a self-service request, it isn't preconfigured out of the box. You must set it up manually for your specific authentication and provisioning scenarios.

For more information, see [Get Your Tenant](../get-your-tenant-0a7313e.md) and [Bundles](bundles-c1550b6.md).

Standalone tenants refer to SAP Cloud Identity Services - Identity Provisioning tenants delivered and used as a separate \(standalone\) product. As of October 20, 2020, Identity Provisioning is no longer sold as a standalone product. Existing customers of standalone tenants can use them as-is until the end of their contracts.

For more information, see [Standalone Tenant](https://help.sap.com/docs/identity-provisioning/identity-provisioning/tenant-model?version=Cloud#standalone-tenant).



<a name="loioe52769f1a7ee4d548f2e9e617cab2433__section_tgy_3mq_dyb"/>

## Licensing and Usage

From a usage perspective, Identity Authentication, Identity Provisioning, Identity Directory, and SAP Authorization and Trust Management service are commercially included for all SAP-branded cloud solutions sold under the general terms and conditions for SAP Cloud Services, and all applications running on SAP BTP. However, you are charged for every successful authentication to SAP Cloud Identity Services from a third-party application regardless of the protocol used. Only logon requests coming from an SAP cloud or SAP on-premise application are free of charge.

Logon requests are independent of the authentication mechanism and user type.

> ### Example:  
> *SAP Applications*
> 
> -   A user wants to access SAP Build Workzone, an application that runs on SAP BTP. The application delegates authentication to Identity Authentication which is configured to act as a proxy and redirects to the corporate identity provider \(IdP\) for authentication. After successful authentication at the corporate IdP, Identity Authentication sends the single-sign-on \(SSO\) token to SAP Build Workzone. This request counts as a free of charge logon to Identity Authentication.
> 
> -   A user wants to access SAP Integrated Business Planning \(IBP\). The user goes to Identity Authentication via a direct link. After providing the required credentials, Identity Authentication authenticates the user and sends assertion about the user to the service provider, which, in turn, validates the assertion and gives access rights to the user. Identity Authentication redirects the user to SAP IBP. This request counts as a free of charge logon to Identity Authentication.
> 
> *Third-Party Applications*
> 
> -   A user wants to access a third-party application, which delegates authentication to Identity Authentication. The user provides a username and password and is authenticated by Identity Authentication. This request counts as a charged logon to Identity Authentication.

To get a tenant, in addition to the test and productive tenants you're already entitled to, use self-service request. You must have a global account that uses one of the consumption-based commercial models: Cloud Platform Enterprise Agreement \(CPEA\) or Pay-As-You-Go for SAP BTP.

For more information, see [General Terms and Conditions for SAP Cloud Services](https://www.sap.com/about/trust-center/agreements/cloud/cloud-services.html?sort=title_asc&search=General+Terms+and+Conditions)



<a name="loioe52769f1a7ee4d548f2e9e617cab2433__section_sts_hny_dyb"/>

## Tenant Types

Before going live, your organization most probably wants to test various tenant configurations. SAP Cloud Identity Services provide three types of tenants - productive, test, and trial.

Test tenants are used for testing purposes. Productive and test tenants have no difference from a technical and functional perspective. The tenant type flag is just a means for structuring your landscape. This means, an SAP Cloud Identity Services bundle tenant and an SAP cloud solution bundle tenant are created of one particular type: test or productive.

A trial tenant is also intended for testing purposes. However, it differs from the test one as it can be used for a limited period with a limited number of users and some other restrictions.

For more information, see [Tenant Types](https://help.sap.com/docs/identity-authentication/identity-authentication/tenant-types).



<a name="loioe52769f1a7ee4d548f2e9e617cab2433__section_wh2_pwy_dyb"/>

## Tenant Infrastructure

SAP Cloud Identity Services run on several underlying Infrastructure-as-a-Service technologies and regions. Regions are provided either by SAP or by our Infrastructure-as-a-Service \(IaaS\) partners Amazon Web Services \(AWS\), Microsoft Azure, Google Cloud. The third-party region providers operate the infrastructure layer of the regions, whereas SAP operates the platform layer.

For more information, see [Regional Availability](https://help.sap.com/docs/identity-authentication/identity-authentication/regional-availability?version=Cloud).

SAP Cloud Identity Services - Identity Authentication and Identity Provisioning tenants run on the infrastructure of SAP Cloud Identity Services.

> ### Note:  
> Identity Provisioning bundle tenants delivered before March 15, 2022, and Identity Provisioning standalone tenants delivered before September 1, 2020, run on SAP BTP, Neo environment. Customers with tenants on Neo environment are encouraged to migrate them to the SAP Cloud Identity Services infrastructure.
> 
> For more information, see [Migrate Identity Provisioning Bundle Tenant](https://help.sap.com/docs/identity-provisioning/identity-provisioning/migrate-identity-provisioning-bundle-tenant).



<a name="loioe52769f1a7ee4d548f2e9e617cab2433__section_pzg_gkz_dyb"/>

## Tenant Names

SAP Cloud Identity Services tenant, Identity Authentication tenant and Identity Provisioning tenant are sometimes used interchangeably in the documentation. However, there are some differences.

-   *SAP Cloud Identity Services* tenant is an Identity Authentication tenant where Identity Provisioning service is enabled. The Identity Provisioning functionality is embedded in the SAP Cloud Identity Services admin console. The tenant runs on the SAP Cloud Identity Services infrastructure and is accessed at: `https://<ias-tenant-host>/admin`.

    > ### Note:  
    > As of March 15, 2022, *SAP Cloud Identity Services* is the default name of the tenant.

-   *Identity Authentication* tenant is a tenant where the Identity Provisioning service isn't enabled. The Identity Provisioning functionality isn't embedded in the SAP Cloud Identity Services admin console. The tenant runs on the SAP Cloud Identity Services infrastructure and is accessed at: `https://<ias-tenant-host>/admin`.

-   *Identity Provisioning* tenant is a standalone or bundle tenant. It runs on the SAP BTP, Neo environment and its administration console is accessed at: `https://ips-<consumer_account>.dispatcher.<region_host>/webapp/index.html`.


-   **[Tenant Lifecycle](tenant-lifecycle-ce0e551.md "Tenants of SAP Cloud Identity Services - Identity Authentication and Identity
		Provisioning go through onboarding and offboarding in their lifecycle.")**  
Tenants of SAP Cloud Identity Services - Identity Authentication and Identity Provisioning go through onboarding and offboarding in their lifecycle.

