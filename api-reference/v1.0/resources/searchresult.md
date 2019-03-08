---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
ms.openlocfilehash: ee6825860f5c1ed82c368b53eb3510175e7d3a11
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481232"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="f4571-102">Тип ресурса SearchResult</span><span class="sxs-lookup"><span data-stu-id="f4571-102">SearchResult resource type</span></span>

<span data-ttu-id="f4571-103">Ресурс **SearchResult** указывает, что элемент представляет собой отклик на поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="f4571-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4571-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f4571-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f4571-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4571-105">Properties</span></span>

| <span data-ttu-id="f4571-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4571-106">Property</span></span>            | <span data-ttu-id="f4571-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f4571-107">Type</span></span>   | <span data-ttu-id="f4571-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f4571-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="f4571-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="f4571-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="f4571-110">Строка</span><span class="sxs-lookup"><span data-stu-id="f4571-110">String</span></span> | <span data-ttu-id="f4571-p101">URL-адрес обратного вызова, с помощью которого можно записывать данные телеметрии. Когда пользователь использует этот элемент, приложение должно выполнять запрос GET на этот URL-адрес, чтобы повышать качество результатов.</span><span class="sxs-lookup"><span data-stu-id="f4571-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="f4571-113">Заметки</span><span class="sxs-lookup"><span data-stu-id="f4571-113">Remarks</span></span> 

<span data-ttu-id="f4571-114">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f4571-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
