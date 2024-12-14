# Cloud-Based Application Documentation

This documentation provides an overview of the system architecture, infrastructure components, and application architecture.

## Cloud Providers <!-- {docsify-ignore} -->

Supported providers:   
- [x] AWS
- [ ] Azure
- [ ] GCP 

## Main Documentation Modules <!-- {docsify-ignore} -->

### System Architecture <!-- {docsify-ignore} -->

This section provides an overview of the system architecture.

- **Overview**: Brief description of the system architecture and key infrastructure components.
- **AWS Services**: List of AWS services used in our infrastructure.
- **Networking**: Description of networking configurations, including VPC, subnets, and security groups.
- **Compute**: Overview of compute resources such as EC2 instances, ECS clusters, or Lambda functions.
- **Storage**: Description of storage solutions like S3 buckets, EBS volumes, or RDS databases.
- **Monitoring and Logging**: Explanation of monitoring and logging solutions using CloudWatch, CloudTrail, etc.
- **Security**: Overview of security measures including IAM policies, encryption, and access controls.

[Click here for detailed documentation on System Architecture](./system-architecture/index.md)

### Infrastructure Components <!-- {docsify-ignore} -->

This section provides an overview of the infrastructure components used to build and deploy our application.

- **Overview**: Brief description of the strategy for constructing infrastructure. 
- **Tooling**: List of tools used in constructing the infrastructure.

[Click here for detailed documentation on Infrastructure Components](./infrastructure/index.md)

### Application Architecture <!-- {docsify-ignore} -->

This section provides insights into the architecture of our application, including its design patterns, components, and interactions.

- **Overview**: Brief description of the application architecture and its key components.
- **Microservices**: Explanation of the microservices architecture, if applicable.
- **Data Management**: Description of data storage and management strategies.
- **Scalability**: Discussion on how the application handles scalability and growth.
- **Resilience**: Explanation of strategies for fault tolerance and disaster recovery.
- **Integration**: Overview of integrations with other systems or services.

### CI/CD Setup<!-- {docsify-ignore} -->

This section provides insights into the configuration and maintenance of CI/CD pipelines.

- **Overview**: Brief description of the strategy for building pipelines.
- **Setup**: Exact steps to required to configure pipelines.
- **Tooling**: List of tools used in pipelines.
  [Click here for detailed documentation on CI/CD](./ci-cd/index.md)
