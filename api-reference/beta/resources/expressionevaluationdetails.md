---
title: Тип ресурса Експрессионевалуатиондетаилс
description: Представляет сведения о выражении, сведения о результатах и свойствах.
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f2d14d19bee60581c65d43e81b5ec69acc53df0a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026978"
---
# <a name="expressionevaluationdetails-resource-type"></a>Тип ресурса Експрессионевалуатиондетаилс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о выражении, сведения о результатах и свойствах.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| выражение | String | Представляет выражение, которое было оценено. |
| expressionEvaluationDetails | Коллекция Експрессионевалуатиондетаилс | Представляет сведения об оценке выражения. |
| експрессионресулт | Boolean | Представляет значение результата текущего выражения. |
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


