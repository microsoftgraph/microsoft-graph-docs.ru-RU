---
title: Тип ресурса Медиапромпт
description: Тип Медиапромпт.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b87af39d6d6ac4879aba44573b920a43d4f92145
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562597"
---
# <a name="mediaprompt-resource-type"></a>Тип ресурса Медиапромпт

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип Медиапромпт.

## <a name="properties"></a>Свойства

| Свойство    | Тип                      | Описание                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| CNAME        | Int32                     | Число циклов. значение 0 указывает, что цикл должен быть бесконечным. Значение по умолчанию — `1`. |
| Медиаинфо   | [Медиаинфо](mediainfo.md) | Сведения о мультимедиа                                                           |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "loop": 1024,
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

## <a name="example"></a>Пример

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->
```json
{
  "mediaInfo": {
    "uri": "https://cdn.contoso.com/beep.wav",
    "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
  },
  "loop": 5
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mediaprompt.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
