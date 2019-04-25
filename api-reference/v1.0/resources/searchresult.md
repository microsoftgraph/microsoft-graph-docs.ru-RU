---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
ms.openlocfilehash: ee6825860f5c1ed82c368b53eb3510175e7d3a11
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579200"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="c570e-102">Тип ресурса SearchResult</span><span class="sxs-lookup"><span data-stu-id="c570e-102">SearchResult resource type</span></span>

<span data-ttu-id="c570e-103">Ресурс **SearchResult** указывает, что элемент представляет собой отклик на поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="c570e-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c570e-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c570e-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c570e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c570e-105">Properties</span></span>

| <span data-ttu-id="c570e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c570e-106">Property</span></span>            | <span data-ttu-id="c570e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c570e-107">Type</span></span>   | <span data-ttu-id="c570e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c570e-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="c570e-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="c570e-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="c570e-110">Строка</span><span class="sxs-lookup"><span data-stu-id="c570e-110">String</span></span> | <span data-ttu-id="c570e-p101">URL-адрес обратного вызова, с помощью которого можно записывать данные телеметрии. Когда пользователь использует этот элемент, приложение должно выполнять запрос GET на этот URL-адрес, чтобы повышать качество результатов.</span><span class="sxs-lookup"><span data-stu-id="c570e-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="c570e-113">Заметки</span><span class="sxs-lookup"><span data-stu-id="c570e-113">Remarks</span></span> 

<span data-ttu-id="c570e-114">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c570e-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
