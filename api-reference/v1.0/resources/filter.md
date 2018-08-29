# <a name="filter-resource-type"></a><span data-ttu-id="c4e91-101">Тип ресурса Filter</span><span class="sxs-lookup"><span data-stu-id="c4e91-101">Filter resource type</span></span>

<span data-ttu-id="c4e91-102">Управляет фильтрацией столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="c4e91-102">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="c4e91-103">Методы</span><span class="sxs-lookup"><span data-stu-id="c4e91-103">Methods</span></span>

| <span data-ttu-id="c4e91-104">Метод</span><span class="sxs-lookup"><span data-stu-id="c4e91-104">Method</span></span>           | <span data-ttu-id="c4e91-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c4e91-105">Return Type</span></span>    |<span data-ttu-id="c4e91-106">Описание</span><span class="sxs-lookup"><span data-stu-id="c4e91-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c4e91-107">Применить</span><span class="sxs-lookup"><span data-stu-id="c4e91-107">Apply</span></span>](../api/filter_apply.md)|<span data-ttu-id="c4e91-108">Нет</span><span class="sxs-lookup"><span data-stu-id="c4e91-108">None</span></span>|<span data-ttu-id="c4e91-109">Применяет заданные условия фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="c4e91-109">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="c4e91-110">Clear</span><span class="sxs-lookup"><span data-stu-id="c4e91-110">Clear</span></span>](../api/filter_clear.md)|<span data-ttu-id="c4e91-111">Нет</span><span class="sxs-lookup"><span data-stu-id="c4e91-111">None</span></span>|<span data-ttu-id="c4e91-112">Сбрасывает фильтр для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="c4e91-112">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="c4e91-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4e91-113">Properties</span></span>

| <span data-ttu-id="c4e91-114">Имя</span><span class="sxs-lookup"><span data-stu-id="c4e91-114">Name</span></span> | <span data-ttu-id="c4e91-115">Тип</span><span class="sxs-lookup"><span data-stu-id="c4e91-115">Type</span></span>   |<span data-ttu-id="c4e91-116">Описание</span><span class="sxs-lookup"><span data-stu-id="c4e91-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4e91-117">criteria</span><span class="sxs-lookup"><span data-stu-id="c4e91-117">criteria</span></span>|[<span data-ttu-id="c4e91-118">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="c4e91-118">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="c4e91-p101">Текущий фильтр, заданный для определенного столбца. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4e91-p101">The currently applied filter on the given column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4e91-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4e91-121">JSON representation</span></span>

<span data-ttu-id="c4e91-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4e91-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
  "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->