---
title: Тип ресурса Сеарчхит
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3d010f3731fa65e1ab2dc3abbf84ffdc5ebdb732
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985778"
---
# <a name="searchhit-resource-type"></a><span data-ttu-id="e47f8-103">Тип ресурса Сеарчхит</span><span class="sxs-lookup"><span data-stu-id="e47f8-103">searchHit resource type</span></span>

<span data-ttu-id="e47f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e47f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e47f8-105">Представляет один результат в списке результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="e47f8-105">Represent a single result within the list of search results.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="e47f8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e47f8-106">Properties</span></span>

| <span data-ttu-id="e47f8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e47f8-107">Property</span></span>     | <span data-ttu-id="e47f8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e47f8-108">Type</span></span>        | <span data-ttu-id="e47f8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e47f8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e47f8-110">_id</span><span class="sxs-lookup"><span data-stu-id="e47f8-110">_id</span></span>|<span data-ttu-id="e47f8-111">String</span><span class="sxs-lookup"><span data-stu-id="e47f8-111">String</span></span>|<span data-ttu-id="e47f8-112">Внутренний идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="e47f8-112">The internal identifier for the item.</span></span>|
|<span data-ttu-id="e47f8-113">_score</span><span class="sxs-lookup"><span data-stu-id="e47f8-113">_score</span></span>|<span data-ttu-id="e47f8-114">Int32</span><span class="sxs-lookup"><span data-stu-id="e47f8-114">Int32</span></span>|<span data-ttu-id="e47f8-115">Оценка или порядок результатов.</span><span class="sxs-lookup"><span data-stu-id="e47f8-115">The score or the order of the result.</span></span>|
|<span data-ttu-id="e47f8-116">_sortField</span><span class="sxs-lookup"><span data-stu-id="e47f8-116">_sortField</span></span>|<span data-ttu-id="e47f8-117">String</span><span class="sxs-lookup"><span data-stu-id="e47f8-117">String</span></span>|<span data-ttu-id="e47f8-118">Используемый порядок сортировки.</span><span class="sxs-lookup"><span data-stu-id="e47f8-118">The sort order used.</span></span> <span data-ttu-id="e47f8-119">Это может быть значение DateTime или релевантность.</span><span class="sxs-lookup"><span data-stu-id="e47f8-119">It can be DateTime or Relevance.</span></span>|
|<span data-ttu-id="e47f8-120">_summary</span><span class="sxs-lookup"><span data-stu-id="e47f8-120">_summary</span></span>|<span data-ttu-id="e47f8-121">String</span><span class="sxs-lookup"><span data-stu-id="e47f8-121">String</span></span>|<span data-ttu-id="e47f8-122">Сводка результатов (если доступна сводка).</span><span class="sxs-lookup"><span data-stu-id="e47f8-122">A summary of the result (if summary is available).</span></span>|
|<span data-ttu-id="e47f8-123">_source</span><span class="sxs-lookup"><span data-stu-id="e47f8-123">_source</span></span>|[<span data-ttu-id="e47f8-124">entity</span><span class="sxs-lookup"><span data-stu-id="e47f8-124">entity</span></span>](entity.md)|<span data-ttu-id="e47f8-125">Базовое представление результата поиска на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="e47f8-125">The underlying Graph representation of the search result.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e47f8-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e47f8-126">JSON representation</span></span>

<span data-ttu-id="e47f8-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e47f8-127">The following is a JSON representation of the resource.</span></span>

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

