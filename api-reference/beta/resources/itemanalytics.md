---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: Итеманалитикс
localization_priority: Normal
ms.openlocfilehash: 72e7f4de752ec04fbc5ebd98655254e2597fa499
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581648"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="3dd38-102">Тип ресурса Итеманалитикс</span><span class="sxs-lookup"><span data-stu-id="3dd38-102">itemAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dd38-103">Ресурс **итеманалитикс** предоставляет аналитику о действиях, которые были выполнены для элемента.</span><span class="sxs-lookup"><span data-stu-id="3dd38-103">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="3dd38-104">Этот ресурс в настоящее время доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="3dd38-104">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="3dd38-105">Вы также можете использовать API [getActivitiesByInterval][] для получения аналитики через настраиваемый диапазон или интервал времени.</span><span class="sxs-lookup"><span data-stu-id="3dd38-105">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="3dd38-106">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="3dd38-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3dd38-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3dd38-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="3dd38-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3dd38-108">Properties</span></span>

| <span data-ttu-id="3dd38-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3dd38-109">Property</span></span>      | <span data-ttu-id="3dd38-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3dd38-110">Type</span></span>                 | <span data-ttu-id="3dd38-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3dd38-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="3dd38-112">Аллтиме</span><span class="sxs-lookup"><span data-stu-id="3dd38-112">allTime</span></span>       | <span data-ttu-id="3dd38-113">[Итемактивитистат][]</span><span class="sxs-lookup"><span data-stu-id="3dd38-113">[itemActivityStat][]</span></span> | <span data-ttu-id="3dd38-114">Аналитика за сроком службы элемента.</span><span class="sxs-lookup"><span data-stu-id="3dd38-114">Analytics over the the item's lifespan.</span></span>
| <span data-ttu-id="3dd38-115">Ластсевендайс</span><span class="sxs-lookup"><span data-stu-id="3dd38-115">lastSevenDays</span></span> | <span data-ttu-id="3dd38-116">[Итемактивитистат][]</span><span class="sxs-lookup"><span data-stu-id="3dd38-116">[itemActivityStat][]</span></span> | <span data-ttu-id="3dd38-117">Аналитика за последние семь дней.</span><span class="sxs-lookup"><span data-stu-id="3dd38-117">Analytics for the last seven days.</span></span>

[Итемактивитистат]: itemactivitystat.md
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
