# Overview <!-- {docsify-ignore} -->
Building infrastructure using Infrastructure as Code (IaaC) has become essential in modern software development practices. It provides numerous benefits such as version control, reproducibility, scalability, and automation. By defining infrastructure in code, teams can manage and deploy complex environments more efficiently, leading to faster development cycles and improved reliability.

# Building Blocks <!-- {docsify-ignore} -->

There are numerous single-purpose Terraform modules available, each offering specific functionalities tailored for building infrastructure. These modules streamline the deployment process, enhance reusability, and promote consistency across environments. In contrast, when leveraging Terragrunt, these modules are organized into configurations, facilitating modularization and abstraction. This approach simplifies management, promotes code reuse, and enables better separation of concerns, ultimately improving maintainability and scalability of the infrastructure.

## Terraform Modules <!-- {docsify-ignore} -->
Terraform modules are reusable, encapsulated components that represent infrastructure resources or configurations. They enable modularization of infrastructure code, promoting reusability, consistency, and scalability. By abstracting complex infrastructure components into modular units, Terraform modules simplify management and facilitate collaboration among teams.

For more information, refer to the [Terraform Modules documentation.](terraform/index.md)

## CDK TF Stacks <!-- {docsify-ignore} -->

CDK TF stacks represent configurations that orchestrate Terraform modules to provision infrastructure. Stacks provide an abstraction layer for managing complex infrastructure deployments, allowing users to organize and reuse modules efficiently. CDK TF enhances Terraform workflows by providing additional features such as remote state management, dependency handling, and configuration templating.

For more details, consult the [CDK TF documentation.](cdktf/index.md)

# Tooling used to built infrastructure <!-- {docsify-ignore} -->
- Terraform
- CDK TF
