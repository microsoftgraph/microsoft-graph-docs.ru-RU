---
title: Тип ресурса RangeSort
description: Управляет операциями сортировки для объектов Range.
ms.openlocfilehash: 09f9a6763c634ee12251651a650d29528a534084
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025410"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="7ff03-103">Тип ресурса RangeSort</span><span class="sxs-lookup"><span data-stu-id="7ff03-103">RangeSort resource type</span></span>

<span data-ttu-id="7ff03-104">Управляет операциями сортировки для объектов Range.</span><span class="sxs-lookup"><span data-stu-id="7ff03-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="7ff03-105">Методы</span><span class="sxs-lookup"><span data-stu-id="7ff03-105">Methods</span></span>

| <span data-ttu-id="7ff03-106">Метод</span><span class="sxs-lookup"><span data-stu-id="7ff03-106">Method</span></span>           | <span data-ttu-id="7ff03-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7ff03-107">Return Type</span></span>    |<span data-ttu-id="7ff03-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7ff03-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7ff03-109">Apply</span><span class="sxs-lookup"><span data-stu-id="7ff03-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="7ff03-110">Нет</span><span class="sxs-lookup"><span data-stu-id="7ff03-110">None</span></span>|<span data-ttu-id="7ff03-111">Выполняет сортировку.</span><span class="sxs-lookup"><span data-stu-id="7ff03-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="7ff03-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ff03-112">Properties</span></span>
<span data-ttu-id="7ff03-113">Нет</span><span class="sxs-lookup"><span data-stu-id="7ff03-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="7ff03-114">Связи</span><span class="sxs-lookup"><span data-stu-id="7ff03-114">Relationships</span></span>
<span data-ttu-id="7ff03-115">Нет</span><span class="sxs-lookup"><span data-stu-id="7ff03-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ff03-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ff03-116">JSON representation</span></span>

<span data-ttu-id="7ff03-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ff03-117">Here is a JSON representation of the resource.</span></span>

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

##### <a name="request"></a><span data-ttu-id="7ff03-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ff03-118">Request</span></span>
<span data-ttu-id="7ff03-119">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ff03-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="7ff03-120">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ff03-120">Response</span></span>
<span data-ttu-id="7ff03-121">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7ff03-121">Here is an example of the response.</span></span> 
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
  "tocPath": ""
}-->