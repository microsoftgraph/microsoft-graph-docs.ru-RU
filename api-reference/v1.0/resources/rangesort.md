---
title: Тип ресурса RangeSort
description: Управляет операциями сортировки для объектов Range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3204a72fe51d3afd3771c0e6775138277ef450e2
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601156"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="473c6-103">Тип ресурса RangeSort</span><span class="sxs-lookup"><span data-stu-id="473c6-103">RangeSort resource type</span></span>

<span data-ttu-id="473c6-104">Управляет операциями сортировки для объектов Range.</span><span class="sxs-lookup"><span data-stu-id="473c6-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="473c6-105">Методы</span><span class="sxs-lookup"><span data-stu-id="473c6-105">Methods</span></span>

| <span data-ttu-id="473c6-106">Метод</span><span class="sxs-lookup"><span data-stu-id="473c6-106">Method</span></span>           | <span data-ttu-id="473c6-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="473c6-107">Return Type</span></span>    |<span data-ttu-id="473c6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="473c6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="473c6-109">Apply</span><span class="sxs-lookup"><span data-stu-id="473c6-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="473c6-110">Нет</span><span class="sxs-lookup"><span data-stu-id="473c6-110">None</span></span>|<span data-ttu-id="473c6-111">Выполняет сортировку.</span><span class="sxs-lookup"><span data-stu-id="473c6-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="473c6-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="473c6-112">Properties</span></span>
<span data-ttu-id="473c6-113">Нет</span><span class="sxs-lookup"><span data-stu-id="473c6-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="473c6-114">Связи</span><span class="sxs-lookup"><span data-stu-id="473c6-114">Relationships</span></span>
<span data-ttu-id="473c6-115">Нет</span><span class="sxs-lookup"><span data-stu-id="473c6-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="473c6-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="473c6-116">JSON representation</span></span>

<span data-ttu-id="473c6-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="473c6-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeSort"
}-->

```json
{
}
```

##### <a name="request"></a><span data-ttu-id="473c6-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="473c6-118">Request</span></span>
<span data-ttu-id="473c6-119">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="473c6-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="473c6-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="473c6-120">Response</span></span>
<span data-ttu-id="473c6-121">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="473c6-121">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeSort"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="473c6-122">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="473c6-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="473c6-123">Языках</span><span class="sxs-lookup"><span data-stu-id="473c6-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_sort-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="473c6-124">Язык</span><span class="sxs-lookup"><span data-stu-id="473c6-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_sort-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/resources/rangesort.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/resources/rangesort.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
