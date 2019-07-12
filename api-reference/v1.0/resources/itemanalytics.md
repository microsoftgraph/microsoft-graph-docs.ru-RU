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
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="ce04b-103">Тип ресурса Итеманалитикс</span><span class="sxs-lookup"><span data-stu-id="ce04b-103">itemAnalytics resource type</span></span>

<span data-ttu-id="ce04b-104">Ресурс **итеманалитикс** предоставляет аналитику о действиях, которые были выполнены для элемента.</span><span class="sxs-lookup"><span data-stu-id="ce04b-104">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="ce04b-105">Этот ресурс в настоящее время доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="ce04b-105">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="ce04b-106">Вы также можете использовать API [getActivitiesByInterval][] для получения аналитики через настраиваемый диапазон или интервал времени.</span><span class="sxs-lookup"><span data-stu-id="ce04b-106">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="ce04b-107">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="ce04b-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="properties"></a><span data-ttu-id="ce04b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce04b-108">Properties</span></span>

| <span data-ttu-id="ce04b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce04b-109">Property</span></span>      | <span data-ttu-id="ce04b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ce04b-110">Type</span></span>                 | <span data-ttu-id="ce04b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ce04b-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="ce04b-112">Аллтиме</span><span class="sxs-lookup"><span data-stu-id="ce04b-112">allTime</span></span>       | <span data-ttu-id="ce04b-113">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="ce04b-113">[itemActivityStat][]</span></span> | <span data-ttu-id="ce04b-114">Аналитика за сроком службы элемента.</span><span class="sxs-lookup"><span data-stu-id="ce04b-114">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="ce04b-115">Ластсевендайс</span><span class="sxs-lookup"><span data-stu-id="ce04b-115">lastSevenDays</span></span> | <span data-ttu-id="ce04b-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="ce04b-116">[itemActivityStat][]</span></span> | <span data-ttu-id="ce04b-117">Аналитика за последние семь дней.</span><span class="sxs-lookup"><span data-stu-id="ce04b-117">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a><span data-ttu-id="ce04b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce04b-120">JSON representation</span></span>

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
