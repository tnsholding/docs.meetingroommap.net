---
title: "Assign editor role"
linkTitle: "Assign editor role"
tags: ["AdminSite"]
weight: 20
description: >
  Users and groups can be assigned the editor role to delete floorplan images, remove mapped locations, etc.
---

All users signed into the admin website can upload new floorplan images and create mappings (rooms, people, and custom locations).
A standard user does not, however, have the ability to:

- Delete a floorplan (including all existing mappings related to this floorplan)
- Remove (or re-assign) an existing mapping (room, person or custom location)


To enable these actions, a user must be assigned the role "MeetingRoomEditor":

1) Go to the Enterprise Application "MeetingRoomMap" in Azure AD ( [Azure portal -> Azure Active Directory -> Enterprise Applications -> All applications](https://portal.azure.com/#blade/Microsoft_AAD_IAM/StartboardApplicationsMenuBlade/AppAppsPreview/menuId/)  -> select "MeetingRoomMap")
2) Select "Users and groups"
3) Select "+ Add user/group" (or edit of the user is already listed with role "Default access")
4) Select the needed user/group and ensure the role "MeetingRoomEditor" is selected. Click "Assign".


## What’s next?

* [Outlook add-in](/getting-started/outlook/): Install the Outlook add-in to show location of meeting rooms inside Outlook meetings
* [Web parts for SharePoint and Teams](/getting-started/sharepoint/): Install the SharePoint web parts for searching and displaying rooms, users, and custom locations in SharePoint pages and Teams.