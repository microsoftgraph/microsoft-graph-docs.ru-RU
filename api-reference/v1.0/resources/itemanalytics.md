---
author: daspek
ms.author: dspektor
title: Тип ресурса Итеманалитикс
description: Объект Итеманалитикс предоставляет аналитику о действиях, которые были выполнены над элементом.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a18d12bd2b431d147f2d23ea2c958cd75078c9a8
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620418"
---
# <a name="itemanalytics-resource-type"></a>Тип ресурса Итеманалитикс

Ресурс **итеманалитикс** предоставляет аналитику о действиях, которые были выполнены для элемента. Этот ресурс в настоящее время доступен только в SharePoint и OneDrive для бизнеса.

Вы также можете использовать API [getActivitiesByInterval][] для получения аналитики через настраиваемый диапазон или интервал времени.

>**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).

## <a name="properties"></a>Свойства

| Свойство      | Тип                 | Описание
|:--------------|:---------------------|:--------------------------------------
| Аллтиме       | [itemActivityStat][] | Аналитика за сроком службы элемента.
| Ластсевендайс | [itemActivityStat][] | Аналитика за последние семь дней.

[itemActivityStat]: itemactivitystat.md
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
