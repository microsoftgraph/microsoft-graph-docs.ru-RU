---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
ms.openlocfilehash: 7e6bd6e6ff48ae34e197955d16a3df1d539a3c05
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080133"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="270f5-102">Тип ресурса SearchResult</span><span class="sxs-lookup"><span data-stu-id="270f5-102">SearchResult resource type</span></span>

> <span data-ttu-id="270f5-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="270f5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="270f5-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="270f5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="270f5-105">Ресурс **SearchResult** указывает, что элемент представляет собой отклик на поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="270f5-105">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="270f5-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="270f5-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="270f5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="270f5-107">Properties</span></span>

| <span data-ttu-id="270f5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="270f5-108">Property</span></span>            | <span data-ttu-id="270f5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="270f5-109">Type</span></span>   | <span data-ttu-id="270f5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="270f5-110">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="270f5-111">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="270f5-111">onClickTelemetryUrl</span></span> | <span data-ttu-id="270f5-112">String</span><span class="sxs-lookup"><span data-stu-id="270f5-112">String</span></span> | <span data-ttu-id="270f5-p102">URL-адрес обратного вызова, с помощью которого можно записывать данные телеметрии. Когда пользователь использует этот элемент, приложение должно выполнять запрос GET на этот URL-адрес, чтобы повышать качество результатов.</span><span class="sxs-lookup"><span data-stu-id="270f5-p102">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="270f5-115">Заметки</span><span class="sxs-lookup"><span data-stu-id="270f5-115">Remarks</span></span> 

<span data-ttu-id="270f5-116">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="270f5-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
