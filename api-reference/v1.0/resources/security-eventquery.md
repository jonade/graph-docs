---
title: "eventQuery resource type"
description: "Represents the workload (SharePoint Online, OneDrive for Business, Exchange Online) and identification information associated with a retention event."
author: "sseth"
ms.localizationpriority: medium
ms.subservice: "security"
doc_type: resourcePageType
ms.date: 07/22/2024
---

# eventQuery resource type

Namespace: microsoft.graph.security
Represents the workload (SharePoint Online, OneDrive for Business, Exchange Online) and identification information associated with a retention event.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|queryType|microsoft.graph.security.queryType|Represents the type of query associated with an event. 'files' for SPO and ODB and 'messages' for EXO.The possible values are: `files`, `messages`, `unknownFutureValue`.|
|query|String|Represents unique identification for the  query. 'Asset ID' for SharePoint Online and OneDrive for Business, 'keywords' for Exchange Online.|

## Relationships
None.

## JSON representation
The following JSON representation shows the resource type.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.eventQuery"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.eventQuery",
  "queryType": "String",
  "query": "String"
}
```


