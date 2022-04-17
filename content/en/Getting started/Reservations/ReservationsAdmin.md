---
title: "Assign ReservationsAdmin role"
linkTitle: "Assign ReservationsAdmin role"
tags: ["Reservations", "AdminSite"]
weight: 50
description: >
  Users and groups can be assigned the ReservationsAdmin role to be able to view and delete any users reservations
---

Reservations are normally edited and viewed using the Reservations add-in in Teams. It's only possible to view your own reservations or those made by other team members - not the entire organization. But an administrator has the ability to view all the reservations across the organization and the possibility to delete reservations made by others. This is done through the admin web site:
[https://www.meetingroommap.net/reservations](https://www.meetingroommap.net/reservations)

To enable these actions, a user must be assigned the role "ReservationsAdmin":

1) Go to the Enterprise Application "MeetingRoomMap" in Azure AD ( [Azure portal -> Azure Active Directory -> Enterprise Applications -> All applications](https://portal.azure.com/#blade/Microsoft_AAD_IAM/StartboardApplicationsMenuBlade/AppAppsPreview/menuId/)  -> select "MeetingRoomMap")
2) Select "Users and groups"
3) Select "+ Add user/group" (or edit of the user is already listed with role "Default access")
4) Select the needed user/group and ensure the role "ReservationsAdmin" is selected. Click "Assign".


## What’s next?

* [View all reservations](/tasks/reservations/): View all reservations as an ReservationsAdmin
* [Sign-up for subscription](/getting-started/subscription/): Sign-up for MeetingRoomMap subscription

