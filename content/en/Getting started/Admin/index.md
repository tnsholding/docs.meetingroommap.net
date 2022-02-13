---
title: "Granting consent to the MeetingRoomMap service"
linkTitle: "Granting consent"
tags: ["AdminSite"]
weight: 10
description: >
  Before using the MeetingRoomMap admin site or any of the add-ins, an Azure/Office365 Tenant administrator needs to give consent.
---

The MeetingRoomMap service is being registered as an application in Azure Active Directory (AAD) and requires a few permissions in the target AAD to function.

## Grant consent as tenant administrator

**To grant consent to MeetingRoomMap, click on "Enroll your company in MeetingRoomMap" on the front page of the admin site ([https://www.meetingroommap.net](https://www.meetingroommap.net/)) or go directly to this link:</br>
[https://www.meetingroommap.net/Account/SignUp](https://www.meetingroommap.net/Account/SignUp)**

{{% alert title="To grant tenant-wide admin consent, you need:" color="secondary" %}}
An Azure account with one of the following roles: Global Administrator, Privileged Role Administrator, Cloud Application Administrator, or Application Administrator. A user can also be authorized to grant tenant-wide consent if they are assigned a custom directory role that includes the permission to grant permissions to applications.
{{% /alert %}}


Learn more about granting admin consent here:</br>
https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/grant-admin-consent

## Permissions

When granting consent the following list of delegated permissions are requested:

{{< imgproc consent Fill "433x749" >}}
{{< /imgproc >}}


{{% alert title="Delegated permissions" color="info" %}}

All permissions granted are of type 'Delegated' (and not application). All requests are thus made on behalf of the currently signed-in user and adhere to the signed-in user's privileges. The application does not have any permissions on it's own (read more here: [https://docs.microsoft.com/en-us/graph/auth/auth-concepts#delegated-and-application-permissions](https://docs.microsoft.com/en-us/graph/auth/auth-concepts#delegated-and-application-permissions))
{{% /alert %}}

The table below indicates the usage and justification of each individual delegated permission:

| Permission                                          | Microsoft internal name  | Description                                                                                                                                                      |
|-----------------------------------------------------|--------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Read all company places                             | Place.Read.All           | Allow to read list of company's places (meeting rooms and room lists). Needed to map meeting rooms defined in Azure AD to floorplans.                            |
| Maintain access to data you have given it access to | offline_access           | Maintain access to data you have given it access to.                                                                                                              |
| Read user mailbox settings                          | MailboxSettings.Read     | Allow to read users mailbox settings. Add-ins need timezone info from mailbox settings to display correct dates/time for displaying meetings.                     |
| Sign in and read user profile                       | User.Read                | Needed in order to sign in as a user and get basic user profile info.                                                                                            |
| Read all users' full profiles                       | User.Read.All            | Read other users profiles. Needed to get OfficeLocation attribute in order to use MeetingRoomMap to map co-workers and used to facilitate search for co-workers. |
| Read user calendars                                 | Calendars.Read           | Allows the app to read events in your calendars. Outlook add-in needs this to access the current meeting and Teams Bot uses this to show your next meetings.     |
| Access MeetingRoomMap (MeetingRoomMap)              | N/A                      | Allow the admin site and add-ins to access the MeetingRoomMap backend API on behalf of the signed-in user.                                                       |
|                                                     |                          |                                                                                                                                                                  |

## What’s next?

* [Assign editor role](/getting-started/editor/): Assign users/groups the editor role in order to delete floorplans and mappings.
* [Outlook add-in](/getting-started/outlook/): Install the Outlook add-in to show location of meeting rooms inside Outlook meetings.
* [Web parts for SharePoint and Teams](/getting-started/sharepoint/): Install the SharePoint web parts for searching and displaying rooms, users, and custom locations in SharePoint pages and Teams.
