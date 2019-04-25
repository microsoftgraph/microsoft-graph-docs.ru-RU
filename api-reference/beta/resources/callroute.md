---
title: Тип ресурса Каллрауте
description: Тип Каллрауте.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cfa470c4d3a03655221cab1f29baa60d00a8cf6c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543840"
---
# <a name="callroute-resource-type"></a>Тип ресурса Каллрауте

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип Каллрауте.

## <a name="properties"></a>Свойства

| Свойство            | Тип                          | Описание                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| Наконец               | [identitySet](identityset.md) | Идентификатор, разрешенный в вызове.               |
| Исходный текст            | [identitySet](identityset.md) | Идентификатор, который изначально использовался при вызове.           |
| Раутингтипе         | String                        | Возможные значения: `forwarded`, `lookup`, `selfFork`.  |

## <a name="json-representation"></a>Представление в формате JSON

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
