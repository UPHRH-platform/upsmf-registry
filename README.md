[Postman Collection](https://api.postman.com/collections/17248210-81d16297-21ec-4100-96c2-a8375d30230f?access_key=PMAT-01GR22Q4K663YDVJ19N84NY2QA)

# upsmf-registry

There are 3 entities declared in the registry

1. Students
2. Teachers
3. Institutes

### Steps to Run 

1. `docker-compose up -d`

**NOTE**
--------

* If you are not using the current config in the folder, then you would have to disable `password-on-login-required` and other settings default security settings in RC's keycloak for the `lr-service` to work properly.
RC's keycloak is customised to force proper emails, username, mobile etc. but these details are missing from CASA database and data sanity is very less, therefor it is needed to disable all those configurations.

* Registry Deployment needs a domain name for it to work properly otherwise tokens will not be provisioned properly. 
