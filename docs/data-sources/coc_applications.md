---
subcategory: "Cloud Operations Center (COC)"
layout: "huaweicloud"
page_title: "HuaweiCloud: huaweicloud_coc_applications"
description: |-
  Use this data source to get the list of COC applications.
---

# huaweicloud_coc_applications

Use this data source to get the list of COC applications.

## Example Usage

```hcl
data "huaweicloud_coc_applications" "test" {}
```

## Argument Reference

The following arguments are supported:

* `id_list` - (Optional, List) Appplication id list

* `parent_id` - (Optional, String) Parent application id

* `name_like` - (Optional, String) Fuzzy query the application name

* `code` - (Optional, String) Application code

## Attribute Reference

In addition to all arguments above, the following attributes are exported:

* `data` - Application list

  The [data](#data_struct) structure is documented below.

<a name="data_struct"></a>
The `data` block supports:

* `code` - Application code

* `domain_id` - Specifies the ID of the IAM tenant account

* `parent_id` - Parent application id

* `description` - Application description

* `path` - Application layer path, which is composed of IDs

* `id` - Application id

* `name` - Application name

* `is_collection` - Indicates whether the application is a favorite application

* `update_time` - Modification time

* `create_time` - Creation time
