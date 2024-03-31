

# healthcare-schema
Repository for developing and deploying ddl scripts to snowflake using Terraform and GitHub Actions for the Blue Cross Blue Shield of Rhode Island project.
-----------------------------------------------------

# Contents:
##  GitHub Actions as CICD:
### YML:
Workflows will be in .github/workflows path.
Contains environment specific yml with steps to do a deployment.
Fetches environment specifc Secrets and variable from github secrets based on environment.
### Terraform:
### Main:
Contains the creation of tables and views in snowflake.

### Providers:
Contains required providers for connection to Snowflake and Azure.

### Variables:
Contains the declared variables which can be used during deployment.

### .tfvars File:
Contains the environment specifc details about snowflake Account, Database, Schema, Warehouse and Roles to use for deployment. This is a mandatory file for successful deployment.

-----------------------------------------------------

## Deployment Process:
Non-Prod Deployment: PR to develop branch --> deploys to Sandbox Snowflake Schema -> Approval of PR --> deploys to Dev snowflake Prod Deployment: PR to main branch --> deploys to Stage Snowflake Schema -> Approval of PR --> deploys to Prod snowflake(Not Active)

-----------------------------------------------------


# Note:
  Create a Issue for any new features.
