# Liquibase files for database management

This bundle generates the following Liquibase files:

 - "**liquibase.properties**"  
   The Liquibase configuration file  
   
   
 - "**changelog.yml**"  
   The root changelog file referencing SQL files
   
   
 - "**change-001.sql**"  
   The first changelog file in "plain SQL" format (Liquibase formatted SQL file)  
   This file is included in the root changelog.
   
After generating the code, you just need to update the database configuration in the "liquibase.properties" file

And then you can run the usual liquibase commands:

```
> liquibase validate --changelog-file changelog.yml
> liquibase update --changelog-file changelog.yml
> liquibase rollback-count 1 --changelog-file changelog.yml
```