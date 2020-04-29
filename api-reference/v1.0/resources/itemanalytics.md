---
author: daspek
ms.author: dspektor
title: Тип ресурса Итеманалитикс
description: Объект Итеманалитикс предоставляет аналитику о действиях, которые были выполнены над элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0b4ee2bba6cff84a99cf5a0e20dddc09ad87ee59
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447656"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="4dddb-103">Тип ресурса Итеманалитикс</span><span class="sxs-lookup"><span data-stu-id="4dddb-103">itemAnalytics resource type</span></span>

<span data-ttu-id="4dddb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dddb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4dddb-105">Ресурс **итеманалитикс** предоставляет аналитику о действиях, которые были выполнены для элемента.</span><span class="sxs-lookup"><span data-stu-id="4dddb-105">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="4dddb-106">Этот ресурс в настоящее время доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4dddb-106">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="4dddb-107">Вы также можете использовать API [getActivitiesByInterval][] для получения аналитики через настраиваемый диапазон или интервал времени.</span><span class="sxs-lookup"><span data-stu-id="4dddb-107">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="4dddb-108">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="4dddb-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="properties"></a><span data-ttu-id="4dddb-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4dddb-109">Properties</span></span>

| <span data-ttu-id="4dddb-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4dddb-110">Property</span></span>      | <span data-ttu-id="4dddb-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4dddb-111">Type</span></span>                 | <span data-ttu-id="4dddb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4dddb-112">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="4dddb-113">аллтиме</span><span class="sxs-lookup"><span data-stu-id="4dddb-113">allTime</span></span>       | <span data-ttu-id="4dddb-114">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="4dddb-114">[itemActivityStat][]</span></span> | <span data-ttu-id="4dddb-115">Аналитика за сроком службы элемента.</span><span class="sxs-lookup"><span data-stu-id="4dddb-115">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="4dddb-116">ластсевендайс</span><span class="sxs-lookup"><span data-stu-id="4dddb-116">lastSevenDays</span></span> | <span data-ttu-id="4dddb-117">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="4dddb-117">[itemActivityStat][]</span></span> | <span data-ttu-id="4dddb-118">Аналитика за последние семь дней.</span><span class="sxs-lookup"><span data-stu-id="4dddb-118">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a><span data-ttu-id="4dddb-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4dddb-121">JSON representation</span></span>

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
