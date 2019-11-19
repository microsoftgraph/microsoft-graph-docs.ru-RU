---
title: Тип ресурса Сеарчхит
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 787ecfeaefc7e5b140dc6338195af7d58e1a8ccd
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703921"
---
# <a name="searchhit-resource-type"></a><span data-ttu-id="10431-103">Тип ресурса Сеарчхит</span><span class="sxs-lookup"><span data-stu-id="10431-103">searchHit resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10431-104">Представляет один результат в списке результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="10431-104">Represent a single result within the list of search results.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="10431-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="10431-105">Properties</span></span>

| <span data-ttu-id="10431-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="10431-106">Property</span></span>     | <span data-ttu-id="10431-107">Тип</span><span class="sxs-lookup"><span data-stu-id="10431-107">Type</span></span>        | <span data-ttu-id="10431-108">Описание</span><span class="sxs-lookup"><span data-stu-id="10431-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="10431-109">_id</span><span class="sxs-lookup"><span data-stu-id="10431-109">_id</span></span>|<span data-ttu-id="10431-110">String</span><span class="sxs-lookup"><span data-stu-id="10431-110">String</span></span>|<span data-ttu-id="10431-111">Внутренний идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="10431-111">The internal identifier for the item.</span></span>|
|<span data-ttu-id="10431-112">_score</span><span class="sxs-lookup"><span data-stu-id="10431-112">_score</span></span>|<span data-ttu-id="10431-113">Int32</span><span class="sxs-lookup"><span data-stu-id="10431-113">Int32</span></span>|<span data-ttu-id="10431-114">Оценка или порядок результатов.</span><span class="sxs-lookup"><span data-stu-id="10431-114">The score or the order of the result.</span></span>|
|<span data-ttu-id="10431-115">_sortField</span><span class="sxs-lookup"><span data-stu-id="10431-115">_sortField</span></span>|<span data-ttu-id="10431-116">String</span><span class="sxs-lookup"><span data-stu-id="10431-116">String</span></span>|<span data-ttu-id="10431-117">Используемый порядок сортировки.</span><span class="sxs-lookup"><span data-stu-id="10431-117">The sort order used.</span></span> <span data-ttu-id="10431-118">Это может быть значение DateTime или релевантность.</span><span class="sxs-lookup"><span data-stu-id="10431-118">It can be DateTime or Relevance.</span></span>|
|<span data-ttu-id="10431-119">_summary</span><span class="sxs-lookup"><span data-stu-id="10431-119">_summary</span></span>|<span data-ttu-id="10431-120">String</span><span class="sxs-lookup"><span data-stu-id="10431-120">String</span></span>|<span data-ttu-id="10431-121">Сводка результатов (если доступна сводка).</span><span class="sxs-lookup"><span data-stu-id="10431-121">A summary of the result (if summary is available).</span></span>|
|<span data-ttu-id="10431-122">_source</span><span class="sxs-lookup"><span data-stu-id="10431-122">_source</span></span>|[<span data-ttu-id="10431-123">entity</span><span class="sxs-lookup"><span data-stu-id="10431-123">entity</span></span>](entity.md)|<span data-ttu-id="10431-124">Базовое представление результата поиска на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="10431-124">The underlying Graph representation of the search result.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10431-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="10431-125">JSON representation</span></span>

<span data-ttu-id="10431-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10431-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHit",
  "baseType": null
}-->

```json
{
  "_id": "String",
  "_score": 1024,
  "_sortField": "String",
  "_summary": "String",
  "_source": { "@odata.type": "microsoft.graph.entity" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->