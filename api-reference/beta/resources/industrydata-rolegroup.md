---
title: "roleGroup resource type"
description: "Represents a named collection of individual roles."
author: "mlafleur"
ms.localizationpriority: medium
ms.prod: "industrydata"
doc_type: resourcePageType
---

# roleGroup resource type

Namespace: microsoft.graph.industryData

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents a named collection of individual roles.

## Methods

| Method                                                                       | Return type                                                                                 | Description                                                                                            |
| :--------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------ | :----------------------------------------------------------------------------------------------------- |
| [List roleGroups](../api/industrydata-industrydatatenant-list-rolegroups.md) | [microsoft.graph.industryData.roleGroup](../resources/industrydata-rolegroup.md) collection | Get a list of the [roleGroup](../resources/industrydata-rolegroup.md) objects and their properties.    |
| [Get roleGroup](../api/industrydata-rolegroup-get.md)                        | [microsoft.graph.industryData.roleGroup](../resources/industrydata-rolegroup.md)            | Read the properties and relationships of a [roleGroup](../resources/industrydata-rolegroup.md) object. |

## Properties

| Property    | Type                                                                                                          | Description                                  |
| :---------- | :------------------------------------------------------------------------------------------------------------ | :------------------------------------------- |
| displayName | String                                                                                                        | The name of the role group.                  |
| roles       | [microsoft.graph.industryData.roleReferenceValue](../resources/industrydata-rolereferencevalue.md) collection | The set of roles included in the role group. |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.industryData.roleGroup",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.industryData.roleGroup",
  "displayName": "String",
  "roles": [
    {
      "@odata.type": "microsoft.graph.industryData.roleReferenceValue"
    }
  ]
}
```
