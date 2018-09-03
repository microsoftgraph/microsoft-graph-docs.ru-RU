# <a name="rangesort-resource-type"></a><span data-ttu-id="fe3b1-101">Тип ресурса RangeSort</span><span class="sxs-lookup"><span data-stu-id="fe3b1-101">RangeSort resource type</span></span>

<span data-ttu-id="fe3b1-102">Управляет операциями сортировки для объектов Range.</span><span class="sxs-lookup"><span data-stu-id="fe3b1-102">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="fe3b1-103">Методы</span><span class="sxs-lookup"><span data-stu-id="fe3b1-103">Methods</span></span>

| <span data-ttu-id="fe3b1-104">Метод</span><span class="sxs-lookup"><span data-stu-id="fe3b1-104">Method</span></span>           | <span data-ttu-id="fe3b1-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fe3b1-105">Return Type</span></span>    |<span data-ttu-id="fe3b1-106">Описание</span><span class="sxs-lookup"><span data-stu-id="fe3b1-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fe3b1-107">Применить</span><span class="sxs-lookup"><span data-stu-id="fe3b1-107">Apply</span></span>](../api/rangesort_apply.md)|<span data-ttu-id="fe3b1-108">Нет</span><span class="sxs-lookup"><span data-stu-id="fe3b1-108">None</span></span>|<span data-ttu-id="fe3b1-109">Выполняет сортировку.</span><span class="sxs-lookup"><span data-stu-id="fe3b1-109">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="fe3b1-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe3b1-110">Properties</span></span>
<span data-ttu-id="fe3b1-111">Нет</span><span class="sxs-lookup"><span data-stu-id="fe3b1-111">None</span></span>

## <a name="relationships"></a><span data-ttu-id="fe3b1-112">Связи</span><span class="sxs-lookup"><span data-stu-id="fe3b1-112">Relationships</span></span>
<span data-ttu-id="fe3b1-113">Нет</span><span class="sxs-lookup"><span data-stu-id="fe3b1-113">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe3b1-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe3b1-114">JSON representation</span></span>

<span data-ttu-id="fe3b1-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe3b1-115">Here is a JSON representation of the resource.</span></span>

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

##### <a name="request"></a><span data-ttu-id="fe3b1-116">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe3b1-116">Request</span></span>
<span data-ttu-id="fe3b1-117">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe3b1-117">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="fe3b1-118">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe3b1-118">Response</span></span>
<span data-ttu-id="fe3b1-119">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fe3b1-119">Here is an example of the response.</span></span> 
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