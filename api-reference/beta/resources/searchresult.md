---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
ms.openlocfilehash: 025d18a48105ddb5834040aba5944a9bd408cfbc
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480385"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="529eb-102">Тип ресурса SearchResult</span><span class="sxs-lookup"><span data-stu-id="529eb-102">SearchResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="529eb-103">Ресурс **SearchResult** указывает, что элемент представляет собой отклик на поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="529eb-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="529eb-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="529eb-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="529eb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="529eb-105">Properties</span></span>

| <span data-ttu-id="529eb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="529eb-106">Property</span></span>            | <span data-ttu-id="529eb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="529eb-107">Type</span></span>   | <span data-ttu-id="529eb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="529eb-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="529eb-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="529eb-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="529eb-110">Строка</span><span class="sxs-lookup"><span data-stu-id="529eb-110">String</span></span> | <span data-ttu-id="529eb-p101">URL-адрес обратного вызова, с помощью которого можно записывать данные телеметрии. Когда пользователь использует этот элемент, приложение должно выполнять запрос GET на этот URL-адрес, чтобы повышать качество результатов.</span><span class="sxs-lookup"><span data-stu-id="529eb-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="529eb-113">Заметки</span><span class="sxs-lookup"><span data-stu-id="529eb-113">Remarks</span></span> 

<span data-ttu-id="529eb-114">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="529eb-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
