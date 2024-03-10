# Packer templates <!-- {docsify-ignore} -->

## Purpose  <!-- {docsify-ignore} -->

This document offers an insight into the Packer templates utilized in constructing the project's infrastructure. Packer templates encapsulate reusable machine image configurations, streamlining images building process in a uniform and effective manner.

## Modules Overview <!-- {docsify-ignore} -->

- **[vault-init-image](./vault-init/index.md)**  
  Description: Packer template to build Docker image for initializing and unsealing Hashicorp Vault instances.    
  Link to source code: [GitHub](https://github.com/MikalaiYatsyna/vault-init-image)

- **[consul-kv-operator](./consul-kv-operator/index.md)**   
  Description: Packer template to build Docker image for Consul KV Kubernetes operator.  
  Link to source code: [GitHub](https://github.com/MikalaiYatsyna/consul-kv-operator)