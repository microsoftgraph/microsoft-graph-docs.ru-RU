---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: Итеманалитикс
localization_priority: Normal
ms.openlocfilehash: 862b0b14f1efeb3a83dd4b842c0eb995abeabb80
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620265"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="d35d3-102">Тип ресурса Итеманалитикс</span><span class="sxs-lookup"><span data-stu-id="d35d3-102">itemAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d35d3-103">Ресурс **итеманалитикс** предоставляет аналитику о действиях, которые были выполнены для элемента.</span><span class="sxs-lookup"><span data-stu-id="d35d3-103">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="d35d3-104">Этот ресурс в настоящее время доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="d35d3-104">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="d35d3-105">Вы также можете использовать API [getActivitiesByInterval][] для получения аналитики через настраиваемый диапазон или интервал времени.</span><span class="sxs-lookup"><span data-stu-id="d35d3-105">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="d35d3-106">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="d35d3-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d35d3-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d35d3-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d35d3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d35d3-108">Properties</span></span>

| <span data-ttu-id="d35d3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d35d3-109">Property</span></span>      | <span data-ttu-id="d35d3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d35d3-110">Type</span></span>                 | <span data-ttu-id="d35d3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d35d3-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="d35d3-112">Аллтиме</span><span class="sxs-lookup"><span data-stu-id="d35d3-112">allTime</span></span>       | <span data-ttu-id="d35d3-113">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="d35d3-113">[itemActivityStat][]</span></span> | <span data-ttu-id="d35d3-114">Аналитика за сроком службы элемента.</span><span class="sxs-lookup"><span data-stu-id="d35d3-114">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="d35d3-115">Ластсевендайс</span><span class="sxs-lookup"><span data-stu-id="d35d3-115">lastSevenDays</span></span> | <span data-ttu-id="d35d3-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="d35d3-116">[itemActivityStat][]</span></span> | <span data-ttu-id="d35d3-117">Аналитика за последние семь дней.</span><span class="sxs-lookup"><span data-stu-id="d35d3-117">Analytics for the last seven days.</span></span>

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
