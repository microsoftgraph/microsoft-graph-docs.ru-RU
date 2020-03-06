---
title: Тип ресурса Worksheet
description: Лист Excel представляет собой сетку ячеек. Он может содержать данные, таблицы, диаграммы и т. д.
localization_priority: Priority
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d9edb4e0ad13f7caf94fd4308f606fccc14861aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533365"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="ba6a6-104">Тип ресурса Worksheet</span><span class="sxs-lookup"><span data-stu-id="ba6a6-104">Worksheet resource type</span></span>

<span data-ttu-id="ba6a6-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba6a6-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba6a6-106">Лист Excel представляет собой сетку ячеек.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-106">An Excel worksheet is a grid of cells.</span></span> <span data-ttu-id="ba6a6-107">Он может содержать данные, таблицы, диаграммы и т. д.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-107">It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="ba6a6-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ba6a6-108">Methods</span></span>

| <span data-ttu-id="ba6a6-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ba6a6-109">Method</span></span>           | <span data-ttu-id="ba6a6-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ba6a6-110">Return Type</span></span>    |<span data-ttu-id="ba6a6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ba6a6-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ba6a6-112">Получение объекта Worksheet</span><span class="sxs-lookup"><span data-stu-id="ba6a6-112">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="ba6a6-113">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="ba6a6-113">WorkbookWorksheet</span></span>](worksheet.md) |<span data-ttu-id="ba6a6-114">Чтение свойств и связей объекта листа.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-114">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="ba6a6-115">Создание объекта Chart</span><span class="sxs-lookup"><span data-stu-id="ba6a6-115">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="ba6a6-116">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="ba6a6-116">WorkbookChart</span></span>](chart.md)| <span data-ttu-id="ba6a6-117">Создание диаграммы путем добавления в коллекцию диаграмм.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-117">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="ba6a6-118">Список имен</span><span class="sxs-lookup"><span data-stu-id="ba6a6-118">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="ba6a6-119">Коллекция [WorkbookNamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="ba6a6-119">[WorkbookNamedItem](nameditem.md) collection</span></span>| <span data-ttu-id="ba6a6-120">Получение коллекции именованных элементов, связанной с листом.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-120">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="ba6a6-121">Список диаграмм</span><span class="sxs-lookup"><span data-stu-id="ba6a6-121">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="ba6a6-122">Коллекция [WorkbookChart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="ba6a6-122">[WorkbookChart](chart.md) collection</span></span>| <span data-ttu-id="ba6a6-123">Получение коллекции объектов Chart.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-123">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="ba6a6-124">Создание объекта Table</span><span class="sxs-lookup"><span data-stu-id="ba6a6-124">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="ba6a6-125">WorkbookTable</span><span class="sxs-lookup"><span data-stu-id="ba6a6-125">WorkbookTable</span></span>](table.md)| <span data-ttu-id="ba6a6-126">Создание таблицы путем добавления в коллекцию таблиц.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-126">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="ba6a6-127">Список таблиц</span><span class="sxs-lookup"><span data-stu-id="ba6a6-127">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="ba6a6-128">Коллекция [WorkbookTable](table.md)</span><span class="sxs-lookup"><span data-stu-id="ba6a6-128">[WorkbookTable](table.md) collection</span></span>| <span data-ttu-id="ba6a6-129">Получение коллекции объектов Table.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-129">Get a Table object collection.</span></span>|
|[<span data-ttu-id="ba6a6-130">Update</span><span class="sxs-lookup"><span data-stu-id="ba6a6-130">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="ba6a6-131">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="ba6a6-131">WorkbookWorksheet</span></span>](worksheet.md)   |<span data-ttu-id="ba6a6-132">Обновление объекта Worksheet.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-132">Update Worksheet object.</span></span> |
|[<span data-ttu-id="ba6a6-133">Cell</span><span class="sxs-lookup"><span data-stu-id="ba6a6-133">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="ba6a6-134">Range</span><span class="sxs-lookup"><span data-stu-id="ba6a6-134">Range</span></span>](range.md)|<span data-ttu-id="ba6a6-p103">Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="ba6a6-137">Range</span><span class="sxs-lookup"><span data-stu-id="ba6a6-137">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="ba6a6-138">Range</span><span class="sxs-lookup"><span data-stu-id="ba6a6-138">Range</span></span>](range.md)|<span data-ttu-id="ba6a6-139">Возвращает объект диапазона по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-139">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="ba6a6-140">Usedrange</span><span class="sxs-lookup"><span data-stu-id="ba6a6-140">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="ba6a6-141">Range</span><span class="sxs-lookup"><span data-stu-id="ba6a6-141">Range</span></span>](range.md)|<span data-ttu-id="ba6a6-p104">Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="ba6a6-144">Delete</span><span class="sxs-lookup"><span data-stu-id="ba6a6-144">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="ba6a6-145">Нет</span><span class="sxs-lookup"><span data-stu-id="ba6a6-145">None</span></span>|<span data-ttu-id="ba6a6-146">Удаляет лист из книги.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-146">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="ba6a6-147">Список</span><span class="sxs-lookup"><span data-stu-id="ba6a6-147">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="ba6a6-148">Коллекция [WorkbookWorksheet](worksheet.md)</span><span class="sxs-lookup"><span data-stu-id="ba6a6-148">[WorkbookWorksheet](worksheet.md) collection</span></span> |<span data-ttu-id="ba6a6-149">Получение коллекции объектов листов.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-149">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="ba6a6-150">Add</span><span class="sxs-lookup"><span data-stu-id="ba6a6-150">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="ba6a6-151">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="ba6a6-151">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="ba6a6-p105">Добавляет новый лист в книгу. Лист будет добавлен после существующих листов.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="ba6a6-154">Список pivotTables</span><span class="sxs-lookup"><span data-stu-id="ba6a6-154">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="ba6a6-155">Коллекция [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="ba6a6-155">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="ba6a6-156">Получение коллекции объектов workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-156">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="ba6a6-157">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba6a6-157">Properties</span></span>
| <span data-ttu-id="ba6a6-158">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba6a6-158">Property</span></span>     | <span data-ttu-id="ba6a6-159">Тип</span><span class="sxs-lookup"><span data-stu-id="ba6a6-159">Type</span></span>   |<span data-ttu-id="ba6a6-160">Описание</span><span class="sxs-lookup"><span data-stu-id="ba6a6-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba6a6-161">id</span><span class="sxs-lookup"><span data-stu-id="ba6a6-161">id</span></span>|<span data-ttu-id="ba6a6-162">string</span><span class="sxs-lookup"><span data-stu-id="ba6a6-162">string</span></span>|<span data-ttu-id="ba6a6-p106">Возвращает значение, однозначно идентифицирующее лист в данной книге. Значение идентификатора остается прежним, даже если переименовать или переместить лист. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="ba6a6-166">name</span><span class="sxs-lookup"><span data-stu-id="ba6a6-166">name</span></span>|<span data-ttu-id="ba6a6-167">string</span><span class="sxs-lookup"><span data-stu-id="ba6a6-167">string</span></span>|<span data-ttu-id="ba6a6-168">Отображаемое имя листа.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-168">The display name of the worksheet.</span></span>|
|<span data-ttu-id="ba6a6-169">position</span><span class="sxs-lookup"><span data-stu-id="ba6a6-169">position</span></span>|<span data-ttu-id="ba6a6-170">int</span><span class="sxs-lookup"><span data-stu-id="ba6a6-170">int</span></span>|<span data-ttu-id="ba6a6-171">Положение листа (начиная с нуля) в книге.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-171">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="ba6a6-172">visibility</span><span class="sxs-lookup"><span data-stu-id="ba6a6-172">visibility</span></span>|<span data-ttu-id="ba6a6-173">string</span><span class="sxs-lookup"><span data-stu-id="ba6a6-173">string</span></span>|<span data-ttu-id="ba6a6-174">Видимость листа.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-174">The Visibility of the worksheet.</span></span> <span data-ttu-id="ba6a6-175">Допустимые значения: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-175">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba6a6-176">Отношения</span><span class="sxs-lookup"><span data-stu-id="ba6a6-176">Relationships</span></span>
| <span data-ttu-id="ba6a6-177">Связь</span><span class="sxs-lookup"><span data-stu-id="ba6a6-177">Relationship</span></span> | <span data-ttu-id="ba6a6-178">Тип</span><span class="sxs-lookup"><span data-stu-id="ba6a6-178">Type</span></span>   |<span data-ttu-id="ba6a6-179">Описание</span><span class="sxs-lookup"><span data-stu-id="ba6a6-179">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba6a6-180">charts</span><span class="sxs-lookup"><span data-stu-id="ba6a6-180">charts</span></span>|<span data-ttu-id="ba6a6-181">Коллекция [WorkbookChart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="ba6a6-181">[WorkbookChart](chart.md) collection</span></span>|<span data-ttu-id="ba6a6-182">Возвращает коллекцию диаграмм, имеющихся на листе.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-182">Returns collection of charts that are part of the worksheet.</span></span> <span data-ttu-id="ba6a6-183">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-183">Read-only.</span></span>|
|<span data-ttu-id="ba6a6-184">names</span><span class="sxs-lookup"><span data-stu-id="ba6a6-184">names</span></span>|<span data-ttu-id="ba6a6-185">Коллекция [WorkbookNamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="ba6a6-185">[WorkbookNamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="ba6a6-186">Возвращает коллекцию имен, связанных с листом.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-186">Returns collection of names that are associated with the worksheet.</span></span> <span data-ttu-id="ba6a6-187">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-187">Read-only.</span></span>|
|<span data-ttu-id="ba6a6-188">pivotTables</span><span class="sxs-lookup"><span data-stu-id="ba6a6-188">pivotTables</span></span>|<span data-ttu-id="ba6a6-189">Коллекция [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="ba6a6-189">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="ba6a6-190">Коллекция сводных таблиц на листе.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-190">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="ba6a6-191">protection</span><span class="sxs-lookup"><span data-stu-id="ba6a6-191">protection</span></span>|[<span data-ttu-id="ba6a6-192">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="ba6a6-192">WorkbookWorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="ba6a6-p110">Возвращает объект защиты листа. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="ba6a6-195">tables</span><span class="sxs-lookup"><span data-stu-id="ba6a6-195">tables</span></span>|<span data-ttu-id="ba6a6-196">Коллекция [WorkbookTable](table.md)</span><span class="sxs-lookup"><span data-stu-id="ba6a6-196">[WorkbookTable](table.md) collection</span></span>|<span data-ttu-id="ba6a6-197">Коллекция таблиц, имеющихся на листе.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-197">Collection of tables that are part of the worksheet.</span></span> <span data-ttu-id="ba6a6-198">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-198">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba6a6-199">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba6a6-199">JSON representation</span></span>

<span data-ttu-id="ba6a6-200">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba6a6-200">Here is a JSON representation of the resource.</span></span>

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
