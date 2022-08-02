---
title: "membershipOutlierInsight resource type"
description: "In the Azure AD access reviews, the membershipOutlierInsight resource represents insights provided to reviewers based on whether a user is a peer outlier in relation to other group members."
author: "shubhamguptacal"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# membershipOutlierInsight resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Represents an insight provided to reviewers based on whether a user is a peer outlier in relation to other group members.

Inherits from [governanceInsight](governanceinsight.md).

## Properties
| Property    | Type   | Description |
| :---------------| :---------- | :---------- |
| memberId | String | Indicates the identifier of the user. |
| containerId | String | Indicates the identifier of the container, for example, a group ID. |
| outlierContainerType | outlierContainerType | Indicates the type of container. The possible values are: `group`, `unknownFutureValue`. |
| outlierMemberType | outlierMemberType | Indicates the type of outlier member. The possible values are: `user`, `unknownFutureValue`. |

## Relationships

|Relationship|Type|Description|
|:---|:---|:---|
|container|[directoryObject](../resources/directoryobject.md)| Navigation link to container directory object. For example: group|
|member|[directoryObject](../resources/directoryobject.md)| Navigation link to member object. For example : user|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.membershipOutlierInsight",
  "baseType": "microsoft.graph.governanceInsight",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.membershipOutlierInsight",
  "id": "String (identifier)",
  "insightCreatedDateTime": "String (timestamp)",
  "memberId": "String",
  "containerId": "String",
  "outlierContainerType": "String",
  "outlierMemberType": "String"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "membershipOutlierInsight resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
