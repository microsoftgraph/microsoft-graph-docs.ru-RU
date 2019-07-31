---
author: daspek
description: Ресурс Итеманалитикс предоставляет аналитику о действиях, которые были выполнены для элемента. Этот ресурс в настоящее время доступен только в SharePoint и OneDrive для бизнеса.
ms.date: 09/14/2017
title: Итеманалитикс
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d2be5c7665961248e989101a1a9bd21eb805e6e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967107"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="8e95a-104">Тип ресурса Итеманалитикс</span><span class="sxs-lookup"><span data-stu-id="8e95a-104">itemAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e95a-105">Ресурс **итеманалитикс** предоставляет аналитику о действиях, которые были выполнены для элемента.</span><span class="sxs-lookup"><span data-stu-id="8e95a-105">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="8e95a-106">Этот ресурс в настоящее время доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="8e95a-106">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="8e95a-107">Вы также можете использовать API [getActivitiesByInterval][] для получения аналитики через настраиваемый диапазон или интервал времени.</span><span class="sxs-lookup"><span data-stu-id="8e95a-107">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="8e95a-108">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="8e95a-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e95a-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e95a-109">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8e95a-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e95a-110">Properties</span></span>

| <span data-ttu-id="8e95a-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e95a-111">Property</span></span>      | <span data-ttu-id="8e95a-112">Тип</span><span class="sxs-lookup"><span data-stu-id="8e95a-112">Type</span></span>                 | <span data-ttu-id="8e95a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8e95a-113">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="8e95a-114">Аллтиме</span><span class="sxs-lookup"><span data-stu-id="8e95a-114">allTime</span></span>       | <span data-ttu-id="8e95a-115">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="8e95a-115">[itemActivityStat][]</span></span> | <span data-ttu-id="8e95a-116">Аналитика за сроком службы элемента.</span><span class="sxs-lookup"><span data-stu-id="8e95a-116">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="8e95a-117">Ластсевендайс</span><span class="sxs-lookup"><span data-stu-id="8e95a-117">lastSevenDays</span></span> | <span data-ttu-id="8e95a-118">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="8e95a-118">[itemActivityStat][]</span></span> | <span data-ttu-id="8e95a-119">Аналитика за последние семь дней.</span><span class="sxs-lookup"><span data-stu-id="8e95a-119">Analytics for the last seven days.</span></span>

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
