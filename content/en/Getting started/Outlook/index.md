---
title: "Install Outlook add-in"
linkTitle: "Outlook add-in"
tags: ["Outlook"]
weight: 20
description: >
  The Outlook add-in provides users to view the location of meeting rooms from within Outlook meetings.
---

The MeetingRoomMap Outlook add-in is available in the Microsoft App store:
[https://appsource.microsoft.com/en-us/product/office/WA104381386](https://appsource.microsoft.com/en-us/product/office/WA104381386?tab=Overview)


{{% alert title="Grant consent to MeetingRoomMap service" color="warning" %}}
Be sure to have granted admin consent to the MeetingRoomMap service before installing any add-ins. See [Granting consent to the MeetingRoomMap service
](/getting-started/admin/).
{{% /alert %}}


## Centralized Deployment from Microsoft 365 admin center

We recommend deploying the add-in by using the Centralized Deployment feature in the Microsoft 365 admin center [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?#/Settings/IntegratedApps).

#### 1. Go to the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/#/homepage) -> Settings (Click 'show all' if not all menu items available) -> Integrated apps -> Get Apps

{{< imgproc admincenter Fill "880x681" >}}
{{< /imgproc >}}

#### 2. Search for "meetingroommap" and click "Get it now" - be sure to select the "MeetingRoomMap for Outlook" add-in (Fill in the contact information form if needed to proceed).

{{< imgproc appsource Fill "880x681" >}}
{{< /imgproc >}}

#### 3. Choose if you want to install only the Outlook add-in or both the Outlook add-in and the [Teams Bot](/getting-started/teamsbot/)  at the same time

{{< imgproc appsToDeploy Resize "880x" >}}
{{< /imgproc >}}

#### 4. Select the users to receive the add-in (you can start with a limited set of users/groups to test before rolling out to the entire organization)

{{< imgproc addUsers Resize "880x" >}}
{{< /imgproc >}}


#### 5. Accept any missing permissions if needed

{{< imgproc permissions Resize "880x" >}}
{{< /imgproc >}}


#### 5. Click "Finish deployment" and then done.

{{< imgproc finishDeployment Resize "880x" >}}
{{< /imgproc >}}
