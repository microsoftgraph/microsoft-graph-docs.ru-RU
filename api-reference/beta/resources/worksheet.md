---
title: Тип ресурса Worksheet
description: Лист Excel представляет собой сетку ячеек. Он может содержать данные, таблицы, диаграммы и т. д.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: d04ebafda64f9a081096fbf0fd94461b9765a6db
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926528"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="adfc9-104">Тип ресурса Worksheet</span><span class="sxs-lookup"><span data-stu-id="adfc9-104">Worksheet resource type</span></span>

> <span data-ttu-id="adfc9-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="adfc9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adfc9-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adfc9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="adfc9-p103">Лист Excel представляет собой сетку ячеек. Он может содержать данные, таблицы, диаграммы и т. д.</span><span class="sxs-lookup"><span data-stu-id="adfc9-p103">An Excel worksheet is a grid of cells. It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="adfc9-109">Методы</span><span class="sxs-lookup"><span data-stu-id="adfc9-109">Methods</span></span>

| <span data-ttu-id="adfc9-110">Метод</span><span class="sxs-lookup"><span data-stu-id="adfc9-110">Method</span></span>           | <span data-ttu-id="adfc9-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="adfc9-111">Return Type</span></span>    |<span data-ttu-id="adfc9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="adfc9-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="adfc9-113">Получение объекта Worksheet</span><span class="sxs-lookup"><span data-stu-id="adfc9-113">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="adfc9-114">Worksheet</span><span class="sxs-lookup"><span data-stu-id="adfc9-114">Worksheet</span></span>](worksheet.md) |<span data-ttu-id="adfc9-115">Чтение свойств и связей объекта листа.</span><span class="sxs-lookup"><span data-stu-id="adfc9-115">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="adfc9-116">Создание объекта Chart</span><span class="sxs-lookup"><span data-stu-id="adfc9-116">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="adfc9-117">Chart</span><span class="sxs-lookup"><span data-stu-id="adfc9-117">Chart</span></span>](chart.md)| <span data-ttu-id="adfc9-118">Создание диаграммы путем добавления в коллекцию диаграмм.</span><span class="sxs-lookup"><span data-stu-id="adfc9-118">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="adfc9-119">List names</span><span class="sxs-lookup"><span data-stu-id="adfc9-119">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="adfc9-120">Коллекция объектов [NamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="adfc9-120">[NamedItem](nameditem.md) collection</span></span>| <span data-ttu-id="adfc9-121">Получение коллекции именованных элементов, связанной с листом.</span><span class="sxs-lookup"><span data-stu-id="adfc9-121">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="adfc9-122">List charts</span><span class="sxs-lookup"><span data-stu-id="adfc9-122">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="adfc9-123">Коллекция объектов [Chart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="adfc9-123">[Chart](chart.md) collection</span></span>| <span data-ttu-id="adfc9-124">Получение коллекции объектов Chart.</span><span class="sxs-lookup"><span data-stu-id="adfc9-124">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="adfc9-125">Создание объекта Table</span><span class="sxs-lookup"><span data-stu-id="adfc9-125">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="adfc9-126">Table</span><span class="sxs-lookup"><span data-stu-id="adfc9-126">Table</span></span>](table.md)| <span data-ttu-id="adfc9-127">Создание таблицы путем добавления в коллекцию таблиц.</span><span class="sxs-lookup"><span data-stu-id="adfc9-127">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="adfc9-128">Список таблиц</span><span class="sxs-lookup"><span data-stu-id="adfc9-128">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="adfc9-129">Коллекция объектов [Table](table.md)</span><span class="sxs-lookup"><span data-stu-id="adfc9-129">[Table](table.md) collection</span></span>| <span data-ttu-id="adfc9-130">Получение коллекции объектов Table.</span><span class="sxs-lookup"><span data-stu-id="adfc9-130">Get a Table object collection.</span></span>|
|<span data-ttu-id="adfc9-131">[обновление](../api/worksheet-update.md).</span><span class="sxs-lookup"><span data-stu-id="adfc9-131">[Update](../api/worksheet-update.md)</span></span> | [<span data-ttu-id="adfc9-132">Worksheet</span><span class="sxs-lookup"><span data-stu-id="adfc9-132">Worksheet</span></span>](worksheet.md)   |<span data-ttu-id="adfc9-133">Обновление объекта Worksheet.</span><span class="sxs-lookup"><span data-stu-id="adfc9-133">Update Worksheet object.</span></span> |
|[<span data-ttu-id="adfc9-134">Cell</span><span class="sxs-lookup"><span data-stu-id="adfc9-134">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="adfc9-135">Range</span><span class="sxs-lookup"><span data-stu-id="adfc9-135">Range</span></span>](range.md)|<span data-ttu-id="adfc9-p104">Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.</span><span class="sxs-lookup"><span data-stu-id="adfc9-p104">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="adfc9-138">Range</span><span class="sxs-lookup"><span data-stu-id="adfc9-138">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="adfc9-139">Range</span><span class="sxs-lookup"><span data-stu-id="adfc9-139">Range</span></span>](range.md)|<span data-ttu-id="adfc9-140">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="adfc9-140">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="adfc9-141">Usedrange</span><span class="sxs-lookup"><span data-stu-id="adfc9-141">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="adfc9-142">Range</span><span class="sxs-lookup"><span data-stu-id="adfc9-142">Range</span></span>](range.md)|<span data-ttu-id="adfc9-p105">Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.</span><span class="sxs-lookup"><span data-stu-id="adfc9-p105">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="adfc9-145">Delete</span><span class="sxs-lookup"><span data-stu-id="adfc9-145">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="adfc9-146">Нет</span><span class="sxs-lookup"><span data-stu-id="adfc9-146">None</span></span>|<span data-ttu-id="adfc9-147">Удаляет лист из книги.</span><span class="sxs-lookup"><span data-stu-id="adfc9-147">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="adfc9-148">List</span><span class="sxs-lookup"><span data-stu-id="adfc9-148">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="adfc9-149">Коллекция объектов [Worksheet](worksheet.md)</span><span class="sxs-lookup"><span data-stu-id="adfc9-149">[Worksheet](worksheet.md) collection</span></span> |<span data-ttu-id="adfc9-150">Получение коллекции объектов листов.</span><span class="sxs-lookup"><span data-stu-id="adfc9-150">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="adfc9-151">Add</span><span class="sxs-lookup"><span data-stu-id="adfc9-151">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="adfc9-152">Worksheet</span><span class="sxs-lookup"><span data-stu-id="adfc9-152">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="adfc9-p106">Добавляет новый лист в книгу. Лист будет добавлен после существующих листов.</span><span class="sxs-lookup"><span data-stu-id="adfc9-p106">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="adfc9-155">Получение списка pivotTables</span><span class="sxs-lookup"><span data-stu-id="adfc9-155">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="adfc9-156">Коллекция [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="adfc9-156">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="adfc9-157">Получение коллекции объектов workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="adfc9-157">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="adfc9-158">Свойства</span><span class="sxs-lookup"><span data-stu-id="adfc9-158">Properties</span></span>
| <span data-ttu-id="adfc9-159">Свойство</span><span class="sxs-lookup"><span data-stu-id="adfc9-159">Property</span></span>     | <span data-ttu-id="adfc9-160">Тип</span><span class="sxs-lookup"><span data-stu-id="adfc9-160">Type</span></span>   |<span data-ttu-id="adfc9-161">Описание</span><span class="sxs-lookup"><span data-stu-id="adfc9-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adfc9-162">id</span><span class="sxs-lookup"><span data-stu-id="adfc9-162">id</span></span>|<span data-ttu-id="adfc9-163">строка</span><span class="sxs-lookup"><span data-stu-id="adfc9-163">string</span></span>|<span data-ttu-id="adfc9-p107">Возвращает значение, однозначно идентифицирующее лист в данной книге. Значение идентификатора остается прежним, даже если переименовать или переместить лист. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="adfc9-p107">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="adfc9-167">name</span><span class="sxs-lookup"><span data-stu-id="adfc9-167">name</span></span>|<span data-ttu-id="adfc9-168">строка</span><span class="sxs-lookup"><span data-stu-id="adfc9-168">string</span></span>|<span data-ttu-id="adfc9-169">Отображаемое имя листа.</span><span class="sxs-lookup"><span data-stu-id="adfc9-169">The display name of the worksheet.</span></span>|
|<span data-ttu-id="adfc9-170">position</span><span class="sxs-lookup"><span data-stu-id="adfc9-170">position</span></span>|<span data-ttu-id="adfc9-171">int</span><span class="sxs-lookup"><span data-stu-id="adfc9-171">int</span></span>|<span data-ttu-id="adfc9-172">Положение листа (начиная с нуля) в книге.</span><span class="sxs-lookup"><span data-stu-id="adfc9-172">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="adfc9-173">visibility</span><span class="sxs-lookup"><span data-stu-id="adfc9-173">visibility</span></span>|<span data-ttu-id="adfc9-174">string</span><span class="sxs-lookup"><span data-stu-id="adfc9-174">string</span></span>|<span data-ttu-id="adfc9-p108">Видимость листа. Возможные значения: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="adfc9-p108">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="adfc9-177">Связи</span><span class="sxs-lookup"><span data-stu-id="adfc9-177">Relationships</span></span>
| <span data-ttu-id="adfc9-178">Связь</span><span class="sxs-lookup"><span data-stu-id="adfc9-178">Relationship</span></span> | <span data-ttu-id="adfc9-179">Тип</span><span class="sxs-lookup"><span data-stu-id="adfc9-179">Type</span></span>   |<span data-ttu-id="adfc9-180">Описание</span><span class="sxs-lookup"><span data-stu-id="adfc9-180">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adfc9-181">charts</span><span class="sxs-lookup"><span data-stu-id="adfc9-181">charts</span></span>|<span data-ttu-id="adfc9-182">Коллекция объектов [Chart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="adfc9-182">[Chart](chart.md) collection</span></span>|<span data-ttu-id="adfc9-p109">Возвращает коллекцию диаграмм, имеющихся на листе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="adfc9-p109">Returns collection of charts that are part of the worksheet. Read-only.</span></span>|
|<span data-ttu-id="adfc9-185">names</span><span class="sxs-lookup"><span data-stu-id="adfc9-185">names</span></span>|<span data-ttu-id="adfc9-186">Коллекция объектов [NamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="adfc9-186">[NamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="adfc9-p110">Возвращает коллекцию имен, связанных с листом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="adfc9-p110">Returns collection of names that are associated with the worksheet. Read-only.</span></span>|
|<span data-ttu-id="adfc9-189">pivotTables</span><span class="sxs-lookup"><span data-stu-id="adfc9-189">pivotTables</span></span>|<span data-ttu-id="adfc9-190">Коллекция [workbookPivotTable](workbookpivottable.md)</span><span class="sxs-lookup"><span data-stu-id="adfc9-190">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="adfc9-191">Коллекция сводных таблиц на листе.</span><span class="sxs-lookup"><span data-stu-id="adfc9-191">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="adfc9-192">protection</span><span class="sxs-lookup"><span data-stu-id="adfc9-192">protection</span></span>|[<span data-ttu-id="adfc9-193">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="adfc9-193">WorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="adfc9-p111">Возвращает объект защиты листа. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="adfc9-p111">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="adfc9-196">tables</span><span class="sxs-lookup"><span data-stu-id="adfc9-196">tables</span></span>|<span data-ttu-id="adfc9-197">Коллекция объектов [Table](table.md)</span><span class="sxs-lookup"><span data-stu-id="adfc9-197">[Table](table.md) collection</span></span>|<span data-ttu-id="adfc9-p112">Коллекция таблиц, имеющихся на листе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="adfc9-p112">Collection of tables that are part of the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="adfc9-200">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="adfc9-200">JSON representation</span></span>

<span data-ttu-id="adfc9-201">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adfc9-201">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
