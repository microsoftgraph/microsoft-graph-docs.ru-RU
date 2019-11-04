---
title: Тип ресурса Сеарчхит
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 2ce5671933589f6066698df3e082390207474b49
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939868"
---
# <a name="searchhit-resource-type"></a><span data-ttu-id="d0edd-103">Тип ресурса Сеарчхит</span><span class="sxs-lookup"><span data-stu-id="d0edd-103">searchHit resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0edd-104">Представляет один результат в списке результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="d0edd-104">Represent a single result within the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="d0edd-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0edd-105">Properties</span></span>

| <span data-ttu-id="d0edd-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0edd-106">Property</span></span>     | <span data-ttu-id="d0edd-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d0edd-107">Type</span></span>        | <span data-ttu-id="d0edd-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d0edd-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d0edd-109">_id</span><span class="sxs-lookup"><span data-stu-id="d0edd-109">_id</span></span>|<span data-ttu-id="d0edd-110">Строка</span><span class="sxs-lookup"><span data-stu-id="d0edd-110">String</span></span>|<span data-ttu-id="d0edd-111">Внутренний идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="d0edd-111">The internal identifier for the item.</span></span>|
|<span data-ttu-id="d0edd-112">_score</span><span class="sxs-lookup"><span data-stu-id="d0edd-112">_score</span></span>|<span data-ttu-id="d0edd-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d0edd-113">Int32</span></span>|<span data-ttu-id="d0edd-114">Оценка или порядок результатов.</span><span class="sxs-lookup"><span data-stu-id="d0edd-114">The score or the order of the result.</span></span>|
|<span data-ttu-id="d0edd-115">_sortField</span><span class="sxs-lookup"><span data-stu-id="d0edd-115">_sortField</span></span>|<span data-ttu-id="d0edd-116">Строка</span><span class="sxs-lookup"><span data-stu-id="d0edd-116">String</span></span>|<span data-ttu-id="d0edd-117">Используемый порядок сортировки.</span><span class="sxs-lookup"><span data-stu-id="d0edd-117">The sort order used.</span></span> <span data-ttu-id="d0edd-118">Это может быть значение DateTime или релевантность.</span><span class="sxs-lookup"><span data-stu-id="d0edd-118">It can be DateTime or Relevance.</span></span>|
|<span data-ttu-id="d0edd-119">_summary</span><span class="sxs-lookup"><span data-stu-id="d0edd-119">_summary</span></span>|<span data-ttu-id="d0edd-120">Строка</span><span class="sxs-lookup"><span data-stu-id="d0edd-120">String</span></span>|<span data-ttu-id="d0edd-121">Сводка результатов (если доступна сводка).</span><span class="sxs-lookup"><span data-stu-id="d0edd-121">A summary of the result (if summary is available).</span></span>|
|<span data-ttu-id="d0edd-122">_source</span><span class="sxs-lookup"><span data-stu-id="d0edd-122">_source</span></span>|[<span data-ttu-id="d0edd-123">entity</span><span class="sxs-lookup"><span data-stu-id="d0edd-123">entity</span></span>](entity.md)|<span data-ttu-id="d0edd-124">Базовое представление результата поиска на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="d0edd-124">The underlying Graph representation of the search result.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0edd-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0edd-125">JSON representation</span></span>

<span data-ttu-id="d0edd-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0edd-126">The following is a JSON representation of the resource.</span></span>

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