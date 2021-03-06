---
title: "scheduleInformation resource type"
description: " > **Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change. Use of these APIs in production applications is not supported."
localization_priority: Normal
---

# scheduleInformation resource type

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Represents the availability of a user, distribution list, or resource for a specified time period.

## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|availabilityView |String |Represents a merged view of availability of all the items in `scheduleItems`. The view consists of time slots. Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.|
|error |[freeBusyError](freebusyerror.md) |Error information from attempting to get the availability of the user, distribution list, or resource. |
|scheduleId |String |An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**. |
|scheduleItems |[scheduleItem](scheduleitem.md) collection |Contains the items that describe the availability of the user or resource. |
|workingHours |[workingHours](workinghours.md) |The days of the week and hours in a specific time zone that the user works. These are set as part of the user's [mailboxSettings](mailboxsettings.md).|


## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleInformation"
}-->

```json
{
  "availabilityView": "String",
  "error": {"@odata.type": "microsoft.graph.freeBusyError"},
  "scheduleId": "String",
  "scheduleItems": [{"@odata.type": "microsoft.graph.scheduleItem"}],
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
