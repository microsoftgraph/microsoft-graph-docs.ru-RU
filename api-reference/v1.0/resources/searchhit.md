---
title: Тип ресурса Сеарчхит
description: Описание объекта Сеарчхит
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: bad671657e46068263d3386eb0bb04026cfaa28e
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378017"
---
# <a name="searchhit-resource-type"></a><span data-ttu-id="c44c8-103">Тип ресурса Сеарчхит</span><span class="sxs-lookup"><span data-stu-id="c44c8-103">searchHit resource type</span></span>

<span data-ttu-id="c44c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c44c8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c44c8-105">Представляет один результат в списке результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="c44c8-105">Represents a single result within the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="c44c8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c44c8-106">Properties</span></span>

| <span data-ttu-id="c44c8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c44c8-107">Property</span></span>     | <span data-ttu-id="c44c8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c44c8-108">Type</span></span>        | <span data-ttu-id="c44c8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c44c8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c44c8-110">hitId</span><span class="sxs-lookup"><span data-stu-id="c44c8-110">hitId</span></span>|<span data-ttu-id="c44c8-111">Строка</span><span class="sxs-lookup"><span data-stu-id="c44c8-111">String</span></span>|<span data-ttu-id="c44c8-112">Внутренний идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="c44c8-112">The internal identifier for the item.</span></span>|
|<span data-ttu-id="c44c8-113">rank</span><span class="sxs-lookup"><span data-stu-id="c44c8-113">rank</span></span>|<span data-ttu-id="c44c8-114">Int32</span><span class="sxs-lookup"><span data-stu-id="c44c8-114">Int32</span></span>|<span data-ttu-id="c44c8-115">Ранг или порядок результатов.</span><span class="sxs-lookup"><span data-stu-id="c44c8-115">The rank or the order of the result.</span></span>|
|<span data-ttu-id="c44c8-116">contentSource</span><span class="sxs-lookup"><span data-stu-id="c44c8-116">contentSource</span></span>|<span data-ttu-id="c44c8-117">Строка</span><span class="sxs-lookup"><span data-stu-id="c44c8-117">String</span></span>|<span data-ttu-id="c44c8-118">Имя источника контента, частью которого является **екстерналитем** .</span><span class="sxs-lookup"><span data-stu-id="c44c8-118">The name of the content source which the **externalItem** is part of .</span></span>|
|<span data-ttu-id="c44c8-119">summary</span><span class="sxs-lookup"><span data-stu-id="c44c8-119">summary</span></span>|<span data-ttu-id="c44c8-120">Строка</span><span class="sxs-lookup"><span data-stu-id="c44c8-120">String</span></span>|<span data-ttu-id="c44c8-121">Сводка результатов, если доступна сводка.</span><span class="sxs-lookup"><span data-stu-id="c44c8-121">A summary of the result, if a summary is available.</span></span>|
|<span data-ttu-id="c44c8-122">resource</span><span class="sxs-lookup"><span data-stu-id="c44c8-122">resource</span></span>|[<span data-ttu-id="c44c8-123">entity</span><span class="sxs-lookup"><span data-stu-id="c44c8-123">entity</span></span>](entity.md)|<span data-ttu-id="c44c8-124">Базовое представление результатов поиска в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c44c8-124">The underlying Microsoft Graph representation of the search result.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c44c8-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c44c8-125">JSON representation</span></span>

<span data-ttu-id="c44c8-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c44c8-126">The following is a JSON representation of the resource.</span></span>

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
  "resource": { "@odata.type": "microsoft.graph.entity" }
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

