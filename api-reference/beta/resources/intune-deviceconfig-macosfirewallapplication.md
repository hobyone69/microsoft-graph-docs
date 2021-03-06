---
title: "macOSFirewallApplication resource type"
description: "Represents an app in the list of macOS firewall applications"
localization_priority: Normal
author: "tfitzmac"
ms.prod: "Intune"
---

# macOSFirewallApplication resource type

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change. Use of these APIs in production applications is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Represents an app in the list of macOS firewall applications

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bundleId|String|BundleId of the application.|
|allowsIncomingConnections|Boolean|Whether or not incoming connections are allowed.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSFirewallApplication"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSFirewallApplication",
  "bundleId": "String",
  "allowsIncomingConnections": true
}
```




