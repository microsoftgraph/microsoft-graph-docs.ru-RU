---
title: Тип ресурса Теамфунсеттингс
description: Параметры для настройки использования Giphy, мемов и наклеек в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 25f49eaff6485fd0d618a91ef942bc2dccf8c8da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094031"
---
# <a name="teamfunsettings-resource-type"></a>Тип ресурса Теамфунсеттингс

Пространство имен: microsoft.graph



Параметры для настройки использования Giphy, мемес и наклеек в [команде](team.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|алловгифи|Boolean|Если задано значение true, включается использование Giphy.|
|гификонтентратинг|String (enum)|Оценка содержимого Giphy. Возможные значения: `moderate`, `strict`.|
|алловстиккерсандмемес|Boolean|Если задано значение true, пользователям разрешается включать наклейки и мемес.|
|алловкустоммемес|Boolean|Если задано значение true, пользователи могут включать пользовательские мемес.|

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

