# user-manager-x-claim-service
Permission-Based Authorization in ASP.NET Core – Complete User Management Guide in .NET 5
Setting up Permissions to access your resources is always a crucial part of your application’s security. In this article, we will implement Permission-Based Authorization in ASP.NET Core that builds upon the concept of Claim-Based Authorization in ASP.NET Core. As usual, we will be building this application right from scratch to get some detailed knowledge about the whole scenario and how it would actually help you secure your projects

Let me set up the scenario. We have an application, say Stock Management that is to be secured with access levels. For instance, our application has features that can add new products, view product details, delete/modify products. As an ideal business requirement, not all the users should have the permissions to do everything, right? Admins can Add, Edit Products. Basic users can only view the product. Super-Admin can do whatever he wants to. So, this is our requirement. What’s your first approach to it? Role-Based Authorization is the most common and easy approach that would come into your mind naturally. 

What’s Role-Based Authorization?

Role-Based Authorization in ASP.NET Core is a way to restrict/allow users to access specific resources in the application. The [Authorize] attribute when declared in the Controller or any action methods, restricts users bases on his/her role settings. For instance, the Delete method is accessible only to users who have the Role ‘SuperAdmin’ assigned to them, and so on. You are getting the point, yeah? 
