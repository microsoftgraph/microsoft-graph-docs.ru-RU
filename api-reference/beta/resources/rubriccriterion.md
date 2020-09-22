---
title: Тип ресурса Рубриккритерион
description: Критерий Rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 60123251d771d06032077231250efe53b35a787c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016116"
---
# <a name="rubriccriterion-resource-type"></a>Тип ресурса Рубриккритерион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Критерий Rubric. Описание связи между Rubric *качеством*, *уровнями*и *критериями*можно узнать в разделе [едукатионрубрик](educationrubric.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|[itemBody](itembody.md)|Описание этого критерия.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricCriterion",
  "baseType": null
}-->

```json
{
  "description": {"@odata.type": "microsoft.graph.itemBody"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricCriterion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

