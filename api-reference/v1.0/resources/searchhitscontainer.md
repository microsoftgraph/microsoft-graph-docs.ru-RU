---
title: Тип ресурса Сеарчхитсконтаинер
description: Представляет список результатов поиска.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f32fa198624c04da6eadfc828b60350164cbdddc
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378059"
---
# <a name="searchhitscontainer-resource-type"></a><span data-ttu-id="d79cd-103">Тип ресурса Сеарчхитсконтаинер</span><span class="sxs-lookup"><span data-stu-id="d79cd-103">searchHitsContainer resource type</span></span>

<span data-ttu-id="d79cd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d79cd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d79cd-105">Представляет список результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="d79cd-105">Represent the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="d79cd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d79cd-106">Properties</span></span>

| <span data-ttu-id="d79cd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d79cd-107">Property</span></span>     | <span data-ttu-id="d79cd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d79cd-108">Type</span></span>        | <span data-ttu-id="d79cd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d79cd-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d79cd-110">успешных</span><span class="sxs-lookup"><span data-stu-id="d79cd-110">hits</span></span>|<span data-ttu-id="d79cd-111">Коллекция [сеарчхит](searchhit.md)</span><span class="sxs-lookup"><span data-stu-id="d79cd-111">[searchHit](searchhit.md) collection</span></span>|<span data-ttu-id="d79cd-112">Коллекция результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="d79cd-112">A collection of the search results.</span></span>|
|<span data-ttu-id="d79cd-113">морересултсаваилабле</span><span class="sxs-lookup"><span data-stu-id="d79cd-113">moreResultsAvailable</span></span>|<span data-ttu-id="d79cd-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="d79cd-114">Boolean</span></span>|<span data-ttu-id="d79cd-115">Предоставляет сведения, если доступны дополнительные результаты.</span><span class="sxs-lookup"><span data-stu-id="d79cd-115">Provides information if more results are available.</span></span> <span data-ttu-id="d79cd-116">На основе этих сведений вы можете соответствующим образом настроить свойства **from** и **size** для [сеарчрекуест](searchrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="d79cd-116">Based on this information, you can adjust the **from** and **size** properties of the [searchRequest](searchrequest.md) accordingly.</span></span>|
|<span data-ttu-id="d79cd-117">total</span><span class="sxs-lookup"><span data-stu-id="d79cd-117">total</span></span>|<span data-ttu-id="d79cd-118">Int32</span><span class="sxs-lookup"><span data-stu-id="d79cd-118">Int32</span></span>|<span data-ttu-id="d79cd-119">Общее число результатов.</span><span class="sxs-lookup"><span data-stu-id="d79cd-119">The total number of results.</span></span> <span data-ttu-id="d79cd-120">Note — это не количество результатов на странице, но общее количество результатов, удовлетворяющих запросу.</span><span class="sxs-lookup"><span data-stu-id="d79cd-120">Note this is not the number of results on the page, but the total number of results satisfying the query.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d79cd-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d79cd-121">JSON representation</span></span>

<span data-ttu-id="d79cd-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d79cd-122">The following is a JSON representation of the resource.</span></span>

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
  "total": 1024
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


