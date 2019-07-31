---
author: JeremyKelley
description: Ресурс SearchResult указывает, что элемент представляет собой отклик на поисковый запрос.
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 716a8147c9041ceee64993f9e90ad2f0f9ecb9e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008609"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="63c1b-103">Тип ресурса SearchResult</span><span class="sxs-lookup"><span data-stu-id="63c1b-103">SearchResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63c1b-104">Ресурс **SearchResult** указывает, что элемент представляет собой отклик на поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="63c1b-104">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="63c1b-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="63c1b-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="63c1b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="63c1b-106">Properties</span></span>

| <span data-ttu-id="63c1b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="63c1b-107">Property</span></span>            | <span data-ttu-id="63c1b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="63c1b-108">Type</span></span>   | <span data-ttu-id="63c1b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="63c1b-109">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="63c1b-110">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="63c1b-110">onClickTelemetryUrl</span></span> | <span data-ttu-id="63c1b-111">Строка</span><span class="sxs-lookup"><span data-stu-id="63c1b-111">String</span></span> | <span data-ttu-id="63c1b-p101">URL-адрес обратного вызова, с помощью которого можно записывать данные телеметрии. Когда пользователь использует этот элемент, приложение должно выполнять запрос GET на этот URL-адрес, чтобы повышать качество результатов.</span><span class="sxs-lookup"><span data-stu-id="63c1b-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="63c1b-114">Заметки</span><span class="sxs-lookup"><span data-stu-id="63c1b-114">Remarks</span></span> 

<span data-ttu-id="63c1b-115">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="63c1b-115">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
