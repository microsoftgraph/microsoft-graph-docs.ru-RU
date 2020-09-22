---
title: Тип ресурса Сеарчреспонсе
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a2bdd013cb755d37664c89aca81a8ae89c63b4f9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973745"
---
# <a name="searchresponse-resource-type"></a><span data-ttu-id="408a0-103">Тип ресурса Сеарчреспонсе</span><span class="sxs-lookup"><span data-stu-id="408a0-103">searchResponse resource type</span></span>

<span data-ttu-id="408a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="408a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="408a0-105">Сеарчреспонсе содержит результаты из поискового запроса.</span><span class="sxs-lookup"><span data-stu-id="408a0-105">The searchResponse contains the results from the search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="408a0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="408a0-106">Properties</span></span>

| <span data-ttu-id="408a0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="408a0-107">Property</span></span>     | <span data-ttu-id="408a0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="408a0-108">Type</span></span>        | <span data-ttu-id="408a0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="408a0-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="408a0-110">хитсконтаинерс</span><span class="sxs-lookup"><span data-stu-id="408a0-110">hitsContainers</span></span>|<span data-ttu-id="408a0-111">Коллекция [сеарчхитсконтаинер](searchhitscontainer.md)</span><span class="sxs-lookup"><span data-stu-id="408a0-111">[searchHitsContainer](searchhitscontainer.md) collection</span></span>|<span data-ttu-id="408a0-112">Коллекция результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="408a0-112">A collection of search results.</span></span>|
|<span data-ttu-id="408a0-113">searchTerms</span><span class="sxs-lookup"><span data-stu-id="408a0-113">searchTerms</span></span>|<span data-ttu-id="408a0-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="408a0-114">String collection</span></span>|<span data-ttu-id="408a0-115">Содержит условия поиска, отправленные в исходном поисковом запросе.</span><span class="sxs-lookup"><span data-stu-id="408a0-115">Contains the search terms sent in the initial search query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="408a0-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="408a0-116">JSON representation</span></span>

<span data-ttu-id="408a0-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="408a0-117">The following is a JSON representation of the resource.</span></span>

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

