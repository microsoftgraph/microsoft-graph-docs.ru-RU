---
title: Тип ресурса Сеарчреспонсе
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 011b027cfcf357dfe80b47067618219cb0067044
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520894"
---
# <a name="searchresponse-resource-type"></a><span data-ttu-id="aa4f3-103">Тип ресурса Сеарчреспонсе</span><span class="sxs-lookup"><span data-stu-id="aa4f3-103">searchResponse resource type</span></span>

<span data-ttu-id="aa4f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa4f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa4f3-105">Сеарчреспонсе содержит результаты из поискового запроса.</span><span class="sxs-lookup"><span data-stu-id="aa4f3-105">The searchResponse contains the results from the search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="aa4f3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa4f3-106">Properties</span></span>

| <span data-ttu-id="aa4f3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa4f3-107">Property</span></span>     | <span data-ttu-id="aa4f3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="aa4f3-108">Type</span></span>        | <span data-ttu-id="aa4f3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aa4f3-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aa4f3-110">хитсконтаинерс</span><span class="sxs-lookup"><span data-stu-id="aa4f3-110">hitsContainers</span></span>|<span data-ttu-id="aa4f3-111">Коллекция [сеарчхитсконтаинер](searchhitscontainer.md)</span><span class="sxs-lookup"><span data-stu-id="aa4f3-111">[searchHitsContainer](searchhitscontainer.md) collection</span></span>|<span data-ttu-id="aa4f3-112">Коллекция результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="aa4f3-112">A collection of search results.</span></span>|
|<span data-ttu-id="aa4f3-113">searchTerms</span><span class="sxs-lookup"><span data-stu-id="aa4f3-113">searchTerms</span></span>|<span data-ttu-id="aa4f3-114">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="aa4f3-114">String collection</span></span>|<span data-ttu-id="aa4f3-115">Содержит условия поиска, отправленные в исходном поисковом запросе.</span><span class="sxs-lookup"><span data-stu-id="aa4f3-115">Contains the search terms sent in the initial search query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa4f3-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa4f3-116">JSON representation</span></span>

<span data-ttu-id="aa4f3-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa4f3-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResponse",
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
  "description": "searchResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->