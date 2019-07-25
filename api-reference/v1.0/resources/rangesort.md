---
title: Тип ресурса RangeSort
description: Управляет операциями сортировки для объектов Range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1fa09d156210d7dbe31b5896be071663cc214c64
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891673"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="dc88e-103">Тип ресурса RangeSort</span><span class="sxs-lookup"><span data-stu-id="dc88e-103">RangeSort resource type</span></span>

<span data-ttu-id="dc88e-104">Управляет операциями сортировки для объектов Range.</span><span class="sxs-lookup"><span data-stu-id="dc88e-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="dc88e-105">Методы</span><span class="sxs-lookup"><span data-stu-id="dc88e-105">Methods</span></span>

| <span data-ttu-id="dc88e-106">Метод</span><span class="sxs-lookup"><span data-stu-id="dc88e-106">Method</span></span>           | <span data-ttu-id="dc88e-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dc88e-107">Return Type</span></span>    |<span data-ttu-id="dc88e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="dc88e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dc88e-109">Apply</span><span class="sxs-lookup"><span data-stu-id="dc88e-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="dc88e-110">Нет</span><span class="sxs-lookup"><span data-stu-id="dc88e-110">None</span></span>|<span data-ttu-id="dc88e-111">Выполняет сортировку.</span><span class="sxs-lookup"><span data-stu-id="dc88e-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc88e-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc88e-112">Properties</span></span>
<span data-ttu-id="dc88e-113">Нет</span><span class="sxs-lookup"><span data-stu-id="dc88e-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="dc88e-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="dc88e-114">Relationships</span></span>
<span data-ttu-id="dc88e-115">Нет</span><span class="sxs-lookup"><span data-stu-id="dc88e-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc88e-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dc88e-116">JSON representation</span></span>

<span data-ttu-id="dc88e-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc88e-117">Here is a JSON representation of the resource.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dc88e-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc88e-118">HTTP</span></span>](#tab/http)
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

##### <a name="request"></a><span data-ttu-id="dc88e-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc88e-119">Request</span></span>
<span data-ttu-id="dc88e-120">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc88e-120">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc88e-121">C#</span><span class="sxs-lookup"><span data-stu-id="dc88e-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-sort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc88e-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="dc88e-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-sort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc88e-123">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dc88e-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-sort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dc88e-124">Java</span><span class="sxs-lookup"><span data-stu-id="dc88e-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-sort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dc88e-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc88e-125">Response</span></span>
<span data-ttu-id="dc88e-126">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dc88e-126">Here is an example of the response.</span></span> 
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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
