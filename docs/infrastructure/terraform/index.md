# Terraform Modules <!-- {docsify-ignore} -->

This document provides an overview of the Terraform modules used to build the infrastructure for project. Terraform modules encapsulate reusable infrastructure components, making it easier to manage, maintain, and scale infrastructure in a consistent and efficient manner.

## Purpose <!-- {docsify-ignore} -->

The purpose of this document is to provide a high-level understanding of the infrastructure components and their interactions, as well as to serve as a reference for the detailed configurations provided in separate documentation for each module.

## Modules Overview <!-- {docsify-ignore} -->


- **[terraform-aws-ecr](./ecr/index.md)**   
  Description: Terraform configuration script to set up an Elastic Container Registry (ECR) on AWS.  
  Link to source code: [GitHub](https://github.com/MikalaiYatsyna/terraform-aws-ecr)

- **[terraform-aws-eks](./ecr/index.md)**   
  Description:   Terraform configuration script to set up an Elastic Kubernetes Service Cluster (EKS) on AWS.   
  Link to source code: [GitHub](https://github.com/MikalaiYatsyna/terraform-aws-eks)

## Interaction Overview <!-- {docsify-ignore} -->

To maintain the DRYness of the Terraform configuration, interactions between modules are abstracted using Terragrunt.
More details about Terragrunt stacks approach can be found [here.](../terragrunt/index.md)

## Next Steps <!-- {docsify-ignore} -->

Refer stakeholders to the detailed documentation for each module to understand specific configurations, usage, and best practices. Encourage feedback and collaboration to continuously improve and evolve infrastructure architecture.
