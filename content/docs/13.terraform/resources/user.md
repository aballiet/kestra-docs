---
# generated by https://github.com/hashicorp/terraform-plugin-docs
title: kestra_user
editLink: false
description: |-
  Manages a Kestra User.
  -> This resource is only available on the Enterprise Edition https://kestra.io/enterprise
---

# kestra_user (Resource)

Manages a Kestra User.

::alert{type="info"}
This resource is only available on the [Enterprise Edition](https://kestra.io/enterprise)
::

## Example Usage

```hcl
resource "kestra_user" "example" {
  username    = "my-username"
  namespace   = "company.team"
  description = "Friendly description"
  first_name  = "John"
  last_name   = "Doe"
  email       = "john@doe.com"
  groups      = ["4by6NvSLcPXFhCj8nwbZOM"]
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `email` (String) The user email.
- `username` (String) The user name.

### Optional

- `description` (String) The user description.
- `first_name` (String) The user first name.
- `groups` (List of String) The user groups id.
- `last_name` (String) The user last name.
- `namespace` (String) The linked namespace.

### Read-Only

- `id` (String) The ID of this resource.

## Import

Import is supported using the following syntax:

```shell
terraform import kestra_user.example {{user_id}}
```
