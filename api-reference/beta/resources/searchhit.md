---
title: Тип ресурса Сеарчхит
description: Описание объекта Сеарчхит
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c140a30d4e77840b1fd7c7ccceec16e0554cd855
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193612"
---
# <a name="searchhit-resource-type"></a><span data-ttu-id="06a3a-103">Тип ресурса Сеарчхит</span><span class="sxs-lookup"><span data-stu-id="06a3a-103">searchHit resource type</span></span>

<span data-ttu-id="06a3a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06a3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

<span data-ttu-id="06a3a-105">Представляет один результат в списке результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="06a3a-105">Represents a single result within the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="06a3a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="06a3a-106">Properties</span></span>

| <span data-ttu-id="06a3a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="06a3a-107">Property</span></span>     | <span data-ttu-id="06a3a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="06a3a-108">Type</span></span>        | <span data-ttu-id="06a3a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="06a3a-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="06a3a-110">хитид</span><span class="sxs-lookup"><span data-stu-id="06a3a-110">hitId</span></span>|<span data-ttu-id="06a3a-111">String</span><span class="sxs-lookup"><span data-stu-id="06a3a-111">String</span></span>|<span data-ttu-id="06a3a-112">Внутренний идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="06a3a-112">The internal identifier for the item.</span></span>|
|<span data-ttu-id="06a3a-113">rank</span><span class="sxs-lookup"><span data-stu-id="06a3a-113">rank</span></span>|<span data-ttu-id="06a3a-114">Int32</span><span class="sxs-lookup"><span data-stu-id="06a3a-114">Int32</span></span>|<span data-ttu-id="06a3a-115">Ранг или порядок результатов.</span><span class="sxs-lookup"><span data-stu-id="06a3a-115">The rank or the order of the result.</span></span>|
|<span data-ttu-id="06a3a-116">contentSource</span><span class="sxs-lookup"><span data-stu-id="06a3a-116">contentSource</span></span>|<span data-ttu-id="06a3a-117">String</span><span class="sxs-lookup"><span data-stu-id="06a3a-117">String</span></span>|<span data-ttu-id="06a3a-118">Имя источника контента, частью которого является **екстерналитем** .</span><span class="sxs-lookup"><span data-stu-id="06a3a-118">The name of the content source which the **externalItem** is part of .</span></span>|
|<span data-ttu-id="06a3a-119">summary</span><span class="sxs-lookup"><span data-stu-id="06a3a-119">summary</span></span>|<span data-ttu-id="06a3a-120">String</span><span class="sxs-lookup"><span data-stu-id="06a3a-120">String</span></span>|<span data-ttu-id="06a3a-121">Сводка результатов, если доступна сводка.</span><span class="sxs-lookup"><span data-stu-id="06a3a-121">A summary of the result, if a summary is available.</span></span>|
|<span data-ttu-id="06a3a-122">resource</span><span class="sxs-lookup"><span data-stu-id="06a3a-122">resource</span></span>|[<span data-ttu-id="06a3a-123">entity</span><span class="sxs-lookup"><span data-stu-id="06a3a-123">entity</span></span>](entity.md)|<span data-ttu-id="06a3a-124">Базовое представление результатов поиска в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="06a3a-124">The underlying Microsoft Graph representation of the search result.</span></span>|
|<span data-ttu-id="06a3a-125">_id (устаревшее)</span><span class="sxs-lookup"><span data-stu-id="06a3a-125">_id (deprecated)</span></span>|<span data-ttu-id="06a3a-126">String</span><span class="sxs-lookup"><span data-stu-id="06a3a-126">String</span></span>| <span data-ttu-id="06a3a-127">Переименован в качестве **хитид**.</span><span class="sxs-lookup"><span data-stu-id="06a3a-127">Renamed as **hitId**.</span></span> <span data-ttu-id="06a3a-128">Внутренний идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="06a3a-128">The internal identifier for the item.</span></span>|
|<span data-ttu-id="06a3a-129">_score (устаревшее)</span><span class="sxs-lookup"><span data-stu-id="06a3a-129">_score (deprecated)</span></span>|<span data-ttu-id="06a3a-130">Int32</span><span class="sxs-lookup"><span data-stu-id="06a3a-130">Int32</span></span>|<span data-ttu-id="06a3a-131">Переименовано в качестве **ранга**.</span><span class="sxs-lookup"><span data-stu-id="06a3a-131">Renamed as **rank**.</span></span> <span data-ttu-id="06a3a-132">Оценка или порядок результатов.</span><span class="sxs-lookup"><span data-stu-id="06a3a-132">The score or the order of the result.</span></span>|
|<span data-ttu-id="06a3a-133">_summary (устаревшее)</span><span class="sxs-lookup"><span data-stu-id="06a3a-133">_summary (deprecated)</span></span>|<span data-ttu-id="06a3a-134">String</span><span class="sxs-lookup"><span data-stu-id="06a3a-134">String</span></span>|<span data-ttu-id="06a3a-135">Переименовано в качестве **сводки**.</span><span class="sxs-lookup"><span data-stu-id="06a3a-135">Renamed as **summary**.</span></span> <span data-ttu-id="06a3a-136">Сводка результатов (если доступна сводка).</span><span class="sxs-lookup"><span data-stu-id="06a3a-136">A summary of the result (if summary is available).</span></span>|
|<span data-ttu-id="06a3a-137">_sortField (устаревшее)</span><span class="sxs-lookup"><span data-stu-id="06a3a-137">_sortField (deprecated)</span></span>|<span data-ttu-id="06a3a-138">String</span><span class="sxs-lookup"><span data-stu-id="06a3a-138">String</span></span>|<span data-ttu-id="06a3a-139">Это свойство было удалено.</span><span class="sxs-lookup"><span data-stu-id="06a3a-139">This property has been removed.</span></span>|
|<span data-ttu-id="06a3a-140">_source (устаревшее)</span><span class="sxs-lookup"><span data-stu-id="06a3a-140">_source (deprecated)</span></span>|[<span data-ttu-id="06a3a-141">entity</span><span class="sxs-lookup"><span data-stu-id="06a3a-141">entity</span></span>](entity.md)|<span data-ttu-id="06a3a-142">Переименовано в качестве **ресурса**.</span><span class="sxs-lookup"><span data-stu-id="06a3a-142">Renamed as **resource**.</span></span> <span data-ttu-id="06a3a-143">Базовое представление результата поиска на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="06a3a-143">The underlying Graph representation of the search result.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06a3a-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06a3a-144">JSON representation</span></span>

<span data-ttu-id="06a3a-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06a3a-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHit",
  "baseType": null
}-->

```json
{
  "hitId": "String",
  "rank": 1,
  "summary": "String",
  "contentSource": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" },
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

