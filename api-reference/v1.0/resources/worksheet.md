---
title: Тип ресурса Worksheet
description: Лист Excel представляет собой сетку ячеек. Он может содержать данные, таблицы, диаграммы и т. д.
localization_priority: Priority
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 60e31738329943d96e1a4f3ea8293851e759eaff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983872"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="279cf-104">Тип ресурса Worksheet</span><span class="sxs-lookup"><span data-stu-id="279cf-104">Worksheet resource type</span></span>

<span data-ttu-id="279cf-p102">Лист Excel представляет собой сетку ячеек. Он может содержать данные, таблицы, диаграммы и т. д.</span><span class="sxs-lookup"><span data-stu-id="279cf-p102">An Excel worksheet is a grid of cells. It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="279cf-107">Методы</span><span class="sxs-lookup"><span data-stu-id="279cf-107">Methods</span></span>

| <span data-ttu-id="279cf-108">Метод</span><span class="sxs-lookup"><span data-stu-id="279cf-108">Method</span></span>           | <span data-ttu-id="279cf-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="279cf-109">Return Type</span></span>    |<span data-ttu-id="279cf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="279cf-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="279cf-111">Получение объекта Worksheet</span><span class="sxs-lookup"><span data-stu-id="279cf-111">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="279cf-112">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="279cf-112">WorkbookWorksheet</span></span>](worksheet.md) |<span data-ttu-id="279cf-113">Чтение свойств и связей объекта листа.</span><span class="sxs-lookup"><span data-stu-id="279cf-113">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="279cf-114">Создание объекта Chart</span><span class="sxs-lookup"><span data-stu-id="279cf-114">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="279cf-115">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="279cf-115">WorkbookChart</span></span>](chart.md)| <span data-ttu-id="279cf-116">Создание диаграммы путем добавления в коллекцию диаграмм.</span><span class="sxs-lookup"><span data-stu-id="279cf-116">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="279cf-117">List names</span><span class="sxs-lookup"><span data-stu-id="279cf-117">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="279cf-118">[WorkbookNamedItem](nameditem.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="279cf-118">[WorkbookNamedItem](nameditem.md) collection</span></span>| <span data-ttu-id="279cf-119">Получение коллекции именованных элементов, связанной с листом.</span><span class="sxs-lookup"><span data-stu-id="279cf-119">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="279cf-120">List charts</span><span class="sxs-lookup"><span data-stu-id="279cf-120">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="279cf-121">[WorkbookChart](chart.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="279cf-121">[WorkbookChart](chart.md) collection</span></span>| <span data-ttu-id="279cf-122">Получение коллекции объектов Chart.</span><span class="sxs-lookup"><span data-stu-id="279cf-122">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="279cf-123">Создание объекта Table</span><span class="sxs-lookup"><span data-stu-id="279cf-123">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="279cf-124">WorkbookTable</span><span class="sxs-lookup"><span data-stu-id="279cf-124">WorkbookTable</span></span>](table.md)| <span data-ttu-id="279cf-125">Создание таблицы путем добавления в коллекцию таблиц.</span><span class="sxs-lookup"><span data-stu-id="279cf-125">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="279cf-126">Список таблиц</span><span class="sxs-lookup"><span data-stu-id="279cf-126">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="279cf-127">[WorkbookTable](table.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="279cf-127">[WorkbookTable](table.md) collection</span></span>| <span data-ttu-id="279cf-128">Получение коллекции объектов Table.</span><span class="sxs-lookup"><span data-stu-id="279cf-128">Get a Table object collection.</span></span>|
|<span data-ttu-id="279cf-129">[обновление](../api/worksheet-update.md).</span><span class="sxs-lookup"><span data-stu-id="279cf-129">[Update](../api/worksheet-update.md)</span></span> | [<span data-ttu-id="279cf-130">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="279cf-130">WorkbookWorksheet</span></span>](worksheet.md)   |<span data-ttu-id="279cf-131">Обновление объекта Worksheet.</span><span class="sxs-lookup"><span data-stu-id="279cf-131">Update Worksheet object.</span></span> |
|[<span data-ttu-id="279cf-132">Cell</span><span class="sxs-lookup"><span data-stu-id="279cf-132">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="279cf-133">Range</span><span class="sxs-lookup"><span data-stu-id="279cf-133">Range</span></span>](range.md)|<span data-ttu-id="279cf-p103">Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.</span><span class="sxs-lookup"><span data-stu-id="279cf-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="279cf-136">Range</span><span class="sxs-lookup"><span data-stu-id="279cf-136">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="279cf-137">Range</span><span class="sxs-lookup"><span data-stu-id="279cf-137">Range</span></span>](range.md)|<span data-ttu-id="279cf-138">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="279cf-138">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="279cf-139">Usedrange</span><span class="sxs-lookup"><span data-stu-id="279cf-139">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="279cf-140">Range</span><span class="sxs-lookup"><span data-stu-id="279cf-140">Range</span></span>](range.md)|<span data-ttu-id="279cf-p104">Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.</span><span class="sxs-lookup"><span data-stu-id="279cf-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="279cf-143">Delete</span><span class="sxs-lookup"><span data-stu-id="279cf-143">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="279cf-144">Нет</span><span class="sxs-lookup"><span data-stu-id="279cf-144">None</span></span>|<span data-ttu-id="279cf-145">Удаляет лист из книги.</span><span class="sxs-lookup"><span data-stu-id="279cf-145">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="279cf-146">List</span><span class="sxs-lookup"><span data-stu-id="279cf-146">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="279cf-147">[WorkbookWorksheet](worksheet.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="279cf-147">[WorkbookWorksheet](worksheet.md) collection</span></span> |<span data-ttu-id="279cf-148">Получение коллекции объектов листов.</span><span class="sxs-lookup"><span data-stu-id="279cf-148">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="279cf-149">Add</span><span class="sxs-lookup"><span data-stu-id="279cf-149">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="279cf-150">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="279cf-150">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="279cf-p105">Добавляет новый лист в книгу. Лист будет добавлен после существующих листов.</span><span class="sxs-lookup"><span data-stu-id="279cf-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="279cf-153">Получение списка pivotTables</span><span class="sxs-lookup"><span data-stu-id="279cf-153">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="279cf-154">Коллекция [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="279cf-154">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="279cf-155">Получение коллекции объектов workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="279cf-155">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="279cf-156">Свойства</span><span class="sxs-lookup"><span data-stu-id="279cf-156">Properties</span></span>
| <span data-ttu-id="279cf-157">Свойство</span><span class="sxs-lookup"><span data-stu-id="279cf-157">Property</span></span>     | <span data-ttu-id="279cf-158">Тип</span><span class="sxs-lookup"><span data-stu-id="279cf-158">Type</span></span>   |<span data-ttu-id="279cf-159">Описание</span><span class="sxs-lookup"><span data-stu-id="279cf-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="279cf-160">id</span><span class="sxs-lookup"><span data-stu-id="279cf-160">id</span></span>|<span data-ttu-id="279cf-161">строка</span><span class="sxs-lookup"><span data-stu-id="279cf-161">string</span></span>|<span data-ttu-id="279cf-p106">Возвращает значение, однозначно идентифицирующее лист в данной книге. Значение идентификатора остается прежним, даже если переименовать или переместить лист. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="279cf-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="279cf-165">name</span><span class="sxs-lookup"><span data-stu-id="279cf-165">name</span></span>|<span data-ttu-id="279cf-166">строка</span><span class="sxs-lookup"><span data-stu-id="279cf-166">string</span></span>|<span data-ttu-id="279cf-167">Отображаемое имя листа.</span><span class="sxs-lookup"><span data-stu-id="279cf-167">The display name of the worksheet.</span></span>|
|<span data-ttu-id="279cf-168">position</span><span class="sxs-lookup"><span data-stu-id="279cf-168">position</span></span>|<span data-ttu-id="279cf-169">int</span><span class="sxs-lookup"><span data-stu-id="279cf-169">int</span></span>|<span data-ttu-id="279cf-170">Положение листа (начиная с нуля) в книге.</span><span class="sxs-lookup"><span data-stu-id="279cf-170">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="279cf-171">visibility</span><span class="sxs-lookup"><span data-stu-id="279cf-171">visibility</span></span>|<span data-ttu-id="279cf-172">строка</span><span class="sxs-lookup"><span data-stu-id="279cf-172">string</span></span>|<span data-ttu-id="279cf-173">Видимость рабочего листа.</span><span class="sxs-lookup"><span data-stu-id="279cf-173">The Visibility of the worksheet.</span></span> <span data-ttu-id="279cf-174">Возможные значения: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="279cf-174">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="279cf-175">Связи</span><span class="sxs-lookup"><span data-stu-id="279cf-175">Relationships</span></span>
| <span data-ttu-id="279cf-176">Связь</span><span class="sxs-lookup"><span data-stu-id="279cf-176">Relationship</span></span> | <span data-ttu-id="279cf-177">Тип</span><span class="sxs-lookup"><span data-stu-id="279cf-177">Type</span></span>   |<span data-ttu-id="279cf-178">Описание</span><span class="sxs-lookup"><span data-stu-id="279cf-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="279cf-179">charts</span><span class="sxs-lookup"><span data-stu-id="279cf-179">charts</span></span>|<span data-ttu-id="279cf-180">[WorkbookChart](chart.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="279cf-180">[WorkbookChart](chart.md) collection</span></span>|<span data-ttu-id="279cf-p108">Возвращает коллекцию диаграмм, имеющихся на листе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="279cf-p108">Returns collection of charts that are part of the worksheet. Read-only.</span></span>|
|<span data-ttu-id="279cf-183">names</span><span class="sxs-lookup"><span data-stu-id="279cf-183">names</span></span>|<span data-ttu-id="279cf-184">[WorkbookNamedItem](nameditem.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="279cf-184">[WorkbookNamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="279cf-p109">Возвращает коллекцию имен, связанных с листом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="279cf-p109">Returns collection of names that are associated with the worksheet. Read-only.</span></span>|
|<span data-ttu-id="279cf-187">pivotTables</span><span class="sxs-lookup"><span data-stu-id="279cf-187">pivotTables</span></span>|<span data-ttu-id="279cf-188">Коллекция [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="279cf-188">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="279cf-189">Коллекция сводных таблиц на листе.</span><span class="sxs-lookup"><span data-stu-id="279cf-189">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="279cf-190">protection</span><span class="sxs-lookup"><span data-stu-id="279cf-190">protection</span></span>|[<span data-ttu-id="279cf-191">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="279cf-191">WorkbookWorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="279cf-p110">Возвращает объект защиты листа. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="279cf-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="279cf-194">tables</span><span class="sxs-lookup"><span data-stu-id="279cf-194">tables</span></span>|<span data-ttu-id="279cf-195">[WorkbookTable](table.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="279cf-195">[WorkbookTable](table.md) collection</span></span>|<span data-ttu-id="279cf-p111">Коллекция таблиц, имеющихся на листе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="279cf-p111">Collection of tables that are part of the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="279cf-198">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="279cf-198">JSON representation</span></span>

<span data-ttu-id="279cf-199">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="279cf-199">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheet"
}-->

```json
{
  "id": "string",
  "name": "string",
  "position": 1024,
  "visibility": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
