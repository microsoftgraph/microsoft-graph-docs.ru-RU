---
author: JeremyKelley
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
description: Ресурс SearchResult указывает, что элемент представляет собой отклик на поисковый запрос.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: aac8ee9c4dea8ba7744e5c86d865b4d2f75a37d8
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240103"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="709ae-103">Тип ресурса SearchResult</span><span class="sxs-lookup"><span data-stu-id="709ae-103">SearchResult resource type</span></span>

<span data-ttu-id="709ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="709ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="709ae-105">Ресурс **SearchResult** указывает, что элемент представляет собой отклик на поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="709ae-105">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="709ae-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="709ae-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="709ae-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="709ae-107">Properties</span></span>

| <span data-ttu-id="709ae-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="709ae-108">Property</span></span>            | <span data-ttu-id="709ae-109">Тип</span><span class="sxs-lookup"><span data-stu-id="709ae-109">Type</span></span>   | <span data-ttu-id="709ae-110">Описание</span><span class="sxs-lookup"><span data-stu-id="709ae-110">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="709ae-111">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="709ae-111">onClickTelemetryUrl</span></span> | <span data-ttu-id="709ae-112">Строка</span><span class="sxs-lookup"><span data-stu-id="709ae-112">String</span></span> | <span data-ttu-id="709ae-p101">URL-адрес обратного вызова, с помощью которого можно записывать данные телеметрии. Когда пользователь использует этот элемент, приложение должно выполнять запрос GET на этот URL-адрес, чтобы повышать качество результатов.</span><span class="sxs-lookup"><span data-stu-id="709ae-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="709ae-115">Заметки</span><span class="sxs-lookup"><span data-stu-id="709ae-115">Remarks</span></span> 

<span data-ttu-id="709ae-116">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="709ae-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->

