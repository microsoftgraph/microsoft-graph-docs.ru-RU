---
title: Тип ресурса Сеарчреспонсе
description: Описание Сеарчреспонсе
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8582da8daf604952807e05376d98dabf16267052
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377780"
---
# <a name="searchresponse-resource-type"></a><span data-ttu-id="de55a-103">Тип ресурса Сеарчреспонсе</span><span class="sxs-lookup"><span data-stu-id="de55a-103">searchResponse resource type</span></span>

<span data-ttu-id="de55a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de55a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de55a-105">Представляет результаты из поискового запроса и термины, используемые для запроса.</span><span class="sxs-lookup"><span data-stu-id="de55a-105">Represents results from a search query, and the terms used for the query.</span></span> 

## <a name="properties"></a><span data-ttu-id="de55a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="de55a-106">Properties</span></span>

| <span data-ttu-id="de55a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="de55a-107">Property</span></span>     | <span data-ttu-id="de55a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="de55a-108">Type</span></span>        | <span data-ttu-id="de55a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="de55a-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="de55a-110">хитсконтаинерс</span><span class="sxs-lookup"><span data-stu-id="de55a-110">hitsContainers</span></span>|<span data-ttu-id="de55a-111">Коллекция [сеарчхитсконтаинер](searchhitscontainer.md)</span><span class="sxs-lookup"><span data-stu-id="de55a-111">[searchHitsContainer](searchhitscontainer.md) collection</span></span>|<span data-ttu-id="de55a-112">Коллекция результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="de55a-112">A collection of search results.</span></span>|
|<span data-ttu-id="de55a-113">searchTerms</span><span class="sxs-lookup"><span data-stu-id="de55a-113">searchTerms</span></span>|<span data-ttu-id="de55a-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="de55a-114">String collection</span></span>|<span data-ttu-id="de55a-115">Содержит условия поиска, отправленные в исходном поисковом запросе.</span><span class="sxs-lookup"><span data-stu-id="de55a-115">Contains the search terms sent in the initial search query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de55a-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="de55a-116">JSON representation</span></span>

<span data-ttu-id="de55a-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de55a-117">The following is a JSON representation of the resource.</span></span>

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

