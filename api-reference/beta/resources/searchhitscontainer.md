---
title: Тип ресурса Сеарчхитсконтаинер
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0bb960156a6c8f3a407dbd0691cdbed32e03693d
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703914"
---
# <a name="searchhitscontainer-resource-type"></a><span data-ttu-id="09f3f-103">Тип ресурса Сеарчхитсконтаинер</span><span class="sxs-lookup"><span data-stu-id="09f3f-103">searchHitsContainer resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09f3f-104">Представляет список результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="09f3f-104">Represent the list of search results.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="09f3f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="09f3f-105">Properties</span></span>

| <span data-ttu-id="09f3f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="09f3f-106">Property</span></span>     | <span data-ttu-id="09f3f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="09f3f-107">Type</span></span>        | <span data-ttu-id="09f3f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="09f3f-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="09f3f-109">успешных</span><span class="sxs-lookup"><span data-stu-id="09f3f-109">hits</span></span>|<span data-ttu-id="09f3f-110">Коллекция [сеарчхит](searchhit.md)</span><span class="sxs-lookup"><span data-stu-id="09f3f-110">[searchHit](searchhit.md) collection</span></span>|<span data-ttu-id="09f3f-111">Енкасулате результаты поиска.</span><span class="sxs-lookup"><span data-stu-id="09f3f-111">Encasulate the Search results.</span></span>|
|<span data-ttu-id="09f3f-112">морересултсаваилабле</span><span class="sxs-lookup"><span data-stu-id="09f3f-112">moreResultsAvailable</span></span>|<span data-ttu-id="09f3f-113">Логическое</span><span class="sxs-lookup"><span data-stu-id="09f3f-113">Boolean</span></span>|<span data-ttu-id="09f3f-114">Предоставляет сведения, если доступны дополнительные результаты.</span><span class="sxs-lookup"><span data-stu-id="09f3f-114">Provides information if more results are available.</span></span> <span data-ttu-id="09f3f-115">В этом случае можно увеличить смещение "от" и "до".</span><span class="sxs-lookup"><span data-stu-id="09f3f-115">In that case you can increase the "from" and "to" offset.</span></span>|
|<span data-ttu-id="09f3f-116">total</span><span class="sxs-lookup"><span data-stu-id="09f3f-116">total</span></span>|<span data-ttu-id="09f3f-117">Int32</span><span class="sxs-lookup"><span data-stu-id="09f3f-117">Int32</span></span>|<span data-ttu-id="09f3f-118">Общее число результатов.</span><span class="sxs-lookup"><span data-stu-id="09f3f-118">The total number of results.</span></span> <span data-ttu-id="09f3f-119">Обратите внимание, что это не количество результатов на странице, а общее количество результатов, удовлетворяющих запросу.</span><span class="sxs-lookup"><span data-stu-id="09f3f-119">Note this is not the number on results in the page, but the total number of results satisfying the query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09f3f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09f3f-120">JSON representation</span></span>

<span data-ttu-id="09f3f-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09f3f-121">The following is a JSON representation of the resource.</span></span>

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