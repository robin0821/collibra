# Sample Python Code for Collibra REST API

The Postman collection contains a mix of basic auth and csrfToken authentication for POST request for reference. 


## How to deal with authentication
#### 1. Basic Authentication
If your environment support basic authentication, this would be the ideal approach. Collibra has detailed documentation re creating user account, roles and permisssions configure

#### 2. OAUTH Authentication (Beta)
If your environment does not support basic authentication e.g., your environment authentication is outsourced to an IdP such as Azure Entra ID, this will be the ideal approach for authentication. 
Firstly, you need to register an Oauth app in the Collibra DIP. 
Then, you can acquire authorization token by query the Oauth endpoint. 
Documentation for registering the Oauth app can be found at https://productresources.collibra.com/docs/collibra/latest/Content/Settings/OAuth/co_oauth-settings.htm

To date, we haven't found documention or UI on how Collibra manage the roles and permissions for the Oauth app. It seemingly gets SysAdmin permissions. Yet it's still to be tested thoroughly. 

Hope the sample code can assist your integration with Collibra. 

Happy coding.