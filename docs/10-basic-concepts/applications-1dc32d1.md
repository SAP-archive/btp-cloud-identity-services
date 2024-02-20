<!-- loio1dc32d156bcc4ed9937bd6778f748e00 -->

# Applications

An application is associated with a consumer of Identity Authentication as an identity provider. This consumer could be for example an SAP cloud solution, a third-party application, SAP BTP subaccount, or the SAP Cloud Identity Services administration console.

The application holds the configuration information about trust, authentication, access, and branding of the given consumer. SAP and customers create applications in SAP Cloud Identity Services administration console. The following table describes the different types of applications, who is in charge of them and whether they are configurable or not:


<table>
<tr>
<th valign="top">

Created By

</th>
<th valign="top">

Application Type

</th>
<th valign="top">

Application Display Name

</th>
<th valign="top">

Specifics

</th>
</tr>
<tr>
<td valign="top" rowspan="4">

SAP

</td>
<td valign="top">

*Bundled Applications* 

</td>
<td valign="top">

For example:

*S4HANA Cloud - *<s4-tenant-type\>**

</td>
<td valign="top">

SAP creates bundled applications and is in charge of their configuration.

</td>
</tr>
<tr>
<td valign="top" rowspan="2">

*System Applications* 

</td>
<td valign="top">

*Administration Console* 

</td>
<td valign="top">

SAP creates and preconfigures the administration console as a system application.

</td>
</tr>
<tr>
<td valign="top">

*User Profile* 

</td>
<td valign="top">

SAP creates and preconfigures the profile page with some personal information.

</td>
</tr>
<tr>
<td valign="top">

*Subscribed Applications* 

</td>
<td valign="top">

For example:

*SAP BTP *<subaccount display name\>**

</td>
<td valign="top">

Subscribed applications are associated with an SAP BTP subaccount or an application registered there. These applications are automatically created for you. You can't create or delete them.

</td>
</tr>
<tr>
<td valign="top" rowspan="2">

Customer

</td>
<td valign="top">

*Charged Applications* 

</td>
<td valign="top">

For example:

*MS Azure AD*

</td>
<td valign="top">

Charged applications are created by customers for third-party \(non-SAP\) solutions. Customers are in charge of the configuration and are charged for integrating applications with Identity Authentication.

</td>
</tr>
<tr>
<td valign="top">

*Bundled Applications* 

</td>
<td valign="top">

For example:

*SAP Concur*

</td>
<td valign="top">

Apart from SAP, bundled applications can also be created by customers. This applies for SAP cloud applications that do not bundle the delivery and preconfiguration of the SAP Cloud Identity Services.

</td>
</tr>
</table>

Applications are sometimes referred to as SAML 2.0 applications or OpenID Connect applications depending on the configured protocol. The SAML 2.0 standard defines applications as service providers, while OpenID Connect \(OIDC\) defines them as relying parties.

For more information, see [Application Types](https://help.sap.com/docs/identity-authentication/identity-authentication/application-types) and [Configuring Applications](https://help.sap.com/docs/identity-authentication/identity-authentication/configuring-applications)

