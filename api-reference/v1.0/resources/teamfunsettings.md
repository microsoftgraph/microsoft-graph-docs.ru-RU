---
title: Тип ресурса Теамфунсеттингс
description: Параметры для настройки использования Giphy, мемов и наклеек в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 696a6a3b02f90abe1456f99d9a40a4d9127b5697
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533550"
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
