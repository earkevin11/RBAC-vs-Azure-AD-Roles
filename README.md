# Role-Based Access Control (RBAC)

# What is Azure RBAC?
  - RBAC is used by IT Adminstrators to assign access to Azure Resources.

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/166570881-abe4fafd-c497-4059-99be-cc803192fd24.png" height="80%" width="80%" alt="AZ AD Relation RBAC"/>
  
<p/>


# Purpose of RBAC
- RBAC provides authorization to your Azure resources such as your storage accounts in your subscription.
- First step to access a resource, a user must authenticate against Azure AD to verify their identity.
- Second step, the user must be authorized to use a specific resource. That is where we use RBAC.
- Remember, if a user is given a role within the Suscription level, the user can access resources with the resource groups within the Sucscription.
- - Subscription Level > Resource Group Level > Resources
- By default, users do not have access to any resources, so we must assign them certain roles.

# How Azure RBAC works
- The way you control access to resources using Azure RBAC is to assign Azure roles. This is a key concept to understand – it's how permissions are enforced. A role assignment consists of three elements: security principal, role definition, and scope.

# Security principal
- A security principal is an object that represents a user, group, service principal, or managed identity that is requesting access to Azure resources. You can assign a role to any of these security principals.

# What are the types of roles used for RBAC?
- Owner: Grants full access to manage all resources, including the ability to assign or degelate roles to others in Azure.
- Example: Owners of a subscription or a resource grp would be able to deploy virtual machines. Global Admins wouldn't be able to deploy unless they owners.
- Contributor: Grants full access to manage all resources, but does not allow you to assign roles in Azure RBAC, manage assignments in Azure Blueprints, or share image galleries.
- Reader Role: allows a user to read the resources but user cannot make changes to the resources.
- User Administrator Role: permission to manage user accesss to Azure resources.
- And more!



# How do we assign roles at the Subscription level?

Select your <strong> <em> subscription </strong> </em>

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/166617829-4ced4ee8-0b55-400e-8f32-13109acb014c.png" height="85%" width="85%" alt="RBAC Subscription Level"/>
  
<p/>

# Navigate to <strong> <em> Access Control (IAM) </em> </strong> - Subscription level

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/166618716-edc422df-3681-4d1c-b852-5eda88328181.png" height="85%" width="85%" alt="IAM Subscription Level"/>
  
<p/>

Pick and assign the <strong> <em> reader role </em> </strong> (Subscription level)

- Since User A was assigned the reader role at the Subscription level, it can only read the resources and cannot make changes to the resource or add a role assignment. <br/>
- The role will also apply to the resource groups and the resources within the subscription. 
- <strong> <em> Remember that permissions can be inherited and are limited by scope. </em> </strong>

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/166619004-47064c5f-6d9d-408a-ad64-773d9bf2e2d2.png" height="85%" width="85%" alt="Role Assignment Subscription Level"/>

<p/>


# How do we assign roles at the Resource Group level?

Select your <strong> <em>  resoure group </strong> </em> 

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/166622092-7984a9de-f18c-4658-8856-719cd6b4b521.png" height="85%" width="85%" alt="RBAC Resource Grp Level"/>

<p/>


Pick and assign the <strong> <em>  contributor role </strong> </em>  (Resource Group level)
- The contributor role assigned to userB will also apply to the resources within the resource group. <br/>
- <strong> <em> Remember that permissions can be inherited and are limited by scope. </em> </strong>

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/166622130-195fdde1-24fe-4550-ac15-440635870a3b.png" height="85%" width="85%" alt="Role Assignment Resource GRP Level"/>

<p/>


Select your Resource

Pick and assign a role (resource level)



