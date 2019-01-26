---
title: Тип ресурса stringKeyObjectValuePair
description: Представляет пару ключ значение, где ключ — это строка, а значение — это произвольный объект JSON. Это открытого типа OData, который будет использовать свойство с именем `value` то есть допустимый объект JSON.
localization_priority: Normal
ms.openlocfilehash: 819a2e004ee712f1250652ce0b3811940545e643
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572173"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a>Тип ресурса stringKeyObjectValuePair

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пару ключ значение, где ключ — это строка, а значение — это произвольный объект JSON. Это открытого типа OData, который будет использовать свойство с именем `value` то есть допустимый объект JSON.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|key|Строка|Ключ.|
|value|Json|Произвольный объект JSON.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String",
  "value":"Json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeyobjectvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
