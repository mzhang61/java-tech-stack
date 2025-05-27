### HATEOAS is not commonly used
### Actuator is commonly used, and its attributes are in the application.properties file.
### Actuator requires more steps for security purpose
### GetMapping
GET http://localhost:8080/v1/organization/{organizationId}/license/{licenseId}
Example: GET http://localhost:8080/v1/organization/123/license/456
### PostMapping
POST http://localhost:8080/v1/organization/{organizationId}/license
Example: POST http://localhost:8080/v1/organization/123/license
Content-Type: application/json
Accept-Language: en
{
"licenseId": "456",
"productName": "Product A",
"licenseType": "FULL",
"organizationId": "123"
}

### PutMapping
PUT http://localhost:8080/v1/organization/{organizationId}/license
Example: PUT http://localhost:8080/v1/organization/123/license
Content-Type: application/json
{
"licenseId": "456",
"productName": "Product B",
"licenseType": "TRIAL",
"organizationId": "123"
}

// DeleteMapping
DELETE http://localhost:8080/v1/organization/{organizationId}/license/{licenseId}
Example: DELETE http://localhost:8080/v1/organization/123/license/456
