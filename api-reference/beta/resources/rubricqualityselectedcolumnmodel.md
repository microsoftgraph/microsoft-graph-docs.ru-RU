---
title: Тип ресурса Рубриккуалитиселектедколумнмодел
description: Указывает Рубриклевел, выбранный преподавателем при ступенчатом Едукатионрубрик
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a381ad878f16dab6197c72bd19d6f5aeee86f4a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016060"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a>Тип ресурса Рубриккуалитиселектедколумнмодел

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает [рубриклевел](rubriclevel.md) , выбранный преподавателем при ступенчатом [едукатионрубрик](educationrubric.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|columnId|String|Идентификатор выбранного уровня для этого качества.|
|куалитид|String|Идентификатор связанного качества.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel",
  "baseType": null
}-->

```json
{
  "columnId": "String",
  "qualityId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQualitySelectedColumnModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

