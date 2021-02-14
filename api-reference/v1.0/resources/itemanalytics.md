---
author: daspek
title: Тип ресурса itemAnalytics
description: Объект ItemAnalytics предоставляет аналитические данные о действиях, которые произошли с элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 96ad65ef5cc8907663a9ca67e5ea2b7546b8fa03
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238661"
---
# <a name="itemanalytics-resource-type"></a>Тип ресурса itemAnalytics

Пространство имен: microsoft.graph

Ресурс **itemAnalytics** предоставляет аналитические данные о действиях, которые произошли с элементом. В настоящее время этот ресурс доступен только в SharePoint и OneDrive для бизнеса.

Вы также можете использовать API [getActivitiesByInterval][] для получения аналитики за настраиваемый диапазон времени или интервал.

>**Примечание.** Ресурс **itemAnalytics** пока не доступен во всех [национальных развертываниях.](/graph/deployments)

## <a name="properties"></a>Свойства

| Свойство      | Тип                 | Описание
|:--------------|:---------------------|:--------------------------------------
| allTime       | [itemActivityStat][] | Аналитика на протяжении жизненного срока элемента.
| lastSevenDays | [itemActivityStat][] | Аналитика за последние семь дней.

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

