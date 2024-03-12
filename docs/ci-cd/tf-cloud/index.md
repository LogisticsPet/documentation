# Terraform Cloud <!-- {docsify-ignore} -->

## Introduction <!-- {docsify-ignore} -->

Terraform Cloud is utilized for provisioning fundamental infrastructure components that cannot be integrated into any Terragrunt stack. These modules cannot be amalgamated into Terragrunt due to the nature of Terragrunt stacks, which permits stacks to be created or deleted at any time, unlike these essential modules that cannot be destroyed.

These include:

1. Terraform module for managing the Terraform state using an S3 bucket for state storage and DynamoDB for state locking.
2. ECR repositories for Docker images and Helm charts.

## Setup <!-- {docsify-ignore} -->

* **Create Terraform Cloud organization and project**: 
Follow Terraform Cloud documentation to create [organization](https://developer.hashicorp.com/terraform/cloud-docs/users-teams-organizations/organizations#creating-organizations) and [project.](https://developer.hashicorp.com/terraform/cloud-docs/workspaces/organize-workspaces-with-projects#create-a-project)

* **Create [Terrafrom Cloud Workspace](https://developer.hashicorp.com/terraform/cloud-docs/workspaces/creating)** for required modules:
  * [terraform-aws-tf-state](https://github.com/MikalaiYatsyna/terraform-aws-tf-state)
  * [vault-init-ecr-repo](https://github.com/MikalaiYatsyna/terraform-aws-ecr)


* **Configuring Terraform Cloud**
  * Create [Variable set](https://developer.hashicorp.com/terraform/cloud-docs/workspaces/variables/managing-variables#variable-sets)
    | Variable              | Value                         | Description                                                                                   |  
    |-----------------------|-------------------------------|-----------------------------------------------------------------------------------------------|
    | TFC_AWS_PROVIDER_AUTH | true                          | Must be set to true; otherwise, Terraform Cloud will not authenticate to AWS using the IAM role |
    | TFC_AWS_RUN_ROLE_ARN  | {Role ARN created by Cloud Formation} | ARN of the IAM role to use for plan and apply operations                                       |

  * Apply Variable set to workspaces.
* **[Run](https://developer.hashicorp.com/terraform/cloud-docs/run/remote-operations#starting-runs) Terraform Plan & Apply for workspaces**
