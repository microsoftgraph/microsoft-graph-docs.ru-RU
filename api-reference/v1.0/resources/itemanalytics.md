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
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="7249f-103">Тип ресурса Итеманалитикс</span><span class="sxs-lookup"><span data-stu-id="7249f-103">itemAnalytics resource type</span></span>

<span data-ttu-id="7249f-104">Ресурс **итеманалитикс** предоставляет аналитику о действиях, которые были выполнены для элемента.</span><span class="sxs-lookup"><span data-stu-id="7249f-104">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="7249f-105">Этот ресурс в настоящее время доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="7249f-105">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="7249f-106">Вы также можете использовать API [getActivitiesByInterval][] для получения аналитики через настраиваемый диапазон или интервал времени.</span><span class="sxs-lookup"><span data-stu-id="7249f-106">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="7249f-107">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="7249f-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="properties"></a><span data-ttu-id="7249f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7249f-108">Properties</span></span>

| <span data-ttu-id="7249f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7249f-109">Property</span></span>      | <span data-ttu-id="7249f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7249f-110">Type</span></span>                 | <span data-ttu-id="7249f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7249f-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="7249f-112">Аллтиме</span><span class="sxs-lookup"><span data-stu-id="7249f-112">allTime</span></span>       | <span data-ttu-id="7249f-113">[Итемактивитистат][]</span><span class="sxs-lookup"><span data-stu-id="7249f-113">[itemActivityStat][]</span></span> | <span data-ttu-id="7249f-114">Аналитика за сроком службы элемента.</span><span class="sxs-lookup"><span data-stu-id="7249f-114">Analytics over the the item's lifespan.</span></span>
| <span data-ttu-id="7249f-115">Ластсевендайс</span><span class="sxs-lookup"><span data-stu-id="7249f-115">lastSevenDays</span></span> | <span data-ttu-id="7249f-116">[Итемактивитистат][]</span><span class="sxs-lookup"><span data-stu-id="7249f-116">[itemActivityStat][]</span></span> | <span data-ttu-id="7249f-117">Аналитика за последние семь дней.</span><span class="sxs-lookup"><span data-stu-id="7249f-117">Analytics for the last seven days.</span></span>

[Итемактивитистат]: itemactivitystat.md
[itemActivityStat]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a><span data-ttu-id="7249f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7249f-120">JSON representation</span></span>

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
