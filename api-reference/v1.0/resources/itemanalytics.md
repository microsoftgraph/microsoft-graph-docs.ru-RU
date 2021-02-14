---
author: daspek
title: Тип ресурса itemAnalytics
description: Объект ItemAnalytics предоставляет аналитические данные о действиях, которые произошли с элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 96ad65ef5cc8907663a9ca67e5ea2b7546b8fa03
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238661"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="53478-103">Тип ресурса itemAnalytics</span><span class="sxs-lookup"><span data-stu-id="53478-103">itemAnalytics resource type</span></span>

<span data-ttu-id="53478-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53478-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="53478-105">Ресурс **itemAnalytics** предоставляет аналитические данные о действиях, которые произошли с элементом.</span><span class="sxs-lookup"><span data-stu-id="53478-105">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="53478-106">В настоящее время этот ресурс доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="53478-106">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="53478-107">Вы также можете использовать API [getActivitiesByInterval][] для получения аналитики за настраиваемый диапазон времени или интервал.</span><span class="sxs-lookup"><span data-stu-id="53478-107">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="53478-108">**Примечание.** Ресурс **itemAnalytics** пока не доступен во всех [национальных развертываниях.](/graph/deployments)</span><span class="sxs-lookup"><span data-stu-id="53478-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="properties"></a><span data-ttu-id="53478-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="53478-109">Properties</span></span>

| <span data-ttu-id="53478-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="53478-110">Property</span></span>      | <span data-ttu-id="53478-111">Тип</span><span class="sxs-lookup"><span data-stu-id="53478-111">Type</span></span>                 | <span data-ttu-id="53478-112">Описание</span><span class="sxs-lookup"><span data-stu-id="53478-112">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="53478-113">allTime</span><span class="sxs-lookup"><span data-stu-id="53478-113">allTime</span></span>       | <span data-ttu-id="53478-114">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="53478-114">[itemActivityStat][]</span></span> | <span data-ttu-id="53478-115">Аналитика на протяжении жизненного срока элемента.</span><span class="sxs-lookup"><span data-stu-id="53478-115">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="53478-116">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="53478-116">lastSevenDays</span></span> | <span data-ttu-id="53478-117">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="53478-117">[itemActivityStat][]</span></span> | <span data-ttu-id="53478-118">Аналитика за последние семь дней.</span><span class="sxs-lookup"><span data-stu-id="53478-118">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a><span data-ttu-id="53478-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53478-121">JSON representation</span></span>

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

