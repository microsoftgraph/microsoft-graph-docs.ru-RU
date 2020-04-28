---
title: Тип ресурса Сеарчхит
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 722641b42a403565afcf7baa9de42af2b36a9dec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520930"
---
# <a name="searchhit-resource-type"></a><span data-ttu-id="ba93c-103">Тип ресурса Сеарчхит</span><span class="sxs-lookup"><span data-stu-id="ba93c-103">searchHit resource type</span></span>

<span data-ttu-id="ba93c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba93c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba93c-105">Представляет один результат в списке результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="ba93c-105">Represent a single result within the list of search results.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="ba93c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba93c-106">Properties</span></span>

| <span data-ttu-id="ba93c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba93c-107">Property</span></span>     | <span data-ttu-id="ba93c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ba93c-108">Type</span></span>        | <span data-ttu-id="ba93c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ba93c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ba93c-110">_id</span><span class="sxs-lookup"><span data-stu-id="ba93c-110">_id</span></span>|<span data-ttu-id="ba93c-111">String</span><span class="sxs-lookup"><span data-stu-id="ba93c-111">String</span></span>|<span data-ttu-id="ba93c-112">Внутренний идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="ba93c-112">The internal identifier for the item.</span></span>|
|<span data-ttu-id="ba93c-113">_score</span><span class="sxs-lookup"><span data-stu-id="ba93c-113">_score</span></span>|<span data-ttu-id="ba93c-114">Int32</span><span class="sxs-lookup"><span data-stu-id="ba93c-114">Int32</span></span>|<span data-ttu-id="ba93c-115">Оценка или порядок результатов.</span><span class="sxs-lookup"><span data-stu-id="ba93c-115">The score or the order of the result.</span></span>|
|<span data-ttu-id="ba93c-116">_sortField</span><span class="sxs-lookup"><span data-stu-id="ba93c-116">_sortField</span></span>|<span data-ttu-id="ba93c-117">String</span><span class="sxs-lookup"><span data-stu-id="ba93c-117">String</span></span>|<span data-ttu-id="ba93c-118">Используемый порядок сортировки.</span><span class="sxs-lookup"><span data-stu-id="ba93c-118">The sort order used.</span></span> <span data-ttu-id="ba93c-119">Это может быть значение DateTime или релевантность.</span><span class="sxs-lookup"><span data-stu-id="ba93c-119">It can be DateTime or Relevance.</span></span>|
|<span data-ttu-id="ba93c-120">_summary</span><span class="sxs-lookup"><span data-stu-id="ba93c-120">_summary</span></span>|<span data-ttu-id="ba93c-121">String</span><span class="sxs-lookup"><span data-stu-id="ba93c-121">String</span></span>|<span data-ttu-id="ba93c-122">Сводка результатов (если доступна сводка).</span><span class="sxs-lookup"><span data-stu-id="ba93c-122">A summary of the result (if summary is available).</span></span>|
|<span data-ttu-id="ba93c-123">_source</span><span class="sxs-lookup"><span data-stu-id="ba93c-123">_source</span></span>|[<span data-ttu-id="ba93c-124">entity</span><span class="sxs-lookup"><span data-stu-id="ba93c-124">entity</span></span>](entity.md)|<span data-ttu-id="ba93c-125">Базовое представление результата поиска на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="ba93c-125">The underlying Graph representation of the search result.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba93c-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba93c-126">JSON representation</span></span>

<span data-ttu-id="ba93c-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba93c-127">The following is a JSON representation of the resource.</span></span>

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