---
title: "Changing mapping attribute"
linkTitle: "Changing mapping attribute"
tags: ["AdminSite", "Users"]
weight: 50
description: >
  If mapping users by their office location attribute is not desired, the grouping attribute can be changed. I.e. to ensure all users are mapped individually use ‘email’ attribute.
---

## Changing mapping attribute

If mapping users by their office location attribute is not desired, the grouping attribute can be changed. I.e. to ensure all users are mapped individually use 'email' attribute.

To change the grouping attribute, navigate to the [TenantSettings](https://www.meetingroommap.net/TenantSettings) page:

{{< imgproc settings Resize "854x" >}}
{{< /imgproc >}}

Change the property to group by and click "Save settings". Be aware that the property specified must be a valid user property name (the internal name as defined in Microsoft Graph API).

{{% alert title="All users must be re-mapped" color="warning" %}}
Be aware that changing the grouping attribute affects all existing mappings for users. All users will have to be re-mapped.
{{% /alert %}}