# Overview
Building infrastructure using Infrastructure as Code (IaaC) has become essential in modern software development practices. It provides numerous benefits such as version control, reproducibility, scalability, and automation. By defining infrastructure in code, teams can manage and deploy complex environments more efficiently, leading to faster development cycles and improved reliability.

# Building Blocks

There are numerous single-purpose Terraform modules available, each offering specific functionalities tailored for building infrastructure. These modules streamline the deployment process, enhance reusability, and promote consistency across environments. In contrast, when leveraging Terragrunt, these modules are organized into configurations, facilitating modularization and abstraction. This approach simplifies management, promotes code reuse, and enables better separation of concerns, ultimately improving maintainability and scalability of the infrastructure.

## Terraform Modules
Terraform modules are reusable, encapsulated components that represent infrastructure resources or configurations. They enable modularization of infrastructure code, promoting reusability, consistency, and scalability. By abstracting complex infrastructure components into modular units, Terraform modules simplify management and facilitate collaboration among teams.

For more information, refer to the [Terraform Modules documentation.](terraform/index.md)

## Terragrunt Stacks

Terragrunt stacks represent configurations that orchestrate Terraform modules to provision infrastructure. Stacks provide an abstraction layer for managing complex infrastructure deployments, allowing users to organize and reuse modules efficiently. Terragrunt enhances Terraform workflows by providing additional features such as remote state management, dependency handling, and configuration templating.

For more details, consult the [Terragrunt documentation.](terragrunt/index.md)

## Packer templates

Packer templates are HCL files used to define the configuration for building machine images (AMI, VHD, etc.). They enable the automated creation of identical machine images for multiple platforms from a single source configuration. Packer templates specify the builders, provisioners, and post-processors required to create and customize machine images efficiently.

For more information, see the [Packer templates documentation.](packer/index.md)

# Tooling used to built infrastructure
- Terragrunt
- Terraform
- Packer