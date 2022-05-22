# NEED-A-PALYER REST SERVER

This REST service is my university project. Works with MongoDB

## CRUD Operations

All requests are sent to /games/:resource. Supported requests are GET, POST, PUT, PATCH, DELETE

### Authentication

### Register 

Create a new user by sending a POST request to /users/register with properties email and password. You can add any other property that you need, like username, avatar, etc. 
The service automatically creates a session and returns an authorization token, that can be used for requests.

### Login

Login by sending a POST request with email and password to /users/login. 
The service will respond with an object, containing a standard string token, that can be used for requests.

### Logout

Send an authorized GET request to /users/logout. The service returns an empty response - if you attempt to parse it as JSON, you will receive an error!

### Get User details


### Authorized Requests

To make an authorized request, add the following header, where {token} is the access token, returned by the service upon successful login or registration:
Authorization-token: {token}








