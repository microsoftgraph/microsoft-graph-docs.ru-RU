---
title: тип ресурса teamFunSettings
description: Параметры для настройки использования Giphy, мемов и наклеек в команде.
ms.localizationpriority: medium
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 169ecc9ff2e3dfc542a6d055b84234f7a3f98039
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134348"
---
# <a name="teamfunsettings-resource-type"></a>тип ресурса teamFunSettings

Пространство имен: microsoft.graph



Параметры для настройки использования Giphy, мемов и стикеров в [команде](team.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowGiphy|Логический|Если установлено для true, включает использование Giphy.|
|giphyContentRating|String (enum)|Оценка контента Giphy. Возможные значения: `moderate`, `strict`.|
|allowStickersAndMemes|Логический|Если установлено верно, позволяет пользователям включать наклейки и мемы.|
|allowCustomMemes|Boolean|Если установлено, что это так, пользователи могут включать настраиваемые мемы.|

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

