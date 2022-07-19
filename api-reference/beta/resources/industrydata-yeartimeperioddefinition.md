---
title: "yearTimePeriodDefinition resource type"
description: "Defines annual time periods such as academic or fiscal years."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=API/Document/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=API/Document/Guidelines/Metadata)**"
doc_type: resourcePageType
---

# yearTimePeriodDefinition resource type

Namespace: microsoft.graph.industryData

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Defines annual time periods such as academic or fiscal years.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List yearTimePeriodDefinitions](../api/industrydata-inboundfileflow-list-year.md)|[microsoft.graph.industryData.yearTimePeriodDefinition](../resources/industrydata-yeartimeperioddefinition.md) collection|Get a list of the [yearTimePeriodDefinition](../resources/industrydata-yeartimeperioddefinition.md) objects and their properties.|
|[Create yearTimePeriodDefinition](../api/industrydata-inboundfileflow-post-year.md)|[microsoft.graph.industryData.yearTimePeriodDefinition](../resources/industrydata-yeartimeperioddefinition.md)|Create a new [yearTimePeriodDefinition](../resources/industrydata-yeartimeperioddefinition.md) object.|
|[Get yearTimePeriodDefinition](../api/industrydata-yeartimeperioddefinition-get.md)|[microsoft.graph.industryData.yearTimePeriodDefinition](../resources/industrydata-yeartimeperioddefinition.md)|Read the properties and relationships of a [yearTimePeriodDefinition](../resources/industrydata-yeartimeperioddefinition.md) object.|
|[Update yearTimePeriodDefinition](../api/industrydata-yeartimeperioddefinition-update.md)|[microsoft.graph.industryData.yearTimePeriodDefinition](../resources/industrydata-yeartimeperioddefinition.md)|Update the properties of a [yearTimePeriodDefinition](../resources/industrydata-yeartimeperioddefinition.md) object.|
|[Delete yearTimePeriodDefinition](../api/industrydata-inboundfileflow-delete-year.md)|None|Deletes a [yearTimePeriodDefinition](../resources/industrydata-yeartimeperioddefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The name of the year.|
|endDate|Date|The last day of the year. ISO 8601 date.|
|startDate|Date|The first day of the year. ISO 8601 date.|
|year|[microsoft.graph.industryData.yearReferenceValue](../resources/industrydata-yearreferencevalue.md)|Pointer to a year entry in the referenceDefinition collection.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.industryData.yearTimePeriodDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.industryData.yearTimePeriodDefinition",
  "displayName": "String",
  "endDate": "Date",
  "startDate": "Date",
  "year": {
    "@odata.type": "microsoft.graph.industryData.yearReferenceValue"
  }
}
```

