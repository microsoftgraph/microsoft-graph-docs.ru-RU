---
title: Тип ресурса Експрессионевалуатиондетаилс
description: Представляет сведения о выражении, сведения о результатах и свойствах.
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 347e356bda19228ea8b3738b5bf8b72f57da95f7
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272850"
---
# <a name="expressionevaluationdetails-resource-type"></a>Тип ресурса Експрессионевалуатиондетаилс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о выражении, сведения о результатах и свойствах.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| выражение | String | Представляет выражение, которое было оценено. |
| експрессионевалуатиондетаилс | Коллекция Експрессионевалуатиондетаилс | Представляет сведения об оценке выражения. |
| експрессионресулт | Логический | Представляет значение результата текущего выражения. |
| пропертитоевалуате | [пропертитоевалуате](propertytoevaluate.md) | Определяет имя свойства и значение этого свойства. |

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
