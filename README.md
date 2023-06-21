# employees-directory

This demonstration repository will execute the following steps to deploy an API to Kong Konnect
  
- Builds our Microservice Container Image and publishes to DockerHub
- Updates the repository containing the Kubernetes configuration with the new docker tag
- Tells ArgoCD to sync and deploy the new microservice containers
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
- Creates Service Hub Service Product
- Prepares Static Documentation
- Uploads Static Documentation using Konnect Admin API
- Deploys declarative config to development environment using decK
- Prepares OAS 
- Uploads OAS to Service Version using Konnect Admin API
- Runs Unit Tests using Inso CLI
- Publishes to Developer Portal using Konnect Admin API
- Turn on App Registration using Konnect Admin API