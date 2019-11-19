---
title: Тип ресурса Сеарчкуеристринг
description: сеарчкуеристринг
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 59809860bd2d0954ee8323f9c8e4fe982fb4faa7
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703828"
---
# <a name="searchquerystring-resource-type"></a><span data-ttu-id="14da1-103">Тип ресурса Сеарчкуеристринг</span><span class="sxs-lookup"><span data-stu-id="14da1-103">searchQueryString resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14da1-104">Условия поиска для запроса.</span><span class="sxs-lookup"><span data-stu-id="14da1-104">The search terms for the query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="14da1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="14da1-105">Properties</span></span>

| <span data-ttu-id="14da1-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="14da1-106">Property</span></span>     | <span data-ttu-id="14da1-107">Тип</span><span class="sxs-lookup"><span data-stu-id="14da1-107">Type</span></span>        | <span data-ttu-id="14da1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="14da1-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="14da1-109">Запрос</span><span class="sxs-lookup"><span data-stu-id="14da1-109">query</span></span>|<span data-ttu-id="14da1-110">String</span><span class="sxs-lookup"><span data-stu-id="14da1-110">String</span></span>|<span data-ttu-id="14da1-111">Содержит фактические условия поиска запроса.</span><span class="sxs-lookup"><span data-stu-id="14da1-111">Contains the actual search terms of the request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14da1-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="14da1-112">JSON representation</span></span>

<span data-ttu-id="14da1-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14da1-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQueryString",
  "baseType": null
}-->

```json
{
  "query": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchQueryString resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->