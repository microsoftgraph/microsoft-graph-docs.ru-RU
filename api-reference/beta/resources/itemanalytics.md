---
author: daspek
description: Ресурс itemAnalytics предоставляет аналитику действий, выполненных с элементом. В настоящее время этот ресурс доступен только в SharePoint и OneDrive для бизнеса.
ms.date: 09/14/2017
title: ItemAnalytics
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 15bd59f04384f2b18329f581f568ee465a86c040
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176927"
---
# <a name="itemanalytics-resource-type"></a>Тип ресурса itemAnalytics

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **itemAnalytics** предоставляет аналитику действий, выполненных с элементом. В настоящее время этот ресурс доступен только в SharePoint и OneDrive для бизнеса.

Вы также можете использовать API [getActivitiesByInterval][] для получения аналитики за настраиваемый диапазон времени или интервал.

>**Примечание:** Ресурс **itemAnalytics** пока доступен не во всех национальных [развертываниях](/graph/deployments).

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemAnalytics",
  "@type.aka": "oneDrive.analytics"
}-->

```json
{
  "allTime": {"@odata.type": "microsoft.graph.itemActivityStat"},
  "lastSevenDays": {"@odata.type": "microsoft.graph.itemActivityStat"}
}
```

## <a name="properties"></a>Свойства

| Свойство      | Тип                 | Описание
|:--------------|:---------------------|:--------------------------------------
| allTime       | [itemActivityStat][] | Аналитика на протяжении жизненного цикла элемента.
| lastSevenDays | [itemActivityStat][] | Аналитика за последние семь дней.

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

<!--
{
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics",
  "suppressions": []
}
-->


