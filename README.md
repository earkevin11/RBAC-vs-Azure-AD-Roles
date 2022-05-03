# RBAC vs Azure AD-Roles

Role-Based Access Control (RBAC) 
  - RBAC is used by IT Adminstrators to assign access to Azure Resources.

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/166570881-abe4fafd-c497-4059-99be-cc803192fd24.png" height="80%" width="80%" alt="AZ AD Relation RBAC"/>
  
<p/>


Purpose of RBAC
- RBAC provides authorization to your Azure resources such as your storage accounts in your subscription.
- First step to access a resource, a user must authenticate against Azure AD to verify their identity.
- Second step, the user must be authorized to use a specific resource. That is where we use RBAC.
- Remember, if a user is given a role within the Suscription level, the user can access resources with the resource groups within the Sucscription.
- - Subscription Level > Resource Group Level > Resources
- By default, users do not have access to any resources, so we must assign them certain roles.



What are the types of roles used for RBAC?
- Reader Role - allows a user to read the resources but user cannot make changes to the resources.
- 



How do we assign roles?

Navigate to resource



Navigate to resource group 



Navigate to Subscription



