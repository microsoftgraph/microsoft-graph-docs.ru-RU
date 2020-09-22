---
title: Тип ресурса searchQuery
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1d2d643fed135f97f1ccf2c6346d8fdd6e22f8b5
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193367"
---
# <a name="searchquery-resource-type"></a><span data-ttu-id="dade4-103">Тип ресурса searchQuery</span><span class="sxs-lookup"><span data-stu-id="dade4-103">searchQuery resource type</span></span>

<span data-ttu-id="dade4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dade4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

<span data-ttu-id="dade4-105">Представляет поисковый запрос, содержащий поисковые термины и необязательные фильтры.</span><span class="sxs-lookup"><span data-stu-id="dade4-105">Represents a search query that contains search terms and optional filters.</span></span>

## <a name="properties"></a><span data-ttu-id="dade4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="dade4-106">Properties</span></span>

| <span data-ttu-id="dade4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="dade4-107">Property</span></span>     | <span data-ttu-id="dade4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="dade4-108">Type</span></span>        | <span data-ttu-id="dade4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dade4-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dade4-110">Строку</span><span class="sxs-lookup"><span data-stu-id="dade4-110">queryString</span></span>|<span data-ttu-id="dade4-111">String</span><span class="sxs-lookup"><span data-stu-id="dade4-111">String</span></span>|<span data-ttu-id="dade4-112">Поисковый запрос, содержащий условия поиска.</span><span class="sxs-lookup"><span data-stu-id="dade4-112">The search query containing the search terms.</span></span> <span data-ttu-id="dade4-113">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="dade4-113">Required.</span></span>|
|<span data-ttu-id="dade4-114">query_string (устаревшее)</span><span class="sxs-lookup"><span data-stu-id="dade4-114">query_string (deprecated)</span></span>|[<span data-ttu-id="dade4-115">сеарчкуеристринг</span><span class="sxs-lookup"><span data-stu-id="dade4-115">searchQueryString</span></span>](searchquerystring.md)|<span data-ttu-id="dade4-116">Теперь оно заменяется свойством **queryString** .</span><span class="sxs-lookup"><span data-stu-id="dade4-116">This is now replaced by the **queryString** property.</span></span> <span data-ttu-id="dade4-117">Поисковый запрос, содержащий условия поиска.</span><span class="sxs-lookup"><span data-stu-id="dade4-117">The search query containing the search terms.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="dade4-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dade4-118">JSON representation</span></span>

<span data-ttu-id="dade4-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dade4-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQuery",
  "baseType": null
}-->

```json
{
  "queryString": "String",
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

