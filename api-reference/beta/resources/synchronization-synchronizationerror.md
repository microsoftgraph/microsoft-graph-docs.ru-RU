---
title: Тип ресурса synchronizationError
description: Представляет ошибки, возникшей во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: f37dca5b65a67eb36b2b6a130eee8feb692cd271
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513174"
---
# <a name="synchronizationerror-resource-type"></a>Тип ресурса synchronizationError

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ошибки, возникшей во время синхронизации.

## <a name="properties"></a>Свойства

<!-- Add descriptions for the properties. -->
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|code|String||
|message|String||
|tenantActionable|Логическое||

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
