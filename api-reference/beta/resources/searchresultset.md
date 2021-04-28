---
title: тип ресурса searchResultSet
description: Описание searchResultSet
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5d17791a618f1d587520f23524da9ce19241d3b1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068125"
---
# <a name="searchresultset-resource-type"></a><span data-ttu-id="27507-103">тип ресурса searchResultSet</span><span class="sxs-lookup"><span data-stu-id="27507-103">searchResultSet resource type</span></span>

<span data-ttu-id="27507-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27507-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27507-105">Представляет результаты запроса поиска и термины, используемые для запроса.</span><span class="sxs-lookup"><span data-stu-id="27507-105">Represents results from a search query, and the terms used for the query.</span></span> 

## <a name="properties"></a><span data-ttu-id="27507-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="27507-106">Properties</span></span>

| <span data-ttu-id="27507-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="27507-107">Property</span></span>     | <span data-ttu-id="27507-108">Тип</span><span class="sxs-lookup"><span data-stu-id="27507-108">Type</span></span>        | <span data-ttu-id="27507-109">Описание</span><span class="sxs-lookup"><span data-stu-id="27507-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="27507-110">hitsContainers</span><span class="sxs-lookup"><span data-stu-id="27507-110">hitsContainers</span></span>|<span data-ttu-id="27507-111">[коллекция searchHitsContainer](searchhitscontainer.md)</span><span class="sxs-lookup"><span data-stu-id="27507-111">[searchHitsContainer](searchhitscontainer.md) collection</span></span>|<span data-ttu-id="27507-112">Коллекция результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="27507-112">A collection of search results.</span></span>|
|<span data-ttu-id="27507-113">searchTerms</span><span class="sxs-lookup"><span data-stu-id="27507-113">searchTerms</span></span>|<span data-ttu-id="27507-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="27507-114">String collection</span></span>|<span data-ttu-id="27507-115">Содержит термины поиска, отправленные в исходном запросе поиска.</span><span class="sxs-lookup"><span data-stu-id="27507-115">Contains the search terms sent in the initial search query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27507-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="27507-116">JSON representation</span></span>

<span data-ttu-id="27507-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27507-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResultSet",
  "baseType": null
}-->

```json
{
  "hitsContainers": [{"@odata.type": "microsoft.graph.searchHitsContainer"}],
  "searchTerms": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchResultSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

