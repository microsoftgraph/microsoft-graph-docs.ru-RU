---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
ms.openlocfilehash: 120f1805196e40d652bd2fcd409f4ee3cd3203fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025430"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="af2f1-102">Тип ресурса SearchResult</span><span class="sxs-lookup"><span data-stu-id="af2f1-102">SearchResult resource type</span></span>

<span data-ttu-id="af2f1-103">Ресурс **SearchResult** указывает, что элемент представляет собой отклик на поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="af2f1-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="af2f1-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="af2f1-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="af2f1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="af2f1-105">Properties</span></span>

| <span data-ttu-id="af2f1-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="af2f1-106">Property</span></span>            | <span data-ttu-id="af2f1-107">Тип</span><span class="sxs-lookup"><span data-stu-id="af2f1-107">Type</span></span>   | <span data-ttu-id="af2f1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="af2f1-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="af2f1-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="af2f1-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="af2f1-110">Строка</span><span class="sxs-lookup"><span data-stu-id="af2f1-110">String</span></span> | <span data-ttu-id="af2f1-p101">URL-адрес обратного вызова, с помощью которого можно записывать данные телеметрии. Когда пользователь использует этот элемент, приложение должно выполнять запрос GET на этот URL-адрес, чтобы повышать качество результатов.</span><span class="sxs-lookup"><span data-stu-id="af2f1-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="af2f1-113">Заметки</span><span class="sxs-lookup"><span data-stu-id="af2f1-113">Remarks</span></span> 

<span data-ttu-id="af2f1-114">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="af2f1-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
