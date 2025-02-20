---
title: "profileCardAnnotation resource type"
description: "Allows an administrator to customize the appearance of selected fields in a Microsoft 365 profile card."
ms.localizationpriority: medium
author: "rwaithera"
ms.subservice: "people"
doc_type: "resourcePageType"
ms.date: 06/10/2024
---

# profileCardAnnotation resource type

Allows an administrator to customize the appearance of selected fields in a Microsoft 365 profile card. The administrator can define a default display name String and a set of alternative translations for the languages supported in their organization.

## Properties

| Property     | Type                                                            | Description                                                                                                                       |
|:-------------|:----------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------|
|displayName   |String                                                           | If present, the value of this field is used by the profile card as the default property label in the experience (for example, "Cost Center"). |
|localizations |[displayNameLocalization](displaynamelocalization.md) collection | Each resource in this collection represents the localized value of the attribute name for a given language, used as the default label for that locale. For example, a user with a `nb-NO` client gets "Kostnadssenter" as the attribute label, rather than "Cost Center."|

## JSON representation

The following JSON representation shows the resource type.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profileCardAnnotation",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "localizations": [{ "@odata.type": "microsoft.graph.displayNameLocalization" }]
}
```
