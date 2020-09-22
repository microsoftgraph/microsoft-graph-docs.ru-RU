---
title: Тип ресурса Сеарчхитсконтаинер
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d314fcdd2a62be5aea05bed3b2a9e1881f95c3d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985799"
---
# <a name="searchhitscontainer-resource-type"></a><span data-ttu-id="6ad83-103">Тип ресурса Сеарчхитсконтаинер</span><span class="sxs-lookup"><span data-stu-id="6ad83-103">searchHitsContainer resource type</span></span>

<span data-ttu-id="6ad83-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ad83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ad83-105">Представляет список результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="6ad83-105">Represent the list of search results.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="6ad83-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ad83-106">Properties</span></span>

| <span data-ttu-id="6ad83-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ad83-107">Property</span></span>     | <span data-ttu-id="6ad83-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6ad83-108">Type</span></span>        | <span data-ttu-id="6ad83-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6ad83-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6ad83-110">успешных</span><span class="sxs-lookup"><span data-stu-id="6ad83-110">hits</span></span>|<span data-ttu-id="6ad83-111">Коллекция [сеарчхит](searchhit.md)</span><span class="sxs-lookup"><span data-stu-id="6ad83-111">[searchHit](searchhit.md) collection</span></span>|<span data-ttu-id="6ad83-112">Енкасулате результаты поиска.</span><span class="sxs-lookup"><span data-stu-id="6ad83-112">Encasulate the Search results.</span></span>|
|<span data-ttu-id="6ad83-113">морересултсаваилабле</span><span class="sxs-lookup"><span data-stu-id="6ad83-113">moreResultsAvailable</span></span>|<span data-ttu-id="6ad83-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ad83-114">Boolean</span></span>|<span data-ttu-id="6ad83-115">Предоставляет сведения, если доступны дополнительные результаты.</span><span class="sxs-lookup"><span data-stu-id="6ad83-115">Provides information if more results are available.</span></span> <span data-ttu-id="6ad83-116">В этом случае можно увеличить смещение "от" и "до".</span><span class="sxs-lookup"><span data-stu-id="6ad83-116">In that case you can increase the "from" and "to" offset.</span></span>|
|<span data-ttu-id="6ad83-117">total</span><span class="sxs-lookup"><span data-stu-id="6ad83-117">total</span></span>|<span data-ttu-id="6ad83-118">Int32</span><span class="sxs-lookup"><span data-stu-id="6ad83-118">Int32</span></span>|<span data-ttu-id="6ad83-119">Общее число результатов.</span><span class="sxs-lookup"><span data-stu-id="6ad83-119">The total number of results.</span></span> <span data-ttu-id="6ad83-120">Обратите внимание, что это не количество результатов на странице, а общее количество результатов, удовлетворяющих запросу.</span><span class="sxs-lookup"><span data-stu-id="6ad83-120">Note this is not the number on results in the page, but the total number of results satisfying the query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6ad83-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ad83-121">JSON representation</span></span>

<span data-ttu-id="6ad83-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ad83-122">The following is a JSON representation of the resource.</span></span>

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

