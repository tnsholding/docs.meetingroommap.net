---
title: "Install Reservations Teams add-in"
linkTitle: "Reservations Teams add-in"
tags: ["Reservations", "Teams"]
weight: 200
description: >
  The reservations add-in for Teams enables users to visually perform reservations for desks or other custom locations defined.
---

The reservation system is built as a Teams app. The Desk Reservations app is available in the Microsoft App store:
[https://appsource.microsoft.com/en-US/product/office/wa200003532](https://appsource.microsoft.com/en-US/product/office/wa200003532)


{{% alert title="Grant consent to MeetingRoomMap service" color="warning" %}}
Be sure to have granted admin consent to the MeetingRoomMap service before installing any add-ins. See [Granting consent to the MeetingRoomMap service
](/getting-started/admin/).
{{% /alert %}}



## Prepare Desk Reservations for all users

To prepare Desk Reservations to be used for the company, a Teams administrator should grant org-wide permissions:


#### 1. Go to [Microsoft Teams admin center -> Teams apps -> Manage apps](https://admin.teams.microsoft.com/policies/manage-apps) and search for "Desk reservations"

{{< imgproc adminCenter Resize "880x" >}}
{{< /imgproc >}}

#### 2. Select Desk Reservations app and go to the "Permissions" tab. From here click "Review permissions" and accept permissions

{{< imgproc reviewPermissions Resize "880x" >}}
{{< /imgproc >}}

The following list of permissions are granted:


|   | Permission                                  | Microsoft internal name | Description                                                                                                                                                                  |   |
|---|---------------------------------------------|-------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---|
|   | Sign in and read user profile               | User.Read               | Needed in order to sign in as a user and get basic user profile info.                                                                                                        |   |
|   | Read all users' basic profiles              | User.ReadBasic.All      | Read other users basic profiles. Needed to be able to show names of Team member bookings.                                                                                    |   |
|   | Have full access to user files              | Files.ReadWrite         | Allows the app to read, create, update and delete the signed-in user's files. Using OneDrive's app folder to store user specific settings (i.e. default floorplan/desk etc.) |   |
|   | Read the members of teams                   | TeamMember.Read.All     | Read the members of teams, on behalf of the signed-in user. Needed to get reservations from other team members.                                                              |   |
|   | Read the members of channels                | ChannelMember.Read.All  | Read the members of channels, on behalf of the signed-in user. Needed to get members when add-in is in a private channel.                                                    |   |
|   | Read the names and descriptions of teams    | Team.ReadBasic.All      | Read the names and descriptions of teams, on behalf of the signed-in user.                                                                                                   |   |
|   | Read the names and descriptions of channels | Channel.ReadBasic.All   | Read the names and description of channels, on behalf of the signed-in user.                                                                                                 |   |
|   | Access MeetingRoomMap (MeetingRoomMap)      | N/A                     | Allow the admin site and add-ins to access the MeetingRoomMap backend API on behalf of the signed-in user.                                                                   |   |
|   |                                             |                         |                                                                                                                                                                              |   |

                                                                                                                                                                     |   |
## Installing Desk reservations in Teams

Once an administrator has granted permissions, any user can add the Desk reservations app in Teams - either in a Teams channel or as a personal tab. 
Click "Add a tab" from within any channel or use the "Apps" button and search for "Desk reservations":


{{< imgproc addToTeams Resize "880x" >}}
{{< /imgproc >}}

If added from "Apps" button, then the user can choose to add the app as a personal tab or add it to a specific Team. As a personal tab the app can be pinned like any other app. 
