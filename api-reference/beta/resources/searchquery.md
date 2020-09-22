---
title: Тип ресурса searchQuery
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: db647c47c528428820acc2ded9b079546b991be6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985743"
---
# <a name="searchquery-resource-type"></a><span data-ttu-id="8a7fa-103">Тип ресурса searchQuery</span><span class="sxs-lookup"><span data-stu-id="8a7fa-103">searchQuery resource type</span></span>

<span data-ttu-id="8a7fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a7fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a7fa-105">Представляет поисковый запрос, содержащий поисковые термины и необязательные фильтры.</span><span class="sxs-lookup"><span data-stu-id="8a7fa-105">Represents a search query that contains search terms and optional filters.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="8a7fa-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a7fa-106">Properties</span></span>

| <span data-ttu-id="8a7fa-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a7fa-107">Property</span></span>     | <span data-ttu-id="8a7fa-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8a7fa-108">Type</span></span>        | <span data-ttu-id="8a7fa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8a7fa-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8a7fa-110">query_string</span><span class="sxs-lookup"><span data-stu-id="8a7fa-110">query_string</span></span>|[<span data-ttu-id="8a7fa-111">сеарчкуеристринг</span><span class="sxs-lookup"><span data-stu-id="8a7fa-111">searchQueryString</span></span>](searchquerystring.md)|<span data-ttu-id="8a7fa-112">Поисковый запрос, содержащий условия поиска.</span><span class="sxs-lookup"><span data-stu-id="8a7fa-112">The search query containing the search terms.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a7fa-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a7fa-113">JSON representation</span></span>

<span data-ttu-id="8a7fa-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a7fa-114">The following is a JSON representation of the resource.</span></span>

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

