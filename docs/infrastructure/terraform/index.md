# Terraform Modules <!-- {docsify-ignore} -->

## Purpose  <!-- {docsify-ignore} -->

This document provides an overview of the Terraform modules used to build the infrastructure for the project. Terraform modules encapsulate reusable infrastructure components, making it easier to manage, maintain, and scale infrastructure in a consistent and efficient manner. The purpose of this document is to provide a high-level understanding of the infrastructure components and their interactions, as well as to serve as a reference for the detailed configurations provided in separate documentation for each module.

## Modules Overview <!-- {docsify-ignore} -->

- **[terraform-aws-tf-state](./tf-state/index.md)**  
  Description: Terraform configuration script to set up S3 bucket and DynamoDB table to manage terraform state.  
  Link to source code: [GitHub](https://github.com/MikalaiYatsyna/terraform-aws-tf-state)

- **[terraform-aws-ecr](./ecr/index.md)**   
  Description: Terraform configuration script to set up Elastic Container Registry (ECR) on AWS.  
  Link to source code: [GitHub](https://github.com/MikalaiYatsyna/terraform-aws-ecr)

- **[terraform-aws-route53](./route53/index.md)**   
  Description: Terraform configuration script to set up Public Route 53 zone for specified domain.  
  Link to source code: [GitHub](https://github.com/MikalaiYatsyna/terraform-aws-route53)

- **[terraform-cloudflare-dns-records](./cloudflare/index.md)**   
  Description: Terraform configuration script to set up Cloudflare DNS delegation.  
  Link to source code: [GitHub](https://github.com/MikalaiYatsyna/terraform-cloudflare-dns-records)

- **[terraform-aws-eks](./eks/index.md)**   
  Description: Terraform configuration script to set up Elastic Kubernetes Service Cluster (EKS) on AWS.   
  Link to source code: [GitHub](https://github.com/MikalaiYatsyna/terraform-aws-eks)

- **[terraform-aws-eks-ingress](./ingress/index.md)**   
  Description: Terraform configuration script to set up Nginx ingress for EKS cluster.   
  Link to source code: [GitHub](https://github.com/MikalaiYatsyna/terraform-aws-eks-ingress)

- **[terraform-aws-eks-autoscaler](./autoscaler/index.md)**   
  Description: Terraform configuration script to set up Cluster Autoscaler for AWS EKS.  
  Link to source code: [GitHub](https://github.com/MikalaiYatsyna/terraform-aws-eks-autoscaler)

- **[terraform-aws-eks-cert-manager](./cert-manager/index.md)**   
  Description: Terraform configuration script to set up Certificate Manager for EKS cluster.   
  Link to source code: [GitHub](https://github.com/MikalaiYatsyna/terraform-aws-eks-cert-manager)

- **[terraform-aws-eks-cert-manager-issuer](./cert-issuer/index.md)**   
  Description: Terraform configuration script to set up Let's Encrypt cert manager issuer.
  Link to source code: [GitHub](https://github.com/MikalaiYatsyna/terraform-aws-cert-manager-issuer)

- **[terraform-aws-external-dns](./external-dns/index.md)**   
 Description: Terraform configuration script to set up External DSN for EKS cluster.
 Link to source code: [GitHub](https://github.com/MikalaiYatsyna/terraform-aws-external-dns)

- **[terraform-aws-consul](./consul/index.md)**   
 Description: Terraform configuration script to deploy Hashicorp Consul to EKS cluster.
 Link to source code: [GitHub](https://github.com/MikalaiYatsyna/terraform-aws-consul)

- **[terraform-aws-vault](./vault/index.md)**   
 Description: Terraform configuration script to deploy Hashicorp Vault to EKS cluster.  
 Link to source code: [GitHub](https://github.com/MikalaiYatsyna/terraform-aws-vault)


- **[terraform-vault-k8s-auth](./vault-k8s/index.md)**   
 Description: Terraform configuration script to configure Kubernetes Authentication for Hashicorp Vault.  
 Link to source code: [GitHub](https://github.com/MikalaiYatsyna/terraform-vault-k8s-auth)

- **[terraform-vault-secret-backends](./vault-backends/index.md)**   
 Description: Terraform configuration script to enable Secret Backends in Hashicorp Vault.  
 Link to source code: [GitHub](https://github.com/MikalaiYatsyna/terraform-vault-secret-backends)

  
- **[terraform-argo-cd](./argo-cd/index.md)**   
 Description: Terraform configuration script to deploy Argo CD to EKS cluster.  
 Link to source code: [GitHub](https://github.com/MikalaiYatsyna/terraform-aws-argo-cd)


## Interaction Overview <!-- {docsify-ignore} -->

To maintain the DRYness of the Terraform configuration, interactions between modules are abstracted using Terragrunt.
More details about Terragrunt stacks approach can be found [here.](../terragrunt/index.md)
