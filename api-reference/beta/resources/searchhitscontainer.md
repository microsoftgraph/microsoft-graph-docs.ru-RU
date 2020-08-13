---
title: Тип ресурса Сеарчхитсконтаинер
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 750bd79dad9758f3ffe883fd87713c42c29c0917
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520923"
---
# <a name="searchhitscontainer-resource-type"></a><span data-ttu-id="e9f1b-103">Тип ресурса Сеарчхитсконтаинер</span><span class="sxs-lookup"><span data-stu-id="e9f1b-103">searchHitsContainer resource type</span></span>

<span data-ttu-id="e9f1b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9f1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9f1b-105">Представляет список результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="e9f1b-105">Represent the list of search results.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="e9f1b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9f1b-106">Properties</span></span>

| <span data-ttu-id="e9f1b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9f1b-107">Property</span></span>     | <span data-ttu-id="e9f1b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e9f1b-108">Type</span></span>        | <span data-ttu-id="e9f1b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e9f1b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e9f1b-110">успешных</span><span class="sxs-lookup"><span data-stu-id="e9f1b-110">hits</span></span>|<span data-ttu-id="e9f1b-111">Коллекция [сеарчхит](searchhit.md)</span><span class="sxs-lookup"><span data-stu-id="e9f1b-111">[searchHit](searchhit.md) collection</span></span>|<span data-ttu-id="e9f1b-112">Енкасулате результаты поиска.</span><span class="sxs-lookup"><span data-stu-id="e9f1b-112">Encasulate the Search results.</span></span>|
|<span data-ttu-id="e9f1b-113">морересултсаваилабле</span><span class="sxs-lookup"><span data-stu-id="e9f1b-113">moreResultsAvailable</span></span>|<span data-ttu-id="e9f1b-114">Логическое</span><span class="sxs-lookup"><span data-stu-id="e9f1b-114">Boolean</span></span>|<span data-ttu-id="e9f1b-115">Предоставляет сведения, если доступны дополнительные результаты.</span><span class="sxs-lookup"><span data-stu-id="e9f1b-115">Provides information if more results are available.</span></span> <span data-ttu-id="e9f1b-116">В этом случае можно увеличить смещение "от" и "до".</span><span class="sxs-lookup"><span data-stu-id="e9f1b-116">In that case you can increase the "from" and "to" offset.</span></span>|
|<span data-ttu-id="e9f1b-117">total</span><span class="sxs-lookup"><span data-stu-id="e9f1b-117">total</span></span>|<span data-ttu-id="e9f1b-118">Int32</span><span class="sxs-lookup"><span data-stu-id="e9f1b-118">Int32</span></span>|<span data-ttu-id="e9f1b-119">Общее число результатов.</span><span class="sxs-lookup"><span data-stu-id="e9f1b-119">The total number of results.</span></span> <span data-ttu-id="e9f1b-120">Обратите внимание, что это не количество результатов на странице, а общее количество результатов, удовлетворяющих запросу.</span><span class="sxs-lookup"><span data-stu-id="e9f1b-120">Note this is not the number on results in the page, but the total number of results satisfying the query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9f1b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9f1b-121">JSON representation</span></span>

<span data-ttu-id="e9f1b-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9f1b-122">The following is a JSON representation of the resource.</span></span>

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