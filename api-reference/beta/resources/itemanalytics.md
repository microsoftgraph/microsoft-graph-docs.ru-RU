---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
ms.openlocfilehash: 03626b5dad041181558af076b5dc0ac05b684e13
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842415"
---
# <a name="itemanalytics-resource-type"></a>Тип ресурса itemAnalytics

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **itemAnalytics** предоставляет analytics о действиях, выполняемых над элементом. Этот ресурс в данный момент доступна только на сервере SharePoint и OneDrive для бизнеса.

Можно также использовать [getActivitiesByInterval][] API для извлечения analytics через интервала времени или интервал.

>**Примечание:** **ItemAnalytics** ресурсов, пока недоступна во всех [Национальный развертываний](/graph/deployments).

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
| allTime       | [itemActivityStat][] | Аналитика по зависящая от элемента.
| lastSevenDays | [itemActivityStat][] | Анализ для за последние семь дней.

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

<!-- {
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics"
} -->
