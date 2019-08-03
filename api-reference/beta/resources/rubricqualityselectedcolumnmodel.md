---
title: Тип ресурса Рубриккуалитиселектедколумнмодел
description: Указывает Рубриклевел, выбранный преподавателем при ступенчатом Едукатионрубрик
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6fd6ff5d9def23a6a6fb180c8d12398437e5dce0
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173295"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a>Тип ресурса Рубриккуалитиселектедколумнмодел

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает [рубриклевел](rubriclevel.md) , выбранный преподавателем при ступенчатом [едукатионрубрик](educationrubric.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|columnId|String|Идентификатор выбранного уровня для этого качества.|
|Куалитид|String|Идентификатор связанного качества.|

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