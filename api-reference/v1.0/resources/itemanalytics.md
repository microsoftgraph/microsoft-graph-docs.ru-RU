---
author: daspek
ms.author: dspektor
title: Тип ресурса Итеманалитикс
description: Объект Итеманалитикс предоставляет аналитику о действиях, которые были выполнены над элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 9c33a79d2728b578eeab1348a655e2b7a7574955
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036584"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="20c4c-103">Тип ресурса Итеманалитикс</span><span class="sxs-lookup"><span data-stu-id="20c4c-103">itemAnalytics resource type</span></span>

<span data-ttu-id="20c4c-104">Ресурс **итеманалитикс** предоставляет аналитику о действиях, которые были выполнены для элемента.</span><span class="sxs-lookup"><span data-stu-id="20c4c-104">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="20c4c-105">Этот ресурс в настоящее время доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="20c4c-105">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="20c4c-106">Вы также можете использовать API [getActivitiesByInterval][] для получения аналитики через настраиваемый диапазон или интервал времени.</span><span class="sxs-lookup"><span data-stu-id="20c4c-106">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="20c4c-107">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="20c4c-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="properties"></a><span data-ttu-id="20c4c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="20c4c-108">Properties</span></span>

| <span data-ttu-id="20c4c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="20c4c-109">Property</span></span>      | <span data-ttu-id="20c4c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="20c4c-110">Type</span></span>                 | <span data-ttu-id="20c4c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="20c4c-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="20c4c-112">Аллтиме</span><span class="sxs-lookup"><span data-stu-id="20c4c-112">allTime</span></span>       | <span data-ttu-id="20c4c-113">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="20c4c-113">[itemActivityStat][]</span></span> | <span data-ttu-id="20c4c-114">Аналитика за сроком службы элемента.</span><span class="sxs-lookup"><span data-stu-id="20c4c-114">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="20c4c-115">Ластсевендайс</span><span class="sxs-lookup"><span data-stu-id="20c4c-115">lastSevenDays</span></span> | <span data-ttu-id="20c4c-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="20c4c-116">[itemActivityStat][]</span></span> | <span data-ttu-id="20c4c-117">Аналитика за последние семь дней.</span><span class="sxs-lookup"><span data-stu-id="20c4c-117">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a><span data-ttu-id="20c4c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20c4c-120">JSON representation</span></span>

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
