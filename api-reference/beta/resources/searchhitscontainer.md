---
title: Тип ресурса Сеарчхитсконтаинер
description: Представляет список результатов поиска.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a2d120722179cb0fd771a84f867948a7fbfffdd4
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192788"
---
# <a name="searchhitscontainer-resource-type"></a><span data-ttu-id="ec636-103">Тип ресурса Сеарчхитсконтаинер</span><span class="sxs-lookup"><span data-stu-id="ec636-103">searchHitsContainer resource type</span></span>

<span data-ttu-id="ec636-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec636-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec636-105">Представляет список результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="ec636-105">Represent the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="ec636-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec636-106">Properties</span></span>

| <span data-ttu-id="ec636-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec636-107">Property</span></span>     | <span data-ttu-id="ec636-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ec636-108">Type</span></span>        | <span data-ttu-id="ec636-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ec636-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ec636-110">успешных</span><span class="sxs-lookup"><span data-stu-id="ec636-110">hits</span></span>|<span data-ttu-id="ec636-111">Коллекция [сеарчхит](searchhit.md)</span><span class="sxs-lookup"><span data-stu-id="ec636-111">[searchHit](searchhit.md) collection</span></span>|<span data-ttu-id="ec636-112">Коллекция результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="ec636-112">A collection of the search results.</span></span>|
|<span data-ttu-id="ec636-113">морересултсаваилабле</span><span class="sxs-lookup"><span data-stu-id="ec636-113">moreResultsAvailable</span></span>|<span data-ttu-id="ec636-114">Логическое</span><span class="sxs-lookup"><span data-stu-id="ec636-114">Boolean</span></span>|<span data-ttu-id="ec636-115">Предоставляет сведения, если доступны дополнительные результаты.</span><span class="sxs-lookup"><span data-stu-id="ec636-115">Provides information if more results are available.</span></span> <span data-ttu-id="ec636-116">На основе этих сведений вы можете соответствующим образом настроить свойства **from** и **size** для [сеарчрекуест](searchrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="ec636-116">Based on this information, you can adjust the **from** and **size** properties of the [searchRequest](searchrequest.md) accordingly.</span></span>|
|<span data-ttu-id="ec636-117">total</span><span class="sxs-lookup"><span data-stu-id="ec636-117">total</span></span>|<span data-ttu-id="ec636-118">Int32</span><span class="sxs-lookup"><span data-stu-id="ec636-118">Int32</span></span>|<span data-ttu-id="ec636-119">Общее число результатов.</span><span class="sxs-lookup"><span data-stu-id="ec636-119">The total number of results.</span></span> <span data-ttu-id="ec636-120">Note — это не количество результатов на странице, но общее количество результатов, удовлетворяющих запросу.</span><span class="sxs-lookup"><span data-stu-id="ec636-120">Note this is not the number of results on the page, but the total number of results satisfying the query.</span></span>|
|<span data-ttu-id="ec636-121">Aggregations</span><span class="sxs-lookup"><span data-stu-id="ec636-121">aggregations</span></span>|<span data-ttu-id="ec636-122">Коллекция [сеарчаггрегатион](searchaggregation.md)</span><span class="sxs-lookup"><span data-stu-id="ec636-122">[searchAggregation](searchaggregation.md) collection</span></span>|<span data-ttu-id="ec636-123">Содержит коллекцию агрегатов, вычисляемых на основе предоставленного [аггрегатионоптион](aggregationoption.md) , указанного в запросе.</span><span class="sxs-lookup"><span data-stu-id="ec636-123">Contains the collection of aggregations computed based on the provided [aggregationOption](aggregationoption.md) specified in the request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec636-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ec636-124">JSON representation</span></span>

<span data-ttu-id="ec636-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec636-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHitsContainer",
  "baseType": null
}-->


```json
{
  "hits": [{"@odata.type": "microsoft.graph.searchHit"}],
  "moreResultsAvailable": true,
  "total": 1024,
  "aggregations": [{"@odata.type": "microsoft.graph.searchAggregation"}]
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHitsContainer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


