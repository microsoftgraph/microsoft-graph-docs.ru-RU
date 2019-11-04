---
title: Тип ресурса Сеарчхитсконтаинер
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7bc36dc49a944de4a12decbf3b0b77a3c203eb21
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938718"
---
# <a name="searchhitscontainer-resource-type"></a><span data-ttu-id="162b2-103">Тип ресурса Сеарчхитсконтаинер</span><span class="sxs-lookup"><span data-stu-id="162b2-103">searchHitsContainer resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="162b2-104">Представляет список результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="162b2-104">Represent the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="162b2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="162b2-105">Properties</span></span>

| <span data-ttu-id="162b2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="162b2-106">Property</span></span>     | <span data-ttu-id="162b2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="162b2-107">Type</span></span>        | <span data-ttu-id="162b2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="162b2-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="162b2-109">успешных</span><span class="sxs-lookup"><span data-stu-id="162b2-109">hits</span></span>|<span data-ttu-id="162b2-110">Коллекция [сеарчхит](searchhit.md)</span><span class="sxs-lookup"><span data-stu-id="162b2-110">[searchHit](searchhit.md) collection</span></span>|<span data-ttu-id="162b2-111">Енкасулате результаты поиска.</span><span class="sxs-lookup"><span data-stu-id="162b2-111">Encasulate the Search results.</span></span>|
|<span data-ttu-id="162b2-112">морересултсаваилабле</span><span class="sxs-lookup"><span data-stu-id="162b2-112">moreResultsAvailable</span></span>|<span data-ttu-id="162b2-113">Логический</span><span class="sxs-lookup"><span data-stu-id="162b2-113">Boolean</span></span>|<span data-ttu-id="162b2-114">Предоставляет сведения, если доступны дополнительные результаты.</span><span class="sxs-lookup"><span data-stu-id="162b2-114">Provides information if more results are available.</span></span> <span data-ttu-id="162b2-115">В этом случае можно увеличить смещение "от" и "до".</span><span class="sxs-lookup"><span data-stu-id="162b2-115">In that case you can increase the "from" and "to" offset.</span></span>|
|<span data-ttu-id="162b2-116">total</span><span class="sxs-lookup"><span data-stu-id="162b2-116">total</span></span>|<span data-ttu-id="162b2-117">Int32</span><span class="sxs-lookup"><span data-stu-id="162b2-117">Int32</span></span>|<span data-ttu-id="162b2-118">Общее число результатов.</span><span class="sxs-lookup"><span data-stu-id="162b2-118">The total number of results.</span></span> <span data-ttu-id="162b2-119">Обратите внимание, что это не количество результатов на странице, а общее количество результатов, удовлетворяющих запросу.</span><span class="sxs-lookup"><span data-stu-id="162b2-119">Note this is not the number on results in the page, but the total number of results satisfying the query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="162b2-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="162b2-120">JSON representation</span></span>

<span data-ttu-id="162b2-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="162b2-121">The following is a JSON representation of the resource.</span></span>

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