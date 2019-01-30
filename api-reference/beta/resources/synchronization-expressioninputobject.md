---
title: Тип ресурса expressionInputObject
description: 'Представляет объект для использования в качестве входного тестовых данных при [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) действие выполняется вычисление выражения.'
localization_priority: Normal
ms.openlocfilehash: 3e631102505408b955404c4badb33b98f314236f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641654"
---
# <a name="expressioninputobject-resource-type"></a>Тип ресурса expressionInputObject

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет объект для использования в качестве входного тестовых данных при [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) действие выполняется вычисление выражения.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|definition|[objectDefinition](synchronization-objectdefinition.md)|Определение объекта теста.|
|properties|[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) коллекции|Значения свойств объекта теста.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionInputObject"
}-->

```json
{
  "definition": {"@odata.type": "microsoft.graph.objectDefinition"},
  "properties": [{"@odata.type": "microsoft.graph.stringKeyObjectValuePair"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-expressioninputobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
