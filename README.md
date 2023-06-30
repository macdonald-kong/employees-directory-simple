# employees-directory-simple

This demonstration repository will execute the following steps to deploy the Employees Directory API to Kong Konnect:
  
- Installs Inso CLI (https://insomnia.rest/products/inso)
- Installs decK (https://docs.konghq.com/deck/latest/)
- Lints the OpenAPI Spec (OAS) using Inso CLI
- Generate Kong declarative configuration from OAS using Inso CLI
- Upgrades Version of Kong declarative configuration using Inso CLI
- Uploads Kong declarative config to Artifact Repository
- Validates Kong declarative config using decK
- Diffs declarative config using decK
- Backup existing Kong configuration using decK
- Uploads Kong config backup to Artifact Repository
- Creates API Product
- Prepares Static Documentation
- Uploads Static Documentation using Konnect Admin API
- Deploys declarative config to development environment using decK
- Prepares OAS 
- Uploads OAS to Product Version using Konnect Admin API
- Runs Unit Tests using Inso CLI
- Publishes Product Version to Developer Portal using Konnect Admin API
- Turn on App Registration using Konnect Admin API
