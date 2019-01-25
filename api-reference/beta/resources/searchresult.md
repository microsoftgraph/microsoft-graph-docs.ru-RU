---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
ms.openlocfilehash: c50f90787627732843e152a37a469c03340aa370
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511074"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="ca662-102">Тип ресурса SearchResult</span><span class="sxs-lookup"><span data-stu-id="ca662-102">SearchResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca662-103">Ресурс **SearchResult** указывает, что элемент представляет собой отклик на поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="ca662-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca662-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ca662-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="ca662-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca662-105">Properties</span></span>

| <span data-ttu-id="ca662-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca662-106">Property</span></span>            | <span data-ttu-id="ca662-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ca662-107">Type</span></span>   | <span data-ttu-id="ca662-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ca662-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="ca662-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="ca662-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="ca662-110">Строка</span><span class="sxs-lookup"><span data-stu-id="ca662-110">String</span></span> | <span data-ttu-id="ca662-p101">URL-адрес обратного вызова, с помощью которого можно записывать данные телеметрии. Когда пользователь использует этот элемент, приложение должно выполнять запрос GET на этот URL-адрес, чтобы повышать качество результатов.</span><span class="sxs-lookup"><span data-stu-id="ca662-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="ca662-113">Заметки</span><span class="sxs-lookup"><span data-stu-id="ca662-113">Remarks</span></span> 

<span data-ttu-id="ca662-114">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ca662-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult",
  "suppressions": [
    "Error: /api-reference/beta/resources/searchresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
