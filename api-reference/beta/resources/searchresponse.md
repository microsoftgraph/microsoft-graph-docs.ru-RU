---
title: Тип ресурса Сеарчреспонсе
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6b433e5aba652a9f68d017975e0651edac4e2ffb
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703997"
---
# <a name="searchresponse-resource-type"></a><span data-ttu-id="0d897-103">Тип ресурса Сеарчреспонсе</span><span class="sxs-lookup"><span data-stu-id="0d897-103">searchResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d897-104">Сеарчреспонсе содержит результаты из поискового запроса.</span><span class="sxs-lookup"><span data-stu-id="0d897-104">The searchResponse contains the results from the search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="0d897-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d897-105">Properties</span></span>

| <span data-ttu-id="0d897-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d897-106">Property</span></span>     | <span data-ttu-id="0d897-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0d897-107">Type</span></span>        | <span data-ttu-id="0d897-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0d897-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0d897-109">хитсконтаинерс</span><span class="sxs-lookup"><span data-stu-id="0d897-109">hitsContainers</span></span>|<span data-ttu-id="0d897-110">Коллекция [сеарчхитсконтаинер](searchhitscontainer.md)</span><span class="sxs-lookup"><span data-stu-id="0d897-110">[searchHitsContainer](searchhitscontainer.md) collection</span></span>|<span data-ttu-id="0d897-111">Коллекция результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="0d897-111">A collection of search results.</span></span>|
|<span data-ttu-id="0d897-112">searchTerms</span><span class="sxs-lookup"><span data-stu-id="0d897-112">searchTerms</span></span>|<span data-ttu-id="0d897-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0d897-113">String collection</span></span>|<span data-ttu-id="0d897-114">Содержит условия поиска, отправленные в исходном поисковом запросе.</span><span class="sxs-lookup"><span data-stu-id="0d897-114">Contains the search terms sent in the initial search query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d897-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d897-115">JSON representation</span></span>

<span data-ttu-id="0d897-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d897-116">The following is a JSON representation of the resource.</span></span>

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