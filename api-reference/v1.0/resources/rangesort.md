---
title: Тип ресурса RangeSort
description: Управляет операциями сортировки для объектов Range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6d1fb0be3feae69ff2cae34f360a0f78d46a6172
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947577"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="207db-103">Тип ресурса RangeSort</span><span class="sxs-lookup"><span data-stu-id="207db-103">RangeSort resource type</span></span>

<span data-ttu-id="207db-104">Управляет операциями сортировки для объектов Range.</span><span class="sxs-lookup"><span data-stu-id="207db-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="207db-105">Методы</span><span class="sxs-lookup"><span data-stu-id="207db-105">Methods</span></span>

| <span data-ttu-id="207db-106">Метод</span><span class="sxs-lookup"><span data-stu-id="207db-106">Method</span></span>           | <span data-ttu-id="207db-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="207db-107">Return Type</span></span>    |<span data-ttu-id="207db-108">Описание</span><span class="sxs-lookup"><span data-stu-id="207db-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="207db-109">Apply</span><span class="sxs-lookup"><span data-stu-id="207db-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="207db-110">Нет</span><span class="sxs-lookup"><span data-stu-id="207db-110">None</span></span>|<span data-ttu-id="207db-111">Выполняет сортировку.</span><span class="sxs-lookup"><span data-stu-id="207db-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="207db-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="207db-112">Properties</span></span>
<span data-ttu-id="207db-113">Нет</span><span class="sxs-lookup"><span data-stu-id="207db-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="207db-114">Связи</span><span class="sxs-lookup"><span data-stu-id="207db-114">Relationships</span></span>
<span data-ttu-id="207db-115">Нет</span><span class="sxs-lookup"><span data-stu-id="207db-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="207db-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="207db-116">JSON representation</span></span>

<span data-ttu-id="207db-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="207db-117">Here is a JSON representation of the resource.</span></span>

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

##### <a name="request"></a><span data-ttu-id="207db-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="207db-118">Request</span></span>
<span data-ttu-id="207db-119">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="207db-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="207db-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="207db-120">Response</span></span>
<span data-ttu-id="207db-121">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="207db-121">Here is an example of the response.</span></span> 
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
