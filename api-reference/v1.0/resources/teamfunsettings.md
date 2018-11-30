---
title: Тип ресурса teamFunSettings
description: Параметры для настройки использования Giphy, memes и наклейки рабочих групп.
ms.openlocfilehash: ef816d027f015155cc09195c359523c83589725e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024796"
---
# <a name="teamfunsettings-resource-type"></a>Тип ресурса teamFunSettings



Параметры для настройки использования Giphy, memes и наклейки в [группы](team.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
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
