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
- Owner: Grants full access to manage all resources, including the ability to assign roles in Azure RBAC.
- Contributor: Grants full access to manage all resources, but does not allow you to assign roles in Azure RBAC, manage assignments in Azure Blueprints, or share image galleries.
- Reader Role: allows a user to read the resources but user cannot make changes to the resources.
- And more!



# How do we assign roles? 

Select your subscription

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/166617829-4ced4ee8-0b55-400e-8f32-13109acb014c.png" height="85%" width="85%" alt="RBAC Subscription Level"/>
  
<p/>

Navigate to Access Control (IAM) - Subscription level

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/166618716-edc422df-3681-4d1c-b852-5eda88328181.png" height="85%" width="85%" alt="IAM Subscription Level"/>
  
<p/>

Pick and assign the reader role (Subscription level)

- Since User A was assigned the reader role, it can only read the resource and cannot make changes to the resource or add a role assignment.

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/166619004-47064c5f-6d9d-408a-ad64-773d9bf2e2d2.png" height="85%" width="85%" alt="Role Assignment Subscription Level"/>

<p/>


Select your resource group

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/166622092-7984a9de-f18c-4658-8856-719cd6b4b521.png" height="85%" width="85%" alt="RBAC Resource Grp Level"/>

<p/>


Pick and assign the contributor role (Resource Group level)

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/166622130-195fdde1-24fe-4550-ac15-440635870a3b.png" height="85%" width="85%" alt="Role Assignment Resource GRP Level"/>

<p/>


Select your Resource

Pick and assign a role (resource level)



