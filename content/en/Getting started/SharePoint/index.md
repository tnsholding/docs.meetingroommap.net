---
title: "Install web parts for SharePoint and Teams"
linkTitle: "SharePoint/Teams web parts"
tags: ["SharePoint", "Teams"]
weight: 30
description: >
  The SharePoint web parts enables users to search and view meeting rooms, people and custom locations in both SharePoint and Teams.
---

The MeetingRoomMap web parts for SharePoint and Teams add-in is available in the Microsoft App store:
[https://appsource.microsoft.com/en-us/product/office/WA200001948](https://appsource.microsoft.com/en-us/product/office/WA200001948?tab=Overview)


{{% alert title="Grant consent to MeetingRoomMap service" color="warning" %}}
Be sure to have granted admin consent to the MeetingRoomMap service before installing any add-ins. See [Granting consent to the MeetingRoomMap service
](/getting-started/admin/).
{{% /alert %}}


## Centralized Deployment from Microsoft 365 admin center

We recommend deploying the add-in by using the Centralized Deployment feature in the Microsoft 365 admin center [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?#/Settings/IntegratedApps).

#### 1. Go to the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/#/homepage) -> Settings (Click 'show all' if not all menu items available) -> Integrated apps -> Get Apps

{{< imgproc admincenter Fill "880x681" >}}
{{< /imgproc >}}

#### 2. Search for "meetingroommap" and click "Get it now" - be sure to select the "MeetingRoomMap WebParts" add-in (Fill in the contact information form if needed to proceed).

{{< imgproc appsource Resize "880x" >}}
{{< /imgproc >}}

#### 3. SharePoint add-ins can't modify users, so just click "Next" on the "Add users" page.

#### 4. Click "Next" on the "Accept permissions requests" page.

#### 5. Click "Finish deployment" on the "Review and finish deployment" page.

#### 6. Make sure you click "Accept permissions" and grant permissions. Click "Done" once permissions accepted.

{{< imgproc acceptPermissions Resize "880x" >}}
{{< /imgproc >}}




## Make sure Web parts are available in all SharePoint sites as well as Teams. 

Once the web part add-in has been installed, a SharePoint administrator needs to deploy the app to all SharePoint sites as well as make the web parts available in Teams.

{{% alert title="SharePoint administrator needed" color="secondary" %}}
To access SharePoint app catalog you need to be a SharePoint administrator.
{{% /alert %}}

#### 1. Go to the SharePoint app catalog. (From the SharePoint admin center, https://\<your tenant name>-admin.sharepoint.com/_layouts/15/online/AdminHome.aspx#/ home -> More Features -> Apps. 

{{< imgproc appCatalog Resize "880x" >}}
{{< /imgproc >}}

#### 2. On the "Apps" page, click "App Catalog" and then "Apps for SharePoint".


#### 3. In the "Apps for SharePoint page", select MeetingRoomMap webparts row in the list, then select the "Files" tab and click the "Deploy" button. Ensure the "Make this solution available to all sites in the organization" is selected in the "Do you trust MeetingRoomMap webparts?" pop-up dialog.

{{< imgproc spappcatalog Resize "880x" >}}
{{< /imgproc >}}

#### 3. Once the web parts are deployed, then click the "Sync to Teams" button in the "Files" tab ribbon. 


## Adding web parts to SharePoint and Teams

### SharePoint 

When the web parts have been installed and sync'ed to Teams, they can be added to any modern SharePoint page. Search for 'mrm' to quickly  look up the three MeetingRoomMap webparts:

{{< imgproc add_webpart Resize "880x" >}}
{{< /imgproc >}}

Use web part properties to configure how the web part should behave (search mode or fixed location etc.):

{{< imgproc webpart_props Resize "880x" >}}
{{< /imgproc >}}

### Teams

The web parts can also be added as a Teams tab (either in a Channel or as a 'Personal' tab):

{{< imgproc addToTeamsTab Resize "880x" >}}
{{< /imgproc >}}


{{< imgproc teamsTab Resize "880x" >}}
{{< /imgproc >}}
