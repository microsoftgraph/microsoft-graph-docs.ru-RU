---
author: JeremyKelley
description: Ресурс SearchResult указывает, что элемент представляет собой отклик на поисковый запрос.
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: cc819d8b81138ef279735d1daead9839d7f3b93f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520887"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="91244-103">Тип ресурса SearchResult</span><span class="sxs-lookup"><span data-stu-id="91244-103">SearchResult resource type</span></span>

<span data-ttu-id="91244-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="91244-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91244-105">Ресурс **SearchResult** указывает, что элемент представляет собой отклик на поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="91244-105">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a><span data-ttu-id="91244-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="91244-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="91244-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="91244-107">Properties</span></span>

| <span data-ttu-id="91244-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="91244-108">Property</span></span>            | <span data-ttu-id="91244-109">Тип</span><span class="sxs-lookup"><span data-stu-id="91244-109">Type</span></span>   | <span data-ttu-id="91244-110">Описание</span><span class="sxs-lookup"><span data-stu-id="91244-110">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="91244-111">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="91244-111">onClickTelemetryUrl</span></span> | <span data-ttu-id="91244-112">Строка</span><span class="sxs-lookup"><span data-stu-id="91244-112">String</span></span> | <span data-ttu-id="91244-p101">URL-адрес обратного вызова, с помощью которого можно записывать данные телеметрии. Когда пользователь использует этот элемент, приложение должно выполнять запрос GET на этот URL-адрес, чтобы повышать качество результатов.</span><span class="sxs-lookup"><span data-stu-id="91244-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="91244-115">Заметки</span><span class="sxs-lookup"><span data-stu-id="91244-115">Remarks</span></span>

<span data-ttu-id="91244-116">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="91244-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
