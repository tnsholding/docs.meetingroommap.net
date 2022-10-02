---
title: "Usage"
linkTitle: "View usage"
tags: ["AdminSite", "Usage"]
weight: 150
description: >
  View usage of MeetingRoomMap across the organization 
---

View usage of MeetingRoomMap API actions - these actions can be invoked by both the admin web site as well as usage of add-ins.  
The Basic and Standard plans are using actions to count 'searches' for billing, when searches exceeds the search limits included in the plan - see [https://www.meetingroommap.net/pricing](https://www.meetingroommap.net/pricing). 

To view usage go to [Admin web site -> Account -> Usage](https://www.meetingroommap.net/usage)

## Usage views

It's possible to select three different time scales for viewing usage history:

- Last 24 hours
- Last week
- Last month

Log data are only kept for one month, so it will not be possibly to create views of usage going further back in time. 

## Usage information

Log information is recorded with a major category and detailed action within that category, i.e. "CustomLocation.FindByName" (major category 'Custom locations' and detailed action 'find a custom location by name').

Below is a description of the different actions recorded.

#### Custom locations log entries

| Log entry                          | Description                                                                  | Count as search |
|------------------------------------|------------------------------------------------------------------------------|-----------------|
| CustomLocation.AttachToImage       | Map a custom location to a specific image/floorplan                          | No              |
| CustomLocation.CreateImage         | Create image with pushpin indication of custom location on floorplan         | Yes             |
| CustomLocation.Details             | Get all details including image with location for a specific custom location | Yes             |
| CustomLocation.FindByName          | Find a specific custom location by name                                      | Yes             |
| CustomLocation.GetList             | Get a list of all custom locations                                           | Yes             |
| CustomLocation.GetListByCategories | Get a list of all custom locations within a specific category                | Yes             |
| CustomLocation.GetListByImage      | Get a list of all custom locations mapped to a specific image/floorplan      | Yes             |
| CustomLocation.RemoveFromImage     | Remove a custom location from image/floorplan                                | No              |


#### Images/floorplans log entries

| Log entry    | Description                                        | Count as search |
|--------------|----------------------------------------------------|-----------------|
| Image.Delete | Delete an image (including all items mapped to it) | No              |
| Image.Upload | Upload a new image/floorpan                        | No              |


#### Meeting room log entries

| Log entry                   | Description                                                                          | Count as search |
|-----------------------------|--------------------------------------------------------------------------------------|-----------------|
| MeetingRoom.AttachToImage   | Attach a meeting room to a specific image/floorplan                                  | No              |
| MeetingRoom.CreateImage     | Create image with push pin indication of meeting room location                       | Yes             |
| MeetingRoom.CreateImageAnon | Create anonymous meeting room image link for embedding in meeting request            | Yes             |
| MeetingRoom.FindByImage     | Get a list of all meeting rooms mapped to a specific image/floorplan                 | Yes             |
| MeetingRoom.NextMeetings    | Get list of users next meetings including images with locations (used by Teams Bot ) | Yes             |
| MeetingRoom.RemoveFromImage | Remove a meeting room from an image/floorplan                                        | No              |
| MeetingRoom.RoomByName      | Get details and image with location for a specific meeting room                      | Yes             |
| MeetingRoom.RoomDetails     | Get all details including image with location for a specific meeting room            | Yes             |
| MeetingRoom.RoomList        | Get a list of all meeting rooms from Azure AD                                        | Yes             |

#### Reservations log entries

| Log entry                          | Description                                                    | Count as search |
|------------------------------------|----------------------------------------------------------------|-----------------|
| Reservations.CancelReservation     | Cancel a reservation                                           | No              |
| Reservations.CreateReservation     | Create a new reservation                                       | Yes             |
| Reservations.GetActiveReservations | Get a list of active reservations for a specific time inverval | Yes             |
| Reservations.GetAllReservations    | Get a list of all reservations                                 | Yes             |
| Reservations.GetReservations       | Get all reservations for a specific item (desk)                | Yes             |
| Reservations.GetReservationsByTeam | Get list of reservations for all users within a specific team  | Yes             |
| Reservations.GetReservationsByUser | Get list of reservations for a specific user                   | Yes             |



#### Person location log entries

| Log entry                      | Description                                                                         | Count as search |
|--------------------------------|-------------------------------------------------------------------------------------|-----------------|
| OfficeLocation.AttachToImage   | Attach a person/office location to a specific image/floorplan                       | No              |
| OfficeLocation.CreateImage     | Create image with push pin indication of person/office location                     | Yes             |
| OfficeLocation.GetDetails      | Get all details including image with location for a specific person/office location | Yes             |
| OfficeLocation.RemoveFromImage | Removes a person/office location from image/floorplan                               | No              |
| Person.GetImage                | Get details and image with location for a specific person                           | Yes             |
| Person.Search                  | Returns list of people by searching name/email                                      | Yes             |


#### License and general settings log entries

| Log entry                      | Description                                        | Count as search |
|--------------------------------|----------------------------------------------------|-----------------|
| License.ActivateSubscription   | When new subscription is activated                 | No              |
| License.DeactivateSubscription | When subscription is deactivated                   | No              |
| License.UpdateSubscription     | When subscription is updated (changing plans etc.) | No              |
| Tenant.UpdateSettings          | Updates to general settings                        | No              |


