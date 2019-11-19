---
title: Тип ресурса searchQuery
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e9501831ef2e83d23aa4a5587b9afd8eaa7f5ee8
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703907"
---
# <a name="searchquery-resource-type"></a><span data-ttu-id="72891-103">Тип ресурса searchQuery</span><span class="sxs-lookup"><span data-stu-id="72891-103">searchQuery resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72891-104">Представляет поисковый запрос, содержащий поисковые термины и необязательные фильтры.</span><span class="sxs-lookup"><span data-stu-id="72891-104">Represents a search query that contains search terms and optional filters.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="72891-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="72891-105">Properties</span></span>

| <span data-ttu-id="72891-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="72891-106">Property</span></span>     | <span data-ttu-id="72891-107">Тип</span><span class="sxs-lookup"><span data-stu-id="72891-107">Type</span></span>        | <span data-ttu-id="72891-108">Описание</span><span class="sxs-lookup"><span data-stu-id="72891-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="72891-109">query_string</span><span class="sxs-lookup"><span data-stu-id="72891-109">query_string</span></span>|[<span data-ttu-id="72891-110">сеарчкуеристринг</span><span class="sxs-lookup"><span data-stu-id="72891-110">searchQueryString</span></span>](searchquerystring.md)|<span data-ttu-id="72891-111">Поисковый запрос, содержащий условия поиска.</span><span class="sxs-lookup"><span data-stu-id="72891-111">The search query containing the search terms.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="72891-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72891-112">JSON representation</span></span>

<span data-ttu-id="72891-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72891-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQuery",
  "baseType": null
}-->

```json
{
  "query_string": {"@odata.type": "microsoft.graph.searchQueryString"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->