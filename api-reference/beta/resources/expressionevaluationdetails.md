---
title: тип ресурса expressionEvaluationDetails
description: Представляет сведения об выражениях, результатах и свойствах.
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: d588719e8d6bcf32ff337beec8815b6fe329ee0b
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587044"
---
# <a name="expressionevaluationdetails-resource-type"></a>тип ресурса expressionEvaluationDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об выражениях, результатах и свойствах.

## <a name="properties"></a>Свойства

| Свойство                    | Тип                                        | Описание                                                      |
| :-------------------------- | :------------------------------------------ | :--------------------------------------------------------------- |
| выражение                  | Строка                                      | Представляет выражение, которое было оценено.                  |
| expressionEvaluationDetails | коллекция expressionEvaluationDetails      | Представляет сведения об оценке выражения.      |
| expressionResult            | Логическое                                     | Представляет значение результата текущего выражения.    |
| propertyToEvaluate          | [propertyToEvaluate](propertytoevaluate.md) | Определяет имя свойства и значение этого свойства. |

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
  "expressionEvaluationDetails": [
    { "@odata.type": "microsoft.graph.expressionEvaluationDetails" }
  ],
  "expressionResult": true,
  "propertyToEvaluate": { "@odata.type": "microsoft.graph.propertyToEvaluate" }
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
