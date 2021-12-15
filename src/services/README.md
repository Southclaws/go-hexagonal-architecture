# services

This is where business logic happens! Services import resources and are imported by interfaces.

## Note regarding basic CRUD

Do not write a service for basic CRUD! This is just a waste of time.

If all your service does is import a repository and re-export those functions, just delete it and use the repository directly.
