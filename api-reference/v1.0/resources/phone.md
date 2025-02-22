---
title: "phone resource type"
description: "Represents a phone number."
ms.localizationpriority: medium
author: "jumasure"
ms.prod: "directory-management"
doc_type: resourcePageType
---

# phone resource type

Namespace: microsoft.graph

Represents a phone number.


## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|number|string|The phone number.|
|type|phoneType|The type of phone number. The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.|

## JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phone"
}-->

```json
{
  "number": "string",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

