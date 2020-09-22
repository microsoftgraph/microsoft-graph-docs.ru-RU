---
title: Тип ресурса Рубриккуалити
description: Качество Rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1773bfb40e7857b65272cbf611cb7394b019197e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016111"
---
# <a name="rubricquality-resource-type"></a>Тип ресурса Рубриккуалити

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Качество Rubric. Описание связи между Rubric *качеством*, *уровнями*и *критериями*можно узнать в разделе [едукатионрубрик](educationrubric.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|criteria|Коллекция [рубриккритерион](rubriccriterion.md)|Коллекция критериев для этого качества Rubric.|
|description|[itemBody](itembody.md)|Описание этого качества Rubric.|
|displayName|String|Имя этого rubricного качества.|
|куалитид|String|ИДЕНТИФИКАТОР этого ресурса.|
|weight|Одинарное|Если задано, числовой вес для этого качества.  Весовые значения должны добавим до 100.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQuality",
  "baseType": null
}-->

```json
{
  "criteria": [{"@odata.type": "microsoft.graph.rubricCriterion"}],
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "qualityId": "String",
  "weight": "Double"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

