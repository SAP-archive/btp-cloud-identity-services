<!-- loio7d2a974c7c1b45b8a61a5c4ad4182002 -->

# Transformations

Transformations help you transform user and group attributes from the data model of the source system to the data model of the target system.



Identity Provisioning provides a default transformation logic for every supported provisioning system. Source systems apply read transformations, target systems apply write transformations, while proxy systems apply both – read and write proxy transformations.

During a provisioning job, the read transformation of the source system converts the system specific JSON representation of users and groups to one common JSON format \(also called internal JSON\). This common JSON format is then used as a source for passing the data to the target system, which applies the write transformation.

The following examples illustrates how the last name user attribute is read from the SAP S/4HANA Cloud source system, transformed and prepared as the family name user attribute for the Identity Authentication target system using both - graphical and JSON text editor.



### Graphical Editor


<table>
<tr>
<th valign="top">

Source System-Specific JSON

</th>
<th valign="top">

Common JSON

</th>
</tr>
<tr>
<td valign="top" colspan="2">

![](images/Transformations_Source_427eb41.png)

</td>
</tr>
</table>


<table>
<tr>
<th valign="top">

Common JSON

</th>
<th valign="top">

Target System-Specific JSON

</th>
</tr>
<tr>
<td valign="top" colspan="2">

![](images/Transformations_Target_0163cb6.png)

</td>
</tr>
</table>



### JSON Text Editor


<table>
<tr>
<th valign="top">

Source System-Specific JSON

</th>
<th valign="top">

Common JSON

</th>
<th valign="top">

Target System-Specific JSON

</th>
</tr>
<tr>
<td valign="top">

> ### Code Syntax:  
> ```
> {
>    "sourcePath":"$.personalInformation.lastName",
>    "targetPath":"$.name.familyName"
> },
> 
> ```



</td>
<td valign="top">

> ### Code Syntax:  
> ```
> {
>    "sourcePath":"$.name.familyName",
>    "targetPath":"$.name.familyName"
> },
> 
> ```



</td>
<td valign="top">

> ### Code Syntax:  
> ```
> {
>    "sourcePath":"$.name.familyName",
>    "targetPath":"$.name.familyName"
> },
> 
> ```



</td>
</tr>
</table>

For more information, see

-   [Transformation Types](https://help.sap.com/docs/identity-provisioning/identity-provisioning/transformation-types?version=Cloud)

-   [Transformation Examples](https://help.sap.com/docs/identity-provisioning/identity-provisioning/transformation-examples?version=Cloud)

-   [Transformation Expressions](https://help.sap.com/docs/identity-provisioning/identity-provisioning/transformation-expressions?version=Cloud)

-   [Transformation Functions](https://help.sap.com/docs/identity-provisioning/identity-provisioning/transformation-functions?version=Cloud)

-   [Transformation Variables](https://help.sap.com/docs/identity-provisioning/identity-provisioning/transformation-variables?version=Cloud)

-   [Transformation Editors](https://help.sap.com/docs/identity-provisioning/identity-provisioning/transformation-editors?version=Cloud)


