---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
ms.openlocfilehash: 5e8bcbc18975758586b012ee32fb32ce15313517
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876603"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="187f4-102">Тип ресурса SearchResult</span><span class="sxs-lookup"><span data-stu-id="187f4-102">SearchResult resource type</span></span>

<span data-ttu-id="187f4-103">Ресурс **SearchResult** указывает, что элемент представляет собой отклик на поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="187f4-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="187f4-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="187f4-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="187f4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="187f4-105">Properties</span></span>

| <span data-ttu-id="187f4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="187f4-106">Property</span></span>            | <span data-ttu-id="187f4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="187f4-107">Type</span></span>   | <span data-ttu-id="187f4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="187f4-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="187f4-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="187f4-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="187f4-110">Строка</span><span class="sxs-lookup"><span data-stu-id="187f4-110">String</span></span> | <span data-ttu-id="187f4-p101">URL-адрес обратного вызова, с помощью которого можно записывать данные телеметрии. Когда пользователь использует этот элемент, приложение должно выполнять запрос GET на этот URL-адрес, чтобы повышать качество результатов.</span><span class="sxs-lookup"><span data-stu-id="187f4-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="187f4-113">Заметки</span><span class="sxs-lookup"><span data-stu-id="187f4-113">Remarks</span></span> 

<span data-ttu-id="187f4-114">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="187f4-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
