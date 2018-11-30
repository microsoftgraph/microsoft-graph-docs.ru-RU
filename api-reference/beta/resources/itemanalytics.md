---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
ms.openlocfilehash: b50df7d1fdf67cffd508c3b5891d07c599521c8a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077155"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="36317-102">Тип ресурса itemAnalytics</span><span class="sxs-lookup"><span data-stu-id="36317-102">itemAnalytics resource type</span></span>

> <span data-ttu-id="36317-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="36317-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36317-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36317-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="36317-105">Ресурс **itemAnalytics** предоставляет analytics о действиях, выполняемых над элементом.</span><span class="sxs-lookup"><span data-stu-id="36317-105">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="36317-106">Этот ресурс в данный момент доступна только на сервере SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="36317-106">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="36317-107">Можно также использовать [getActivitiesByInterval][] API для извлечения analytics через интервала времени или интервал.</span><span class="sxs-lookup"><span data-stu-id="36317-107">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="36317-108">**Примечание:** **ItemAnalytics** ресурсов, пока недоступна во всех [Национальный развертываний](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="36317-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="36317-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36317-109">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="36317-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="36317-110">Properties</span></span>

| <span data-ttu-id="36317-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="36317-111">Property</span></span>      | <span data-ttu-id="36317-112">Тип</span><span class="sxs-lookup"><span data-stu-id="36317-112">Type</span></span>                 | <span data-ttu-id="36317-113">Description</span><span class="sxs-lookup"><span data-stu-id="36317-113">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="36317-114">allTime</span><span class="sxs-lookup"><span data-stu-id="36317-114">allTime</span></span>       | <span data-ttu-id="36317-115">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="36317-115">[itemActivityStat][]</span></span> | <span data-ttu-id="36317-116">Аналитика по зависящая от элемента.</span><span class="sxs-lookup"><span data-stu-id="36317-116">Analytics over the the item's lifespan.</span></span>
| <span data-ttu-id="36317-117">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="36317-117">lastSevenDays</span></span> | <span data-ttu-id="36317-118">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="36317-118">[itemActivityStat][]</span></span> | <span data-ttu-id="36317-119">Анализ для за последние семь дней.</span><span class="sxs-lookup"><span data-stu-id="36317-119">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

<!-- {
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics"
} -->
