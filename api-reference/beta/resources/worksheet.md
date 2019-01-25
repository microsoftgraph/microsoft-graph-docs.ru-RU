---
title: Тип ресурса Worksheet
description: Лист Excel представляет собой сетку ячеек. Он может содержать данные, таблицы, диаграммы и т. д.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: beffb9747045d0d3792d994237710e886ff0b3d8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509149"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="752df-104">Тип ресурса Worksheet</span><span class="sxs-lookup"><span data-stu-id="752df-104">Worksheet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="752df-p102">Лист Excel представляет собой сетку ячеек. Он может содержать данные, таблицы, диаграммы и т. д.</span><span class="sxs-lookup"><span data-stu-id="752df-p102">An Excel worksheet is a grid of cells. It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="752df-107">Методы</span><span class="sxs-lookup"><span data-stu-id="752df-107">Methods</span></span>

| <span data-ttu-id="752df-108">Метод</span><span class="sxs-lookup"><span data-stu-id="752df-108">Method</span></span>           | <span data-ttu-id="752df-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="752df-109">Return Type</span></span>    |<span data-ttu-id="752df-110">Описание</span><span class="sxs-lookup"><span data-stu-id="752df-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="752df-111">Получение объекта Worksheet</span><span class="sxs-lookup"><span data-stu-id="752df-111">[Get Worksheet](../api/worksheet-get.md)</span></span> | [<span data-ttu-id="752df-112">Worksheet</span><span class="sxs-lookup"><span data-stu-id="752df-112">Worksheet</span></span>](worksheet.md) |<span data-ttu-id="752df-113">Чтение свойств и связей объекта листа.</span><span class="sxs-lookup"><span data-stu-id="752df-113">Read properties and relationships of worksheet object.</span></span>|
|<span data-ttu-id="752df-114">Создание объекта Chart</span><span class="sxs-lookup"><span data-stu-id="752df-114">[Create Chart](../api/worksheet-post-charts.md)</span></span> |[<span data-ttu-id="752df-115">Chart</span><span class="sxs-lookup"><span data-stu-id="752df-115">Chart</span></span>](chart.md)| <span data-ttu-id="752df-116">Создание диаграммы путем добавления в коллекцию диаграмм.</span><span class="sxs-lookup"><span data-stu-id="752df-116">Create a new Chart by posting to the charts collection.</span></span>|
|<span data-ttu-id="752df-117">List names</span><span class="sxs-lookup"><span data-stu-id="752df-117">[List names](../api/worksheet-list-names.md)</span></span> |<span data-ttu-id="752df-118">Коллекция объектов [NamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="752df-118">[NamedItem](nameditem.md) collection</span></span>| <span data-ttu-id="752df-119">Получение коллекции именованных элементов, связанной с листом.</span><span class="sxs-lookup"><span data-stu-id="752df-119">Get named item collection associated with the worksheet.</span></span>|
|<span data-ttu-id="752df-120">List charts</span><span class="sxs-lookup"><span data-stu-id="752df-120">[List charts](../api/worksheet-list-charts.md)</span></span> |<span data-ttu-id="752df-121">Коллекция объектов Chart</span><span class="sxs-lookup"><span data-stu-id="752df-121">[Chart](chart.md) collection</span></span>| <span data-ttu-id="752df-122">Получение коллекции объектов Chart.</span><span class="sxs-lookup"><span data-stu-id="752df-122">Get a Chart object collection.</span></span>|
|<span data-ttu-id="752df-123">Создание объекта Table</span><span class="sxs-lookup"><span data-stu-id="752df-123">[Create Table](../api/worksheet-post-tables.md)</span></span> |[<span data-ttu-id="752df-124">Table</span><span class="sxs-lookup"><span data-stu-id="752df-124">Table</span></span>](table.md)| <span data-ttu-id="752df-125">Создание таблицы путем добавления в коллекцию таблиц.</span><span class="sxs-lookup"><span data-stu-id="752df-125">Create a new Table by posting to the tables collection.</span></span>|
|<span data-ttu-id="752df-126">Список таблиц</span><span class="sxs-lookup"><span data-stu-id="752df-126">[List tables](../api/worksheet-list-tables.md)</span></span> |<span data-ttu-id="752df-127">Коллекция объектов [Table](table.md)</span><span class="sxs-lookup"><span data-stu-id="752df-127">[Table](table.md) collection</span></span>| <span data-ttu-id="752df-128">Получение коллекции объектов Table.</span><span class="sxs-lookup"><span data-stu-id="752df-128">Get a Table object collection.</span></span>|
|[<span data-ttu-id="752df-129">Update</span><span class="sxs-lookup"><span data-stu-id="752df-129">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="752df-130">Worksheet</span><span class="sxs-lookup"><span data-stu-id="752df-130">Worksheet</span></span>](worksheet.md)   |<span data-ttu-id="752df-131">Обновление объекта Worksheet.</span><span class="sxs-lookup"><span data-stu-id="752df-131">Update Worksheet object.</span></span> |
|[<span data-ttu-id="752df-132">Cell</span><span class="sxs-lookup"><span data-stu-id="752df-132">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="752df-133">Range</span><span class="sxs-lookup"><span data-stu-id="752df-133">Range</span></span>](range.md)|<span data-ttu-id="752df-p103">Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.</span><span class="sxs-lookup"><span data-stu-id="752df-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="752df-136">Range</span><span class="sxs-lookup"><span data-stu-id="752df-136">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="752df-137">Range</span><span class="sxs-lookup"><span data-stu-id="752df-137">Range</span></span>](range.md)|<span data-ttu-id="752df-138">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="752df-138">Gets the range object specified by the address or name.</span></span>|
|<span data-ttu-id="752df-139">Usedrange</span><span class="sxs-lookup"><span data-stu-id="752df-139">[Usedrange](../api/worksheet-usedrange.md)</span></span>|[<span data-ttu-id="752df-140">Range</span><span class="sxs-lookup"><span data-stu-id="752df-140">Range</span></span>](range.md)|<span data-ttu-id="752df-p104">Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.</span><span class="sxs-lookup"><span data-stu-id="752df-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="752df-143">Delete</span><span class="sxs-lookup"><span data-stu-id="752df-143">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="752df-144">Нет</span><span class="sxs-lookup"><span data-stu-id="752df-144">None</span></span>|<span data-ttu-id="752df-145">Удаляет лист из книги.</span><span class="sxs-lookup"><span data-stu-id="752df-145">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="752df-146">List</span><span class="sxs-lookup"><span data-stu-id="752df-146">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="752df-147">Коллекция объектов [Worksheet](worksheet.md)</span><span class="sxs-lookup"><span data-stu-id="752df-147">[Worksheet](worksheet.md) collection</span></span> |<span data-ttu-id="752df-148">Получение коллекции объектов листов.</span><span class="sxs-lookup"><span data-stu-id="752df-148">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="752df-149">Add</span><span class="sxs-lookup"><span data-stu-id="752df-149">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="752df-150">Worksheet</span><span class="sxs-lookup"><span data-stu-id="752df-150">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="752df-p105">Добавляет новый лист в книгу. Лист будет добавлен после существующих листов.</span><span class="sxs-lookup"><span data-stu-id="752df-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|<span data-ttu-id="752df-153">Получение списка pivotTables</span><span class="sxs-lookup"><span data-stu-id="752df-153">[List pivotTables](../api/workbookworksheet-list-pivottables.md)</span></span> |<span data-ttu-id="752df-154">Коллекция workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="752df-154">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="752df-155">Получение коллекции объектов workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="752df-155">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="752df-156">Свойства</span><span class="sxs-lookup"><span data-stu-id="752df-156">Properties</span></span>
| <span data-ttu-id="752df-157">Свойство</span><span class="sxs-lookup"><span data-stu-id="752df-157">Property</span></span>     | <span data-ttu-id="752df-158">Тип</span><span class="sxs-lookup"><span data-stu-id="752df-158">Type</span></span>   |<span data-ttu-id="752df-159">Описание</span><span class="sxs-lookup"><span data-stu-id="752df-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="752df-160">id</span><span class="sxs-lookup"><span data-stu-id="752df-160">id</span></span>|<span data-ttu-id="752df-161">string</span><span class="sxs-lookup"><span data-stu-id="752df-161">string</span></span>|<span data-ttu-id="752df-p106">Возвращает значение, однозначно идентифицирующее лист в данной книге. Значение идентификатора остается прежним, даже если переименовать или переместить лист. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="752df-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="752df-165">name</span><span class="sxs-lookup"><span data-stu-id="752df-165">name</span></span>|<span data-ttu-id="752df-166">строка</span><span class="sxs-lookup"><span data-stu-id="752df-166">string</span></span>|<span data-ttu-id="752df-167">Отображаемое имя листа.</span><span class="sxs-lookup"><span data-stu-id="752df-167">The display name of the worksheet.</span></span>|
|<span data-ttu-id="752df-168">position</span><span class="sxs-lookup"><span data-stu-id="752df-168">position</span></span>|<span data-ttu-id="752df-169">int</span><span class="sxs-lookup"><span data-stu-id="752df-169">int</span></span>|<span data-ttu-id="752df-170">Положение листа (начиная с нуля) в книге.</span><span class="sxs-lookup"><span data-stu-id="752df-170">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="752df-171">visibility</span><span class="sxs-lookup"><span data-stu-id="752df-171">visibility</span></span>|<span data-ttu-id="752df-172">string</span><span class="sxs-lookup"><span data-stu-id="752df-172">string</span></span>|<span data-ttu-id="752df-p107">Видимость листа. Возможные значения: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="752df-p107">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="752df-175">Отношения</span><span class="sxs-lookup"><span data-stu-id="752df-175">Relationships</span></span>
| <span data-ttu-id="752df-176">Связь</span><span class="sxs-lookup"><span data-stu-id="752df-176">Relationship</span></span> | <span data-ttu-id="752df-177">Тип</span><span class="sxs-lookup"><span data-stu-id="752df-177">Type</span></span>   |<span data-ttu-id="752df-178">Описание</span><span class="sxs-lookup"><span data-stu-id="752df-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="752df-179">charts</span><span class="sxs-lookup"><span data-stu-id="752df-179">charts</span></span>|<span data-ttu-id="752df-180">Коллекция объектов [Chart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="752df-180">[Chart](chart.md) collection</span></span>|<span data-ttu-id="752df-p108">Возвращает коллекцию диаграмм, имеющихся на листе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="752df-p108">Returns collection of charts that are part of the worksheet. Read-only.</span></span>|
|<span data-ttu-id="752df-183">names</span><span class="sxs-lookup"><span data-stu-id="752df-183">names</span></span>|<span data-ttu-id="752df-184">Коллекция объектов [NamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="752df-184">[NamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="752df-p109">Возвращает коллекцию имен, связанных с листом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="752df-p109">Returns collection of names that are associated with the worksheet. Read-only.</span></span>|
|<span data-ttu-id="752df-187">pivotTables</span><span class="sxs-lookup"><span data-stu-id="752df-187">pivotTables</span></span>|<span data-ttu-id="752df-188">Коллекция [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="752df-188">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="752df-189">Коллекция сводных таблиц на листе.</span><span class="sxs-lookup"><span data-stu-id="752df-189">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="752df-190">protection</span><span class="sxs-lookup"><span data-stu-id="752df-190">protection</span></span>|[<span data-ttu-id="752df-191">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="752df-191">WorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="752df-p110">Возвращает объект защиты листа. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="752df-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="752df-194">tables</span><span class="sxs-lookup"><span data-stu-id="752df-194">tables</span></span>|<span data-ttu-id="752df-195">Коллекция объектов [Table](table.md)</span><span class="sxs-lookup"><span data-stu-id="752df-195">[Table](table.md) collection</span></span>|<span data-ttu-id="752df-p111">Коллекция таблиц, имеющихся на листе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="752df-p111">Collection of tables that are part of the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="752df-198">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="752df-198">JSON representation</span></span>

<span data-ttu-id="752df-199">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="752df-199">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheet"
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
