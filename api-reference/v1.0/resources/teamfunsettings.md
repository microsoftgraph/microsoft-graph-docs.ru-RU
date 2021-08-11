---
title: тип ресурса teamFunSettings
description: Параметры для настройки использования Giphy, мемов и наклеек в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 62e944143bc7dd6eac13c911b38872708777dd76dc6a812869d9e0b0655bc38d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129969"
---
# <a name="teamfunsettings-resource-type"></a>тип ресурса teamFunSettings

Пространство имен: microsoft.graph



Параметры для настройки использования Giphy, мемов и стикеров в [команде](team.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowGiphy|Логическое|Если установлено для true, включает использование Giphy.|
|giphyContentRating|String (enum)|Оценка контента Giphy. Возможные значения: `moderate`, `strict`.|
|allowStickersAndMemes|Логическое|Если установлено верно, позволяет пользователям включать наклейки и мемы.|
|allowCustomMemes|Логический|Если установлено, что это так, пользователи могут включать настраиваемые мемы.|

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

