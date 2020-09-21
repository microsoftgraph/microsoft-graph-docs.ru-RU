---
author: JeremyKelley
description: Ресурс SearchResult указывает, что элемент представляет собой отклик на поисковый запрос.
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8ee83da0ffdd5d2ed577ba1b7165c05f5a63b1e8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063949"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="4afda-103">Тип ресурса SearchResult</span><span class="sxs-lookup"><span data-stu-id="4afda-103">SearchResult resource type</span></span>

<span data-ttu-id="4afda-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4afda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4afda-105">Ресурс **SearchResult** указывает, что элемент представляет собой отклик на поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="4afda-105">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a><span data-ttu-id="4afda-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4afda-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "onClickTelemtryUrl" ],
  "@odata.type": "microsoft.graph.searchResult"
}-->

```json
{
  "onClickTelemetryUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="4afda-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4afda-107">Properties</span></span>

| <span data-ttu-id="4afda-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4afda-108">Property</span></span>            | <span data-ttu-id="4afda-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4afda-109">Type</span></span>   | <span data-ttu-id="4afda-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4afda-110">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="4afda-111">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="4afda-111">onClickTelemetryUrl</span></span> | <span data-ttu-id="4afda-112">Строка</span><span class="sxs-lookup"><span data-stu-id="4afda-112">String</span></span> | <span data-ttu-id="4afda-p101">URL-адрес обратного вызова, с помощью которого можно записывать данные телеметрии. Когда пользователь использует этот элемент, приложение должно выполнять запрос GET на этот URL-адрес, чтобы повышать качество результатов.</span><span class="sxs-lookup"><span data-stu-id="4afda-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="4afda-115">Заметки</span><span class="sxs-lookup"><span data-stu-id="4afda-115">Remarks</span></span>

<span data-ttu-id="4afda-116">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="4afda-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult",
  "suppressions": []
}
-->


