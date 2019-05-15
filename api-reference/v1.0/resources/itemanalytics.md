---
author: daspek
ms.author: dspektor
title: Тип ресурса Итеманалитикс
description: Объект Итеманалитикс предоставляет аналитику о действиях, которые были выполнены над элементом.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5c716f8faaafffe6afd75987843e6b614f5d6552
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970795"
---
# <a name="itemanalytics-resource-type"></a>Тип ресурса Итеманалитикс

Ресурс **итеманалитикс** предоставляет аналитику о действиях, которые были выполнены для элемента. Этот ресурс в настоящее время доступен только в SharePoint и OneDrive для бизнеса.

Вы также можете использовать API [getActivitiesByInterval][] для получения аналитики через настраиваемый диапазон или интервал времени.

>**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).

## <a name="properties"></a>Свойства

| Свойство      | Тип                 | Описание
|:--------------|:---------------------|:--------------------------------------
| Аллтиме       | [Итемактивитистат][] | Аналитика за сроком службы элемента.
| Ластсевендайс | [Итемактивитистат][] | Аналитика за последние семь дней.

[Итемактивитистат]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

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
