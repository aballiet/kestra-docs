---
# generated by https://github.com/hashicorp/terraform-plugin-docs
title: kestra_tenant
editLink: false
description: |-
  Use this data source to access information about an existing Kestra Tenant.
  -> This resource is only available on the Enterprise Edition https://kestra.io/enterprise
---

# kestra_tenant (Data Source)

Use this data source to access information about an existing Kestra Tenant.

::alert{type="info"}
This resource is only available on the [Enterprise Edition](https://kestra.io/enterprise)
::

## Example Usage

```hcl
data "kestra_tenant" "example" {
  tenant_id = "my-tenant"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `tenant_id` (String) The tenant id.

### Read-Only

- `id` (String) The ID of this resource.
- `name` (String) The tenant name.
