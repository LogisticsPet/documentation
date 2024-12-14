# Terraform Modules <!-- {docsify-ignore} -->

## Purpose  <!-- {docsify-ignore} -->

This document provides an overview of the Terraform modules used to build the infrastructure for the project. Terraform modules encapsulate reusable infrastructure components, making it easier to manage, maintain, and scale infrastructure in a consistent and efficient manner. The purpose of this document is to provide a high-level understanding of the infrastructure components and their interactions, as well as to serve as a reference for the detailed configurations provided in separate documentation for each module.

## Modules Overview <!-- {docsify-ignore} -->

- **[terraform-aws-vpc](./vpc/index.md)**  
  Description: Terraform configuration script to set up AWS VPC  
  Link to source code: [GitHub](https://github.com/LogisticsPet/terraform-aws-vpc)

- **[terraform-aws-route53](./route53/index.md)**   
  Description: Terraform configuration script to set up Public Route 53 zone for specified domain.  
  Link to source code: [GitHub](https://github.com/LogisticsPet/terraform-aws-route53)

- **[terraform-cloudflare-dns-records](./cloudflare/index.md)**   
  Description: Terraform configuration script to set up Cloudflare DNS delegation.  
  Link to source code: [GitHub](https://github.com/LogisticsPet/terraform-cloudflare-dns-records)

- **[terraform-aws-eks](./eks/index.md)**   
  Description: Terraform configuration script to set up Elastic Kubernetes Service Cluster (EKS) on AWS.   
  Link to source code: [GitHub](https://github.com/LogisticsPet/terraform-aws-eks)


## Interaction Overview <!-- {docsify-ignore} -->

To maintain the DRYness of the Terraform configuration, interactions between modules are abstracted using CDK TF.
More details about Terragrunt stacks approach can be found [here.](../cdktf/index.md)
