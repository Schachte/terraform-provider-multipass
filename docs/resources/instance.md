---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "multipass_instance Resource - terraform-provider-multipass"
subcategory: ""
description: |-
  Multipass instance resource.
---

# multipass_instance (Resource)

Multipass instance resource.



<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `name` (String) Name for the instance. If it is 'primary' (the configured primary instance name), the user's home directory is mounted inside the newly launched instance, in 'Home'.

### Optional

- `cloudinit_file` (String) Path to a user-data cloud-init configuration.
- `cpus` (Number) Number of CPUs to allocate. Minimum: 1, default: 1.
- `disk` (String) Disk space to allocate. Positive integers, in bytes, or with K, M, G suffix. Minimum: 512M, default: 5G.
- `image` (String) Optional image to launch. If omitted, then the default Ubuntu LTS will be used. <remote> can be either ‘release’ or ‘daily‘. If <remote> is omitted, ‘release’ will be used. <image> can be a partial image hash or an Ubuntu release version, codename or alias. <url> is a custom image URL that is in http://, https://, or file:// format.
- `memory` (String) Amount of memory to allocate. Positive integers, in bytes, or with K, M, G suffix. Minimum: 128M, default: 1G.

