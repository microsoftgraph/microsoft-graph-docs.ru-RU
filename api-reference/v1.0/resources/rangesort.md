---
title: Тип ресурса RangeSort
description: Управляет операциями сортировки для объектов Range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 4964162d6c3380f3dcbe12ef0ed6ce0009149bb3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028261"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="8a47d-103">Тип ресурса RangeSort</span><span class="sxs-lookup"><span data-stu-id="8a47d-103">RangeSort resource type</span></span>

<span data-ttu-id="8a47d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a47d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a47d-105">Управляет операциями сортировки для объектов Range.</span><span class="sxs-lookup"><span data-stu-id="8a47d-105">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="8a47d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8a47d-106">Methods</span></span>

| <span data-ttu-id="8a47d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8a47d-107">Method</span></span>           | <span data-ttu-id="8a47d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8a47d-108">Return Type</span></span>    |<span data-ttu-id="8a47d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8a47d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8a47d-110">Apply</span><span class="sxs-lookup"><span data-stu-id="8a47d-110">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="8a47d-111">Нет</span><span class="sxs-lookup"><span data-stu-id="8a47d-111">None</span></span>|<span data-ttu-id="8a47d-112">Выполняет сортировку.</span><span class="sxs-lookup"><span data-stu-id="8a47d-112">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="8a47d-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a47d-113">Properties</span></span>
<span data-ttu-id="8a47d-114">Нет</span><span class="sxs-lookup"><span data-stu-id="8a47d-114">None</span></span>

## <a name="relationships"></a><span data-ttu-id="8a47d-115">Связи</span><span class="sxs-lookup"><span data-stu-id="8a47d-115">Relationships</span></span>
<span data-ttu-id="8a47d-116">Нет</span><span class="sxs-lookup"><span data-stu-id="8a47d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a47d-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a47d-117">JSON representation</span></span>

<span data-ttu-id="8a47d-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a47d-118">Here is a JSON representation of the resource.</span></span>


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

##### <a name="request"></a><span data-ttu-id="8a47d-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a47d-119">Request</span></span>
<span data-ttu-id="8a47d-120">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a47d-120">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8a47d-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a47d-121">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```
# <a name="c"></a>[<span data-ttu-id="8a47d-122">C#</span><span class="sxs-lookup"><span data-stu-id="8a47d-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-sort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a47d-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a47d-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-sort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a47d-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a47d-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-sort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a47d-125">Java</span><span class="sxs-lookup"><span data-stu-id="8a47d-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-sort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8a47d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a47d-126">Response</span></span>
<span data-ttu-id="8a47d-127">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8a47d-127">Here is an example of the response.</span></span> 
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

