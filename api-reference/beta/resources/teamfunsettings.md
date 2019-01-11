---
title: Тип ресурса teamFunSettings
description: Параметры для настройки использования Giphy, memes и наклейки рабочих групп.
localization_priority: Normal
ms.openlocfilehash: c53d3215e5f515361c66fe2d3d0ad10a5338e0c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852068"
---
# <a name="teamfunsettings-resource-type"></a>Тип ресурса teamFunSettings

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Параметры для настройки использования Giphy, memes и наклейки в [группы](team.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowGiphy|Логический|Если присвоено значение true, позволяет использовать Giphy.|
|giphyContentRating|String (enum)|Оценка контента Giphy. Возможные значения: `moderate`, `strict`.|
|allowStickersAndMemes|Логический|Если параметр имеет значение true, позволяет пользователям включают в себя наклейки и memes.|
|allowCustomMemes|Логический|Если задано значение true, предоставляет пользователям возможность включать настраиваемых memes.|

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
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
