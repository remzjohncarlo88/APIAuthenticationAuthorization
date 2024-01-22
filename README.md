This repository features the API Authentication and Authorization with Identity.

Below are the test instructions.
1. Register a username.
2. Login the newly created user. This produce a token to be used in the authorization tab when accessing the controller method/api endpoint.
3. Register a new admin user. Add [Authorize(Roles = UserRoles.Admin)] header in the controller class to allow admin users to access the endpoints.

Decode payload using jwt.io site.
Input the token for decoding from the login endpoint.

TO UPDATE the Database.
From Package Manager Console in VS
- “add-migration Initial” (when creating the DB from start)
- “update-database”

References:
* https://www.c-sharpcorner.com/article/authentication-and-authorization-in-asp-net-core-web-api-with-json-web-tokens/
* https://learn.microsoft.com/en-us/aspnet/core/security/authentication/identity-api-authorization?view=aspnetcore-8.0
* https://auth0.com/docs/quickstart/backend/aspnet-core-webapi/01-authorization
