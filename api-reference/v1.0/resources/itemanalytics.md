---
author: daspek
title: Тип ресурса itemAnalytics
description: Объект ItemAnalytics предоставляет аналитику действий, которые произошли на элементе.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a9f1e6a70829d809feb6784441744ed74f8ea0d2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084346"
---
# <a name="itemanalytics-resource-type"></a>Тип ресурса itemAnalytics

Пространство имен: microsoft.graph

Ресурс **itemAnalytics** предоставляет аналитику действий, которые произошли на элементе. В настоящее время этот ресурс доступен только в SharePoint и OneDrive для бизнеса.

Вы также можете использовать [API getActivitiesByInterval][] для получения аналитики в настраиваемом диапазоне времени или интервале.

>**Примечание:** Ресурс **itemAnalytics** еще не доступен во всех [национальных развертываниях.](/graph/deployments)

## <a name="properties"></a>Свойства

| Свойство      | Тип                 | Описание
|:--------------|:---------------------|:--------------------------------------
| allTime       | [itemActivityStat][] | Аналитика продолжительности жизни элемента.
| lastSevenDays | [itemActivityStat][] | Аналитика за последние семь дней.

[itemActivityStat]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemAnalytics",
  "@type.aka&quot;: &quot;oneDrive.analytics"
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

