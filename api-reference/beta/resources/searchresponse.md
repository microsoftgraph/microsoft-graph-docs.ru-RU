---
title: тип ресурса searchResponse
description: Описание searchResponse
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5778d82c0c4718b9f34c686a613270eebfcc56e1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067091"
---
# <a name="searchresponse-resource-type"></a><span data-ttu-id="f0b19-103">тип ресурса searchResponse</span><span class="sxs-lookup"><span data-stu-id="f0b19-103">searchResponse resource type</span></span>

<span data-ttu-id="f0b19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0b19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0b19-105">Представляет ответ из поискового запроса.</span><span class="sxs-lookup"><span data-stu-id="f0b19-105">Represents the response from a search query.</span></span> 

## <a name="properties"></a><span data-ttu-id="f0b19-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0b19-106">Properties</span></span>

| <span data-ttu-id="f0b19-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0b19-107">Property</span></span>     | <span data-ttu-id="f0b19-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f0b19-108">Type</span></span>        | <span data-ttu-id="f0b19-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f0b19-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f0b19-110">queryAlterationResponse</span><span class="sxs-lookup"><span data-stu-id="f0b19-110">queryAlterationResponse</span></span>|[<span data-ttu-id="f0b19-111">alterationResponse</span><span class="sxs-lookup"><span data-stu-id="f0b19-111">alterationResponse</span></span>](alterationResponse.md)|<span data-ttu-id="f0b19-112">Предоставляет сведения об ответе на изменение запросов для исправления правописания.</span><span class="sxs-lookup"><span data-stu-id="f0b19-112">Provides details of query alteration response for spelling correction.</span></span>|
|<span data-ttu-id="f0b19-113">значение</span><span class="sxs-lookup"><span data-stu-id="f0b19-113">value</span></span>|<span data-ttu-id="f0b19-114">[коллекция searchResultSet](searchResultSet.md)</span><span class="sxs-lookup"><span data-stu-id="f0b19-114">[searchResultSet](searchResultSet.md) collection</span></span>|<span data-ttu-id="f0b19-115">Представляет результаты запроса поиска и термины, используемые для запроса.</span><span class="sxs-lookup"><span data-stu-id="f0b19-115">Represents results from a search query, and the terms used for the query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0b19-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f0b19-116">JSON representation</span></span>

<span data-ttu-id="f0b19-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0b19-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResponse",
  "baseType": null
}-->

```json
{
  "queryAlterationResponse": {"@odata.type": "microsoft.graph.alterationResponse"},
  "value": [{"@odata.type": "microsoft.graph.searchResultSet"}]
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

