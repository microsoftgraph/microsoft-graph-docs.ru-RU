---
title: Тип ресурса teamFunSettings
description: Параметры для настройки использования Giphy, memes и наклейки рабочих групп.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: dc8d4cfa05f7bc6cbda9dfbf5d113370a1981ba5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515862"
---
# <a name="teamfunsettings-resource-type"></a>Тип ресурса teamFunSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры для настройки использования Giphy, memes и наклейки в [группы](team.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowGiphy|Логическое|Если присвоено значение true, позволяет использовать Giphy.|
|giphyContentRating|String (enum)|Оценка контента Giphy. Возможные значения: `moderate`, `strict`.|
|allowStickersAndMemes|Логическое|Если параметр имеет значение true, позволяет пользователям включают в себя наклейки и memes.|
|allowCustomMemes|Логическое|Если задано значение true, предоставляет пользователям возможность включать настраиваемых memes.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamfunsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
