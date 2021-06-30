---
title: тип ресурса searchHit
description: Описание объекта searchHit
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7c546483eea81e7d89a3a87ba5b8c0eb0ff48783
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210334"
---
# <a name="searchhit-resource-type"></a><span data-ttu-id="98394-103">тип ресурса searchHit</span><span class="sxs-lookup"><span data-stu-id="98394-103">searchHit resource type</span></span>

<span data-ttu-id="98394-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98394-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

<span data-ttu-id="98394-105">Представляет один результат в списке результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="98394-105">Represents a single result within the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="98394-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="98394-106">Properties</span></span>

| <span data-ttu-id="98394-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="98394-107">Property</span></span>     | <span data-ttu-id="98394-108">Тип</span><span class="sxs-lookup"><span data-stu-id="98394-108">Type</span></span>        | <span data-ttu-id="98394-109">Описание</span><span class="sxs-lookup"><span data-stu-id="98394-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="98394-110">hitId</span><span class="sxs-lookup"><span data-stu-id="98394-110">hitId</span></span>|<span data-ttu-id="98394-111">String</span><span class="sxs-lookup"><span data-stu-id="98394-111">String</span></span>|<span data-ttu-id="98394-112">Внутренний идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="98394-112">The internal identifier for the item.</span></span>|
|<span data-ttu-id="98394-113">rank</span><span class="sxs-lookup"><span data-stu-id="98394-113">rank</span></span>|<span data-ttu-id="98394-114">Int32</span><span class="sxs-lookup"><span data-stu-id="98394-114">Int32</span></span>|<span data-ttu-id="98394-115">Ранж или порядок результата.</span><span class="sxs-lookup"><span data-stu-id="98394-115">The rank or the order of the result.</span></span>|
|<span data-ttu-id="98394-116">contentSource</span><span class="sxs-lookup"><span data-stu-id="98394-116">contentSource</span></span>|<span data-ttu-id="98394-117">String</span><span class="sxs-lookup"><span data-stu-id="98394-117">String</span></span>|<span data-ttu-id="98394-118">Имя источника контента, **частью которого является externalItem.**</span><span class="sxs-lookup"><span data-stu-id="98394-118">The name of the content source which the **externalItem** is part of .</span></span>|
|<span data-ttu-id="98394-119">summary</span><span class="sxs-lookup"><span data-stu-id="98394-119">summary</span></span>|<span data-ttu-id="98394-120">String</span><span class="sxs-lookup"><span data-stu-id="98394-120">String</span></span>|<span data-ttu-id="98394-121">Сводка результатов, если резюме доступно.</span><span class="sxs-lookup"><span data-stu-id="98394-121">A summary of the result, if a summary is available.</span></span>|
|<span data-ttu-id="98394-122">resultTemplateId</span><span class="sxs-lookup"><span data-stu-id="98394-122">resultTemplateId</span></span>|<span data-ttu-id="98394-123">String</span><span class="sxs-lookup"><span data-stu-id="98394-123">String</span></span>|<span data-ttu-id="98394-124">ID шаблона результатов для отрисовки результата поиска.</span><span class="sxs-lookup"><span data-stu-id="98394-124">ID of the result template for rendering the search result.</span></span> <span data-ttu-id="98394-125">Этот ID должен отображать макет в словаре **resultTemplates,** который также включен в [searchresponse.](searchresponse.md)</span><span class="sxs-lookup"><span data-stu-id="98394-125">This ID must map to a display layout in the **resultTemplates** dictionary, included in the [searchresponse](searchresponse.md) as well.</span></span>|
|<span data-ttu-id="98394-126">resource</span><span class="sxs-lookup"><span data-stu-id="98394-126">resource</span></span>|[<span data-ttu-id="98394-127">entity</span><span class="sxs-lookup"><span data-stu-id="98394-127">entity</span></span>](entity.md)|<span data-ttu-id="98394-128">В основном microsoft Graph представление результата поиска.</span><span class="sxs-lookup"><span data-stu-id="98394-128">The underlying Microsoft Graph representation of the search result.</span></span>|
|<span data-ttu-id="98394-129">_id (неподготовленный)</span><span class="sxs-lookup"><span data-stu-id="98394-129">_id (deprecated)</span></span>|<span data-ttu-id="98394-130">String</span><span class="sxs-lookup"><span data-stu-id="98394-130">String</span></span>| <span data-ttu-id="98394-131">Переименован в **hitId**.</span><span class="sxs-lookup"><span data-stu-id="98394-131">Renamed as **hitId**.</span></span> <span data-ttu-id="98394-132">Внутренний идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="98394-132">The internal identifier for the item.</span></span>|
|<span data-ttu-id="98394-133">_score (обесценилось)</span><span class="sxs-lookup"><span data-stu-id="98394-133">_score (deprecated)</span></span>|<span data-ttu-id="98394-134">Int32</span><span class="sxs-lookup"><span data-stu-id="98394-134">Int32</span></span>|<span data-ttu-id="98394-135">Переименован в **ранж.**</span><span class="sxs-lookup"><span data-stu-id="98394-135">Renamed as **rank**.</span></span> <span data-ttu-id="98394-136">Оценка или порядок результата.</span><span class="sxs-lookup"><span data-stu-id="98394-136">The score or the order of the result.</span></span>|
|<span data-ttu-id="98394-137">_summary (обесценилось)</span><span class="sxs-lookup"><span data-stu-id="98394-137">_summary (deprecated)</span></span>|<span data-ttu-id="98394-138">String</span><span class="sxs-lookup"><span data-stu-id="98394-138">String</span></span>|<span data-ttu-id="98394-139">Переименовано в **сводку**.</span><span class="sxs-lookup"><span data-stu-id="98394-139">Renamed as **summary**.</span></span> <span data-ttu-id="98394-140">Сводка результатов (если сводка доступна).</span><span class="sxs-lookup"><span data-stu-id="98394-140">A summary of the result (if summary is available).</span></span>|
|<span data-ttu-id="98394-141">_sortField (обесценилось)</span><span class="sxs-lookup"><span data-stu-id="98394-141">_sortField (deprecated)</span></span>|<span data-ttu-id="98394-142">String</span><span class="sxs-lookup"><span data-stu-id="98394-142">String</span></span>|<span data-ttu-id="98394-143">Это свойство удалено.</span><span class="sxs-lookup"><span data-stu-id="98394-143">This property has been removed.</span></span>|
|<span data-ttu-id="98394-144">_source (обесценилось)</span><span class="sxs-lookup"><span data-stu-id="98394-144">_source (deprecated)</span></span>|[<span data-ttu-id="98394-145">entity</span><span class="sxs-lookup"><span data-stu-id="98394-145">entity</span></span>](entity.md)|<span data-ttu-id="98394-146">Переименован в **ресурс.**</span><span class="sxs-lookup"><span data-stu-id="98394-146">Renamed as **resource**.</span></span> <span data-ttu-id="98394-147">В Graph представлен результат поиска.</span><span class="sxs-lookup"><span data-stu-id="98394-147">The underlying Graph representation of the search result.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98394-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98394-148">JSON representation</span></span>

<span data-ttu-id="98394-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98394-149">The following is a JSON representation of the resource.</span></span>

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
  "resultTemplateId": "String",
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

