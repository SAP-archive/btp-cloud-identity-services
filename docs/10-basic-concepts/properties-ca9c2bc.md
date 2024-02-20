<!-- loioca9c2bc5ffee4b6f83b47544264c80eb -->

# Properties

Properties hold the configuration of a provisioning system.

Properties define the connection and authentication information needed for accessing the provisioning system. They control which entities \(users and groups\) will be provisioned - by defining filters and unique attributes, as well as how they will be provisioned - in bulk operations or one entity at a time, with put or patch requests.

There are various types of properties depending on their usability, whether they hold mandatory or optional information, standard information in plain text or credentials in encrypted strings.

Property names have prefixes which indicate the provisioning system the property is applicable for. Properties starting with *<ips\>* are applicable for all provisioning systems, for example `ips.failed.request.retry.attempts`. Those starting with the abbreviation of a provisioning system name, such as *<s4hana.cloud\>* or *<sf\>* are applicable for the given system. For example, `s4hana.cloud.support.bulk.operation` and `sf.user.filter`.

For more information, see [Property Types](https://help.sap.com/docs/identity-provisioning/identity-provisioning/property-types?version=Cloud) and [List of Properties](https://help.sap.com/docs/identity-provisioning/identity-provisioning/list-of-properties?version=Cloud).

