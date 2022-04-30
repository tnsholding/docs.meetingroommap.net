---
title: "Users"
linkTitle: "Mapping co-workers location"
tags: ["AdminSite", "Users"]
weight: 30
description: >
  Map co-workers to floorplans
---

Mapped co-workers enables searching and viewing their location in the Teams and SharePoint add-ins.

## Users available to map

The list of users is automatically fetched from Azure AD and displayed on the [Persons](https://www.meetingroommap.net/Persons) page.

By default users are grouped by their Office location attribute. This enables mapping all users having the same Office Location with a single mapping (see [Changing mapping attribute](/tasks/people/changemappingattribute/) to change the grouping).

The Office location attribute can be viewed here: Microsoft 365 admin center -> Users -> select user -> Manage contact information:

{{< imgproc officeLocation Resize "575x" >}}
{{< /imgproc >}}

## Map users

Mapping a user (or group of users with same grouping attribute) is done by navigating to the [Persons](https://www.meetingroommap.net/Persons) page.

1) Find the user to map in the list (use sorting, paging and search to quickly find the correct user)
2) Click "Attach to map" button
3) A popup "Select map to attach to" with all available floorplans displays - click the floorplan to map to
4) A popup windows with the floorplan is opened - click the location of the user to create the mapping

#### Removing mapping

An existing mapping can be removed by clicking the "Remove" button for a specific user (or group of users with same grouping attribute) in the list. (NB. requires the role "MeetingRoomEditor" to remove).




