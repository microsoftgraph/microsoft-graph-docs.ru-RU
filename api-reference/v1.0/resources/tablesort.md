# <a name="tablesort-resource-type"></a><span data-ttu-id="8e8e6-101">Тип ресурса TableSort</span><span class="sxs-lookup"><span data-stu-id="8e8e6-101">TableSort resource type</span></span>

<span data-ttu-id="8e8e6-102">Управляет операциями сортировки для объектов Table.</span><span class="sxs-lookup"><span data-stu-id="8e8e6-102">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="8e8e6-103">Методы</span><span class="sxs-lookup"><span data-stu-id="8e8e6-103">Methods</span></span>

| <span data-ttu-id="8e8e6-104">Метод</span><span class="sxs-lookup"><span data-stu-id="8e8e6-104">Method</span></span>           | <span data-ttu-id="8e8e6-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8e8e6-105">Return Type</span></span>    |<span data-ttu-id="8e8e6-106">Описание</span><span class="sxs-lookup"><span data-stu-id="8e8e6-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8e8e6-107">Получение объекта TableSort</span><span class="sxs-lookup"><span data-stu-id="8e8e6-107">Get TableSort</span></span>](../api/tablesort_get.md) | [<span data-ttu-id="8e8e6-108">WorkbookTableSort</span><span class="sxs-lookup"><span data-stu-id="8e8e6-108">WorkbookTableSort</span></span>](tablesort.md) |<span data-ttu-id="8e8e6-109">Чтение свойств и связей объекта tableSort.</span><span class="sxs-lookup"><span data-stu-id="8e8e6-109">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="8e8e6-110">Apply</span><span class="sxs-lookup"><span data-stu-id="8e8e6-110">Apply</span></span>](../api/tablesort_apply.md)|<span data-ttu-id="8e8e6-111">Нет</span><span class="sxs-lookup"><span data-stu-id="8e8e6-111">None</span></span>|<span data-ttu-id="8e8e6-112">Выполняет сортировку.</span><span class="sxs-lookup"><span data-stu-id="8e8e6-112">Perform a sort operation.</span></span>|
|[<span data-ttu-id="8e8e6-113">Clear</span><span class="sxs-lookup"><span data-stu-id="8e8e6-113">Clear</span></span>](../api/tablesort_clear.md)|<span data-ttu-id="8e8e6-114">Нет</span><span class="sxs-lookup"><span data-stu-id="8e8e6-114">None</span></span>|<span data-ttu-id="8e8e6-p101">Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="8e8e6-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="8e8e6-117">Reapply</span><span class="sxs-lookup"><span data-stu-id="8e8e6-117">Reapply</span></span>](../api/tablesort_reapply.md)|<span data-ttu-id="8e8e6-118">Нет</span><span class="sxs-lookup"><span data-stu-id="8e8e6-118">None</span></span>|<span data-ttu-id="8e8e6-119">Повторно применяет текущие параметры сортировки к таблице.</span><span class="sxs-lookup"><span data-stu-id="8e8e6-119">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="8e8e6-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e8e6-120">Properties</span></span>
| <span data-ttu-id="8e8e6-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e8e6-121">Property</span></span>     | <span data-ttu-id="8e8e6-122">Тип</span><span class="sxs-lookup"><span data-stu-id="8e8e6-122">Type</span></span>   |<span data-ttu-id="8e8e6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8e8e6-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e8e6-124">fields</span><span class="sxs-lookup"><span data-stu-id="8e8e6-124">fields</span></span>|<span data-ttu-id="8e8e6-125">Коллекция [WorkbookSortField](sortfield.md)</span><span class="sxs-lookup"><span data-stu-id="8e8e6-125">[WorkbookSortField](sortfield.md) collection</span></span>|<span data-ttu-id="8e8e6-p102">Указывает текущие условия, которые использовались при последней сортировке таблицы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e8e6-p102">Represents the current conditions used to last sort the table. Read-only.</span></span>|
|<span data-ttu-id="8e8e6-128">matchCase</span><span class="sxs-lookup"><span data-stu-id="8e8e6-128">matchCase</span></span>|<span data-ttu-id="8e8e6-129">логический</span><span class="sxs-lookup"><span data-stu-id="8e8e6-129">boolean</span></span>|<span data-ttu-id="8e8e6-p103">Указывает, учитывался ли регистр при последней сортировке таблице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e8e6-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="8e8e6-132">method</span><span class="sxs-lookup"><span data-stu-id="8e8e6-132">method</span></span>|<span data-ttu-id="8e8e6-133">строка</span><span class="sxs-lookup"><span data-stu-id="8e8e6-133">string</span></span>|<span data-ttu-id="8e8e6-134">Представляет метод сортировки китайских знаков, который в последний раз использовался для сортировки таблицы.</span><span class="sxs-lookup"><span data-stu-id="8e8e6-134">Represents Chinese character ordering method last used to sort the table. Possible values are: , . Read-only.</span></span> <span data-ttu-id="8e8e6-135">Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="8e8e6-135">The possible values are:</span></span> <span data-ttu-id="8e8e6-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e8e6-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8e8e6-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e8e6-137">JSON representation</span></span>

<span data-ttu-id="8e8e6-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e8e6-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->