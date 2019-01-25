---
title: Тип ресурса callRoute
description: Тип callRoute.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cfa470c4d3a03655221cab1f29baa60d00a8cf6c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512803"
---
# <a name="callroute-resource-type"></a>Тип ресурса callRoute

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип callRoute.

## <a name="properties"></a>Свойства

| Свойство            | Тип                          | Описание                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| Final               | [identitySet](identityset.md) | Идентификатор, который был разрешен к в вызове.               |
| Original            | [identitySet](identityset.md) | Идентификатор, который изначально использовался в вызове.           |
| routingType         | String                        | Возможные значения: `forwarded`, `lookup`, `selfFork`.  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/callroute.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
