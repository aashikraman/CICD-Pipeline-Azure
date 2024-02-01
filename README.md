# DevOps-Journey-Using-Azure-DevOps

![Azure-DevOps](https://imgur.com/J2F5qPP.png)

In this project I:
- Setup Azure DevOps Project to begin deploying to Azure using Pipelines as code
- Deployed Azure resources using Terraform modules
- Deployed a test application to Azure Kubernetes Service 
- Showcased an understanding of CI/CD with automated application deployments
- Tested my deployed Azure resources using automated testing
- Reviewed monitoring and alerting using Application & Container Insights

The Steps I took in this project are as follows:

1. Initial Setup
   - Azure DevOps Setup
     - Azure DevOps Organisation Setup
     - Azure DevOps Project Creation
     - Azure Service Principal Creation

   - Azure Terraform Setup
     - Create Blob Storage location for Terraform State file

   - Create Azure AD Group for AKS Admin
     - Create Azure AD AKS Admin Group

2. Setup Azure DevOps Pipeline

3. Deployed the application to Azure Container Registry
     - Build the Docker Image Locally
     - Run The Docker Image Locally
     - Deploy sample Application to Container Registry

4. Deployed the application to Azure Kubernetes Cluster
   - Added an AKS ACR Role Assignment
     - Terraform to add role assignment for AKS managed identity to access the deployed ACR

   - Added application insights to terraform
     - Application Insights were used to monitor the application once deployed!

   - Added Azure Key Vault to terraform
     - Azure Key Vault was used to store secrets used within your Azure DevOps Variable Group.

   - Updated pipeline to deploy application to Azure Kubernetes Service
     - Update Pipeline to Deploy asp Application to AKS

5. Introduced CI/CD
   - Began CI/CD with Pipeline Trigger for automatic pipeline runs
   - Automated the deployment of the AKS Application

6. Added Testing to the deployed Azure Infrastructure
  - Used Inspec-Azure to test Azure Resources
     - Run Inspec-Tests using Azure DevOps
     - View Inspec reports in Azure DevOps


7. Added Monitoring and Alerting
   - Used Application Insights to view telemetry data!
   - Configure availability test using Application Insights
   - Logged Analytics Contain Insights


