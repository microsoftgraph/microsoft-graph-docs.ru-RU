---
title: Тип ресурса Сеарчкуеристринг
description: сеарчкуеристринг
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 93142dcc672c5fee18a5f98d0988352e6c02cbd0
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936072"
---
# <a name="searchquerystring-resource-type"></a><span data-ttu-id="48dd0-103">Тип ресурса Сеарчкуеристринг</span><span class="sxs-lookup"><span data-stu-id="48dd0-103">searchQueryString resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48dd0-104">Условия поиска для запроса.</span><span class="sxs-lookup"><span data-stu-id="48dd0-104">The search terms for the query.</span></span>

## <a name="properties"></a><span data-ttu-id="48dd0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="48dd0-105">Properties</span></span>

| <span data-ttu-id="48dd0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="48dd0-106">Property</span></span>     | <span data-ttu-id="48dd0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="48dd0-107">Type</span></span>        | <span data-ttu-id="48dd0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="48dd0-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="48dd0-109">Запрос</span><span class="sxs-lookup"><span data-stu-id="48dd0-109">query</span></span>|<span data-ttu-id="48dd0-110">Строка</span><span class="sxs-lookup"><span data-stu-id="48dd0-110">String</span></span>|<span data-ttu-id="48dd0-111">Содержит фактические условия поиска запроса.</span><span class="sxs-lookup"><span data-stu-id="48dd0-111">Contains the actual search terms of the request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48dd0-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="48dd0-112">JSON representation</span></span>

<span data-ttu-id="48dd0-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48dd0-113">The following is a JSON representation of the resource.</span></span>

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