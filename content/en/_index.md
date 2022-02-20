
---
title: "Documentation"
linkTitle: "Documentation"
type: "docs"
tags: ["intro"]
weight: 20

cascade:
- _target:
    path: "/blog/**"
  type: "blog"
  # set to false to include a blog section in the section nav along with docs
  toc_root: true
- _target:
    path: "/**"
    kind: "page"
  type: "docs"
- _target:
    path: "/**"
    kind: "section"
  type: "docs"
- _target:
    path: "/**"
    kind: "section"
  type: "home"
---

This is the documentation site for MeetingRoomMap. MeetingRoomMap is a Software as a Service (SaaS) solution to visually show locations on your own floorplans. Floorplans are uploaded as images. The following types of locations can be mapped:

* Meeting rooms (automatically listed from the meeting rooms defined in Office 365)

* People (automatically listed from Azure AD)

* Custom locations (your own categories of locations, i.e. printers, desks, fire extinguisher,
defibrillators)

</br>
The MeetingRoomMap suite consists of: </br></br>

* An admin web site (https://www.meetingroommap.net) to upload your own floorplan images and visually map locations to these floorplans.

* A series of Office add-ins for Outlook, Teams, and SharePoint to search and display the mapped locations.

* A reservation system for handling reservations based on visually making a reservation of mapped entities (i.e. of desks in a flexible office setup). The reservations system is integrated as an app for Microsoft Teams.


## Where should I go next?

* [Getting Started](/getting-started/): Go to the 'Getting Started' section to get help setting up MeetingRoomMap in your company.
* [Admin Core tasks](/tasks/): Check out the guide for common tasks in the admin web site.
* [Using the add-ins](/addins/): See this section for using the different add-ins.


