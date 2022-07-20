---
title: "industryDataRunActivity resource type"
description: "This entity is the base class for all activity types. Activities provide read-only information about the execution of flows either in the past or currently executing."
author: "mlafleur"
ms.localizationpriority: medium
ms.prod: "industrydata"
doc_type: resourcePageType
---

# industryDataRunActivity resource type

Namespace: microsoft.graph.industryData

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

This entity is the base class for all activity types. Activities provide read-only information about the execution of flows either in the past or currently executing.
This is an abstract type.

## Methods

| Method                                                                                   | Return type                                                                                                             | Description                                                                                                                         |
| :--------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------- |
| [List industryDataRunActivities](../api/industrydata-industrydatarun-list-activities.md) | [microsoft.graph.industryData.industryDataRunActivity](../resources/industrydata-industrydatarunactivity.md) collection | Get a list of the [industryDataRunActivity](../resources/industrydata-industrydatarunactivity.md) objects and their properties.     |
| [Get industryDataRunActivity](../api/industrydata-industrydatarunactivity-get.md)        | [microsoft.graph.industryData.industryDataRunActivity](../resources/industrydata-industrydatarunactivity.md)            | Read the properties and relationships of an [industryDataRunActivity](../resources/industrydata-industrydatarunactivity.md) object. |

## Properties

| Property      | Type                                                       | Description                                                                                                                                                                    |
| :------------ | :--------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| blockingError | [microsoft.graph.publicError](../resources/publicerror.md) | An error object to diagnose critical failures in a activity .                                                                                                                  |
| displayName   | String                                                     | The name of the flow being executed.                                                                                                                                           |
| status        | industryDataActivityStatus                                 | Current status of the activity .The possible values are: `inProgress`, `skipped`, `failed`, `completed`, `completedWithErrors`, `completedWithWarnings`, `unknownFutureValue`. |

## Relationships

| Relationship | Type                                                                      | Description                      |
| :----------- | :------------------------------------------------------------------------ | :------------------------------- |
| activity     | [industryDataActivity](../resources/industrydata-industrydataactivity.md) | The flow this activity executed. |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.industryData.industryDataRunActivity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.industryData.industryDataRunActivity",
  "blockingError": {
    "@odata.type": "microsoft.graph.publicError"
  },
  "displayName": "String",
  "status": "String"
}
```
