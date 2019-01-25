---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
ms.openlocfilehash: 72e7f4de752ec04fbc5ebd98655254e2597fa499
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514966"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="b4458-102">Тип ресурса itemAnalytics</span><span class="sxs-lookup"><span data-stu-id="b4458-102">itemAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4458-103">Ресурс **itemAnalytics** предоставляет analytics о действиях, выполняемых над элементом.</span><span class="sxs-lookup"><span data-stu-id="b4458-103">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="b4458-104">Этот ресурс в данный момент доступна только на сервере SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b4458-104">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="b4458-105">Можно также использовать [getActivitiesByInterval][] API для извлечения analytics через интервала времени или интервал.</span><span class="sxs-lookup"><span data-stu-id="b4458-105">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="b4458-106">**Примечание:** **ItemAnalytics** ресурсов, пока недоступна во всех [Национальный развертываний](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="b4458-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4458-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b4458-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b4458-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b4458-108">Properties</span></span>

| <span data-ttu-id="b4458-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4458-109">Property</span></span>      | <span data-ttu-id="b4458-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b4458-110">Type</span></span>                 | <span data-ttu-id="b4458-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b4458-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="b4458-112">allTime</span><span class="sxs-lookup"><span data-stu-id="b4458-112">allTime</span></span>       | <span data-ttu-id="b4458-113">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="b4458-113">[itemActivityStat][]</span></span> | <span data-ttu-id="b4458-114">Аналитика по зависящая от элемента.</span><span class="sxs-lookup"><span data-stu-id="b4458-114">Analytics over the the item's lifespan.</span></span>
| <span data-ttu-id="b4458-115">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="b4458-115">lastSevenDays</span></span> | <span data-ttu-id="b4458-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="b4458-116">[itemActivityStat][]</span></span> | <span data-ttu-id="b4458-117">Анализ для за последние семь дней.</span><span class="sxs-lookup"><span data-stu-id="b4458-117">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

<!--
{
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemanalytics.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
