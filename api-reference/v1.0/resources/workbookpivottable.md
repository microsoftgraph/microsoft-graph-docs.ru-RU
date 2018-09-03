# <a name="pivottable-resource-type"></a><span data-ttu-id="fdff2-101">Тип ресурсов pivotTable</span><span class="sxs-lookup"><span data-stu-id="fdff2-101">pivotTable resource type</span></span>

<span data-ttu-id="fdff2-102">Представляет сводную таблицу Excel.</span><span class="sxs-lookup"><span data-stu-id="fdff2-102">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="fdff2-103">Методы</span><span class="sxs-lookup"><span data-stu-id="fdff2-103">Methods</span></span>

| <span data-ttu-id="fdff2-104">Метод</span><span class="sxs-lookup"><span data-stu-id="fdff2-104">Method</span></span>           | <span data-ttu-id="fdff2-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fdff2-105">Return Type</span></span>    |<span data-ttu-id="fdff2-106">Описание</span><span class="sxs-lookup"><span data-stu-id="fdff2-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fdff2-107">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="fdff2-107">Get workbookPivotTable</span></span>](../api/workbookpivottable_get.md) | [<span data-ttu-id="fdff2-108">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="fdff2-108">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="fdff2-109">Чтение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="fdff2-109">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="fdff2-110">Refresh</span><span class="sxs-lookup"><span data-stu-id="fdff2-110">Refresh</span></span>](../api/workbookpivottable_refresh.md)|<span data-ttu-id="fdff2-111">Нет</span><span class="sxs-lookup"><span data-stu-id="fdff2-111">None</span></span>|<span data-ttu-id="fdff2-112">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="fdff2-112">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="fdff2-113">Refreshall</span><span class="sxs-lookup"><span data-stu-id="fdff2-113">Refreshall</span></span>](../api/workbookpivottable_refreshall.md)|<span data-ttu-id="fdff2-114">Нет</span><span class="sxs-lookup"><span data-stu-id="fdff2-114">None</span></span>|<span data-ttu-id="fdff2-p101">Обновляет все таблицы на заданном листе. Обратите внимание, что это действие доступно только в коллекции сводных таблиц.</span><span class="sxs-lookup"><span data-stu-id="fdff2-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="fdff2-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="fdff2-117">Properties</span></span>
| <span data-ttu-id="fdff2-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdff2-118">Property</span></span>     | <span data-ttu-id="fdff2-119">Тип</span><span class="sxs-lookup"><span data-stu-id="fdff2-119">Type</span></span>   |<span data-ttu-id="fdff2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fdff2-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdff2-121">id</span><span class="sxs-lookup"><span data-stu-id="fdff2-121">id</span></span>|<span data-ttu-id="fdff2-122">Строка</span><span class="sxs-lookup"><span data-stu-id="fdff2-122">String</span></span>| <span data-ttu-id="fdff2-p102">Идентификатор сводной таблицы.   Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fdff2-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="fdff2-125">name</span><span class="sxs-lookup"><span data-stu-id="fdff2-125">name</span></span>|<span data-ttu-id="fdff2-126">Строка</span><span class="sxs-lookup"><span data-stu-id="fdff2-126">String</span></span>|<span data-ttu-id="fdff2-127">Имя сводной таблицы.</span><span class="sxs-lookup"><span data-stu-id="fdff2-127">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="fdff2-128">Связи</span><span class="sxs-lookup"><span data-stu-id="fdff2-128">Relationships</span></span>
| <span data-ttu-id="fdff2-129">Связь</span><span class="sxs-lookup"><span data-stu-id="fdff2-129">Relationship</span></span> | <span data-ttu-id="fdff2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fdff2-130">Type</span></span>   |<span data-ttu-id="fdff2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fdff2-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdff2-132">лист</span><span class="sxs-lookup"><span data-stu-id="fdff2-132">worksheet</span></span>|[<span data-ttu-id="fdff2-133">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="fdff2-133">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="fdff2-p103">Лист, содержащий текущую сводную таблицу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fdff2-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="fdff2-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fdff2-136">JSON representation</span></span>
<span data-ttu-id="fdff2-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdff2-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
