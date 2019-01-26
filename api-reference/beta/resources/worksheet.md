---
title: Тип ресурса Worksheet
description: Лист Excel представляет собой сетку ячеек. Он может содержать данные, таблицы, диаграммы и т. д.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 6a3a5fbb222c9228b55b2dac2a38b699ed15f213
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574378"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="ad22c-104">Тип ресурса Worksheet</span><span class="sxs-lookup"><span data-stu-id="ad22c-104">Worksheet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad22c-p102">Лист Excel представляет собой сетку ячеек. Он может содержать данные, таблицы, диаграммы и т. д.</span><span class="sxs-lookup"><span data-stu-id="ad22c-p102">An Excel worksheet is a grid of cells. It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="ad22c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ad22c-107">Methods</span></span>

| <span data-ttu-id="ad22c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ad22c-108">Method</span></span>           | <span data-ttu-id="ad22c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ad22c-109">Return Type</span></span>    |<span data-ttu-id="ad22c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ad22c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ad22c-111">Получение объекта Worksheet</span><span class="sxs-lookup"><span data-stu-id="ad22c-111">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="ad22c-112">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="ad22c-112">WorkbookWorksheet</span></span>](worksheet.md) |<span data-ttu-id="ad22c-113">Чтение свойств и связей объекта листа.</span><span class="sxs-lookup"><span data-stu-id="ad22c-113">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="ad22c-114">Создание объекта Chart</span><span class="sxs-lookup"><span data-stu-id="ad22c-114">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="ad22c-115">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="ad22c-115">WorkbookChart</span></span>](chart.md)| <span data-ttu-id="ad22c-116">Создание диаграммы путем добавления в коллекцию диаграмм.</span><span class="sxs-lookup"><span data-stu-id="ad22c-116">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="ad22c-117">List names</span><span class="sxs-lookup"><span data-stu-id="ad22c-117">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="ad22c-118">[WorkbookNamedItem](workbooknameditem.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ad22c-118">[WorkbookNamedItem](workbooknameditem.md) collection</span></span>| <span data-ttu-id="ad22c-119">Получение коллекции именованных элементов, связанной с листом.</span><span class="sxs-lookup"><span data-stu-id="ad22c-119">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="ad22c-120">List charts</span><span class="sxs-lookup"><span data-stu-id="ad22c-120">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="ad22c-121">[WorkbookChart](chart.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ad22c-121">[WorkbookChart](chart.md) collection</span></span>| <span data-ttu-id="ad22c-122">Получение коллекции объектов Chart.</span><span class="sxs-lookup"><span data-stu-id="ad22c-122">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="ad22c-123">Создание объекта Table</span><span class="sxs-lookup"><span data-stu-id="ad22c-123">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="ad22c-124">WorkbookTable</span><span class="sxs-lookup"><span data-stu-id="ad22c-124">WorkbookTable</span></span>](table.md)| <span data-ttu-id="ad22c-125">Создание таблицы путем добавления в коллекцию таблиц.</span><span class="sxs-lookup"><span data-stu-id="ad22c-125">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="ad22c-126">Список таблиц</span><span class="sxs-lookup"><span data-stu-id="ad22c-126">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="ad22c-127">[WorkbookTable](table.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ad22c-127">[WorkbookTable](table.md) collection</span></span>| <span data-ttu-id="ad22c-128">Получение коллекции объектов Table.</span><span class="sxs-lookup"><span data-stu-id="ad22c-128">Get a Table object collection.</span></span>|
|[<span data-ttu-id="ad22c-129">Update</span><span class="sxs-lookup"><span data-stu-id="ad22c-129">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="ad22c-130">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="ad22c-130">WorkbookWorksheet</span></span>](worksheet.md)   |<span data-ttu-id="ad22c-131">Обновление объекта Worksheet.</span><span class="sxs-lookup"><span data-stu-id="ad22c-131">Update Worksheet object.</span></span> |
|[<span data-ttu-id="ad22c-132">Cell</span><span class="sxs-lookup"><span data-stu-id="ad22c-132">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="ad22c-133">Range</span><span class="sxs-lookup"><span data-stu-id="ad22c-133">Range</span></span>](range.md)|<span data-ttu-id="ad22c-p103">Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.</span><span class="sxs-lookup"><span data-stu-id="ad22c-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="ad22c-136">Range</span><span class="sxs-lookup"><span data-stu-id="ad22c-136">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="ad22c-137">Range</span><span class="sxs-lookup"><span data-stu-id="ad22c-137">Range</span></span>](range.md)|<span data-ttu-id="ad22c-138">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="ad22c-138">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="ad22c-139">Usedrange</span><span class="sxs-lookup"><span data-stu-id="ad22c-139">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="ad22c-140">Range</span><span class="sxs-lookup"><span data-stu-id="ad22c-140">Range</span></span>](range.md)|<span data-ttu-id="ad22c-p104">Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.</span><span class="sxs-lookup"><span data-stu-id="ad22c-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="ad22c-143">Delete</span><span class="sxs-lookup"><span data-stu-id="ad22c-143">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="ad22c-144">Нет</span><span class="sxs-lookup"><span data-stu-id="ad22c-144">None</span></span>|<span data-ttu-id="ad22c-145">Удаляет лист из книги.</span><span class="sxs-lookup"><span data-stu-id="ad22c-145">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="ad22c-146">List</span><span class="sxs-lookup"><span data-stu-id="ad22c-146">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="ad22c-147">[WorkbookWorksheet](worksheet.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ad22c-147">[WorkbookWorksheet](worksheet.md) collection</span></span> |<span data-ttu-id="ad22c-148">Получение коллекции объектов листов.</span><span class="sxs-lookup"><span data-stu-id="ad22c-148">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="ad22c-149">Add</span><span class="sxs-lookup"><span data-stu-id="ad22c-149">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="ad22c-150">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="ad22c-150">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="ad22c-p105">Добавляет новый лист в книгу. Лист будет добавлен после существующих листов.</span><span class="sxs-lookup"><span data-stu-id="ad22c-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="ad22c-153">Получение списка pivotTables</span><span class="sxs-lookup"><span data-stu-id="ad22c-153">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="ad22c-154">Коллекция [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="ad22c-154">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="ad22c-155">Получение коллекции объектов workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="ad22c-155">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="ad22c-156">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad22c-156">Properties</span></span>
| <span data-ttu-id="ad22c-157">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad22c-157">Property</span></span>     | <span data-ttu-id="ad22c-158">Тип</span><span class="sxs-lookup"><span data-stu-id="ad22c-158">Type</span></span>   |<span data-ttu-id="ad22c-159">Описание</span><span class="sxs-lookup"><span data-stu-id="ad22c-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad22c-160">id</span><span class="sxs-lookup"><span data-stu-id="ad22c-160">id</span></span>|<span data-ttu-id="ad22c-161">string</span><span class="sxs-lookup"><span data-stu-id="ad22c-161">string</span></span>|<span data-ttu-id="ad22c-p106">Возвращает значение, однозначно идентифицирующее лист в данной книге. Значение идентификатора остается прежним, даже если переименовать или переместить лист. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad22c-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="ad22c-165">name</span><span class="sxs-lookup"><span data-stu-id="ad22c-165">name</span></span>|<span data-ttu-id="ad22c-166">строка</span><span class="sxs-lookup"><span data-stu-id="ad22c-166">string</span></span>|<span data-ttu-id="ad22c-167">Отображаемое имя листа.</span><span class="sxs-lookup"><span data-stu-id="ad22c-167">The display name of the worksheet.</span></span>|
|<span data-ttu-id="ad22c-168">position</span><span class="sxs-lookup"><span data-stu-id="ad22c-168">position</span></span>|<span data-ttu-id="ad22c-169">int</span><span class="sxs-lookup"><span data-stu-id="ad22c-169">int</span></span>|<span data-ttu-id="ad22c-170">Положение листа (начиная с нуля) в книге.</span><span class="sxs-lookup"><span data-stu-id="ad22c-170">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="ad22c-171">visibility</span><span class="sxs-lookup"><span data-stu-id="ad22c-171">visibility</span></span>|<span data-ttu-id="ad22c-172">string</span><span class="sxs-lookup"><span data-stu-id="ad22c-172">string</span></span>|<span data-ttu-id="ad22c-173">Видимость рабочего листа.</span><span class="sxs-lookup"><span data-stu-id="ad22c-173">The Visibility of the worksheet.</span></span> <span data-ttu-id="ad22c-174">Возможные значения: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="ad22c-174">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad22c-175">Связи</span><span class="sxs-lookup"><span data-stu-id="ad22c-175">Relationships</span></span>
| <span data-ttu-id="ad22c-176">Связь</span><span class="sxs-lookup"><span data-stu-id="ad22c-176">Relationship</span></span> | <span data-ttu-id="ad22c-177">Тип</span><span class="sxs-lookup"><span data-stu-id="ad22c-177">Type</span></span>   |<span data-ttu-id="ad22c-178">Описание</span><span class="sxs-lookup"><span data-stu-id="ad22c-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad22c-179">charts</span><span class="sxs-lookup"><span data-stu-id="ad22c-179">charts</span></span>|<span data-ttu-id="ad22c-180">[WorkbookChart](chart.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ad22c-180">[WorkbookChart](chart.md) collection</span></span>|<span data-ttu-id="ad22c-p108">Возвращает коллекцию диаграмм, имеющихся на листе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad22c-p108">Returns collection of charts that are part of the worksheet. Read-only.</span></span>|
|<span data-ttu-id="ad22c-183">names</span><span class="sxs-lookup"><span data-stu-id="ad22c-183">names</span></span>|<span data-ttu-id="ad22c-184">[workbookNamedItem](workbooknameditem.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ad22c-184">[workbookNamedItem](workbooknameditem.md) collection</span></span>|<span data-ttu-id="ad22c-p109">Возвращает коллекцию имен, связанных с листом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad22c-p109">Returns collection of names that are associated with the worksheet. Read-only.</span></span>|
|<span data-ttu-id="ad22c-187">pivotTables</span><span class="sxs-lookup"><span data-stu-id="ad22c-187">pivotTables</span></span>|<span data-ttu-id="ad22c-188">Коллекция [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="ad22c-188">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="ad22c-189">Коллекция сводных таблиц на листе.</span><span class="sxs-lookup"><span data-stu-id="ad22c-189">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="ad22c-190">protection</span><span class="sxs-lookup"><span data-stu-id="ad22c-190">protection</span></span>|[<span data-ttu-id="ad22c-191">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="ad22c-191">WorkbookWorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="ad22c-p110">Возвращает объект защиты листа. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad22c-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="ad22c-194">tables</span><span class="sxs-lookup"><span data-stu-id="ad22c-194">tables</span></span>|<span data-ttu-id="ad22c-195">[WorkbookTable](table.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ad22c-195">[WorkbookTable](table.md) collection</span></span>|<span data-ttu-id="ad22c-p111">Коллекция таблиц, имеющихся на листе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad22c-p111">Collection of tables that are part of the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad22c-198">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad22c-198">JSON representation</span></span>

<span data-ttu-id="ad22c-199">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad22c-199">Here is a JSON representation of the resource.</span></span>

<!-- {
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
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
