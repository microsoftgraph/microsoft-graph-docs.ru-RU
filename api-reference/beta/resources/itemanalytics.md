---
author: daspek
description: Ресурс Итеманалитикс предоставляет аналитику о действиях, которые были выполнены для элемента. Этот ресурс в настоящее время доступен только в SharePoint и OneDrive для бизнеса.
ms.date: 09/14/2017
title: итеманалитикс
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4035ff821927d520ed457c3040be01bd9368240c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523102"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="d7328-104">Тип ресурса Итеманалитикс</span><span class="sxs-lookup"><span data-stu-id="d7328-104">itemAnalytics resource type</span></span>

<span data-ttu-id="d7328-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7328-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7328-106">Ресурс **итеманалитикс** предоставляет аналитику о действиях, которые были выполнены для элемента.</span><span class="sxs-lookup"><span data-stu-id="d7328-106">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="d7328-107">Этот ресурс в настоящее время доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="d7328-107">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="d7328-108">Вы также можете использовать API [getActivitiesByInterval][] для получения аналитики через настраиваемый диапазон или интервал времени.</span><span class="sxs-lookup"><span data-stu-id="d7328-108">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="d7328-109">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="d7328-109">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7328-110">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7328-110">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d7328-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7328-111">Properties</span></span>

| <span data-ttu-id="d7328-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7328-112">Property</span></span>      | <span data-ttu-id="d7328-113">Тип</span><span class="sxs-lookup"><span data-stu-id="d7328-113">Type</span></span>                 | <span data-ttu-id="d7328-114">Описание</span><span class="sxs-lookup"><span data-stu-id="d7328-114">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="d7328-115">аллтиме</span><span class="sxs-lookup"><span data-stu-id="d7328-115">allTime</span></span>       | <span data-ttu-id="d7328-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="d7328-116">[itemActivityStat][]</span></span> | <span data-ttu-id="d7328-117">Аналитика за сроком службы элемента.</span><span class="sxs-lookup"><span data-stu-id="d7328-117">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="d7328-118">ластсевендайс</span><span class="sxs-lookup"><span data-stu-id="d7328-118">lastSevenDays</span></span> | <span data-ttu-id="d7328-119">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="d7328-119">[itemActivityStat][]</span></span> | <span data-ttu-id="d7328-120">Аналитика за последние семь дней.</span><span class="sxs-lookup"><span data-stu-id="d7328-120">Analytics for the last seven days.</span></span>

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
