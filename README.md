# Liquibase files and SQL scripts for database management

This bundle generates the following Liquibase files:

 - "**liquibase.properties**"  
   The Liquibase configuration file  
   
   
 - "**changelog.yml**"  
   The root changelog file with the <include> tag referencing other files
   
   
 - "**change-001.sql**"  
   The first changelog file in "plain SQL" format (Liquibase formatted SQL file)
   This file is included in the root changelog.
   
   