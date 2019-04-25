---
title: Тип ресурса Стрингкэйобжектвалуепаир
description: Представляет собой запись "ключ-значение", в которой ключ является строкой, а значение — произвольным объектом JSON. Это открытый тип OData, который предполагает наличие свойства с именем `value` , которое является допустимым объектом JSON.
localization_priority: Normal
ms.openlocfilehash: 8f939c177f2130813c6080d46ad78664f6118857
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523219"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a>Тип ресурса Стрингкэйобжектвалуепаир

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет собой запись "ключ-значение", в которой ключ является строкой, а значение — произвольным объектом JSON. Это открытый тип OData, который предполагает наличие свойства с именем `value` , которое является допустимым объектом JSON.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ключа|String|Ключ.|
|значение|Любые|Произвольный объект JSON.|

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
  "key": "String"
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
