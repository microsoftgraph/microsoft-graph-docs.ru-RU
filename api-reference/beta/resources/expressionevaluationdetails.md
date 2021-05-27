---
title: тип ресурса expressionEvaluationDetails
description: Представляет сведения об выражениях, результатах и свойствах.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: a2e2b2620f30234c23753ef743f14e55e29f6f91
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679902"
---
# <a name="expressionevaluationdetails-resource-type"></a>тип ресурса expressionEvaluationDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об выражениях, результатах и свойствах.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| выражение | String | Представляет выражение, которое было оценено. |
| expressionEvaluationDetails | коллекция expressionEvaluationDetails | Представляет сведения об оценке выражения. |
| expressionResult | Boolean | Представляет значение результата текущего выражения. |
| propertyToEvaluate | [propertyToEvaluate](propertytoevaluate.md) | Определяет имя свойства и значение этого свойства. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionEvaluationDetails",
  "baseType": null
}-->

```json
{
  "expression": "String",
  "expressionEvaluationDetails": [{"@odata.type": "microsoft.graph.expressionEvaluationDetails"}],
  "expressionResult": true,
  "propertyToEvaluate": {"@odata.type": "microsoft.graph.propertyToEvaluate"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expressionEvaluationDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


