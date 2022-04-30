---
title: "MeetingRooms"
linkTitle: "Mapping MeetingRooms"
tags: ["AdminSite", "MeetingRooms"]
weight: 20
description: >
  Assign Exchange meeting rooms to floorplans
---

A mapped meeting room can be displayed in the Outlook add-in when editing or viewing a meeting as well as being searched and viewed in the Teams and SharePoint add-ins.

## Rooms and room lists

The list of rooms to map is automatically fetched from Exchange in Office 365. The rooms must be defined in Exchange as a resource of type "Room" to show up in MeetingRoomMap.

Rooms can optionally be organized in room lists - see [https://docs.microsoft.com/en-us/exchange/recipients/room-mailboxes?view=exchserver-2019#create-a-room-list](https://docs.microsoft.com/en-us/exchange/recipients/room-mailboxes?view=exchserver-2019#create-a-room-list)

## Mapping rooms to floorplans

Mapping a meeting room to a floorplan can be done in two ways in the admin web site:

1) Per image/floorplan from [Images](https://www.meetingroommap.net/MapImage) page by clicking "Attach rooms" button for an image"
2) From the [Rooms](https://www.meetingroommap.net/Rooms) page.

### 1. Mapping from Image list

Mappings can be done per floorplan by going to the [Images](https://www.meetingroommap.net/MapImage) page and clicking "Attach rooms" button for a selected floorplan:

1) On the "Edit room map" page select a room in the Room dropdown - if rooms are organized in room lists, first select a room list, then a room. 
2) Once a room is selected click "Attach" button. 
3) A popup windows with the floorplan is opened - click the location of the meeting room to create the mapping.

{{< imgproc map_per_image Resize "880x" >}}
{{< /imgproc >}}

#### Removing mapping

An existing mapping can be removed by clicking the "Remove" button in the "Rooms in this map" list (NB. Requires the role "MeetingRoomEditor" to be able to remove).



### 2. Mapping from Rooms page

Alternatively, mappings can be done by viewing the complete list of known rooms on the [Rooms](https://www.meetingroommap.net/Rooms) page.

1) Find the room to map in the list (use sorting, paging and search to quickly find the correct room)
2) Click "Attach to map" button
3) A popup "Select map to attach to" with all available floorplans displays - click the floorplan to map to
4) A popup windows with the floorplan is opened - click the location of the meeting room to create the mapping

#### Removing mapping

An existing mapping can be removed by clicking the "Remove" button for a specific room in the list. (NB. The button only displays for users with the role "MeetingRoomEditor").
