# Overview <!-- {docsify-ignore} -->

CI/CD Pipelines with GitHub Actions and Terraform Cloud

## Introduction <!-- {docsify-ignore} -->
CI/CD (Continuous Integration/Continuous Deployment) pipelines are essential for automating software development workflows. GitHub Actions (GA) and Terraform Cloud (TF Cloud) offer powerful tools for managing and deploying infrastructure resources efficiently.

This guide provides an overview of setting up CI/CD pipelines using GitHub Actions and Terraform Cloud, focusing on authenticating AWS resources.

## Cloud Formation stacks setup <!-- {docsify-ignore} -->

In order to enable Terraform Cloud and GitHub Actions to create resources in AWS, it's essential to set up AWS Authentication. The preferred method involves configuring an OIDC provider, which leverages OIDC to acquire the short-lived credentials necessary for performing actions.

To establish the OIDC provider, IAM Role, and IAM Policy, CloudFormation stacks have been defined. Further details can be found in the [documentation](https://github.com/MikalaiYatsyna/terraform-aws-iam/blob/main/README.md) provided within the terraform-aws-iam repository.

## Terraform Cloud Setup <!-- {docsify-ignore} -->
Terraform Cloud provides a collaborative platform for managing Terraform configurations and state files. 
Terraform Cloud used to provision resources that cannot be part of Terragrunt stacks such as 
1. **[Terraform remote state](https://github.com/MikalaiYatsyna/terraform-aws-tf-state)**: Creates S3 bucket and DynamoDB table to manage Terraform state.
2. **[Docker image and Helm Chart registry](https://github.com/MikalaiYatsyna/terraform-aws-ecr)**: Creates Public ECR Registry to store Docker images and Helm Charts

For detailed instructions on setting up Terraform Cloud, refer to the [Terraform Cloud](./tf-cloud/index.md) documentation.