---
title: Тип ресурса RangeFormat
description: Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3e1b79c80c20197cc14a5097efdf9eb0513b43e4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034890"
---
# <a name="rangeformat-resource-type"></a><span data-ttu-id="35ed5-103">Тип ресурса RangeFormat</span><span class="sxs-lookup"><span data-stu-id="35ed5-103">RangeFormat resource type</span></span>

<span data-ttu-id="35ed5-104">Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.</span><span class="sxs-lookup"><span data-stu-id="35ed5-104">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="35ed5-105">Методы</span><span class="sxs-lookup"><span data-stu-id="35ed5-105">Methods</span></span>

| <span data-ttu-id="35ed5-106">Метод</span><span class="sxs-lookup"><span data-stu-id="35ed5-106">Method</span></span>           | <span data-ttu-id="35ed5-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="35ed5-107">Return Type</span></span>    |<span data-ttu-id="35ed5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="35ed5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35ed5-109">Получение объекта RangeFormat</span><span class="sxs-lookup"><span data-stu-id="35ed5-109">Get RangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="35ed5-110">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="35ed5-110">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="35ed5-111">Чтение свойств и связей объекта rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="35ed5-111">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="35ed5-112">Создание объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="35ed5-112">Create RangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="35ed5-113">Воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="35ed5-113">WorkbookRangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="35ed5-114">Создание объекта RangeBorder путем добавления в коллекцию границ.</span><span class="sxs-lookup"><span data-stu-id="35ed5-114">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="35ed5-115">Список границ</span><span class="sxs-lookup"><span data-stu-id="35ed5-115">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="35ed5-116">Коллекция [воркбукранжебордер](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="35ed5-116">[WorkbookRangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="35ed5-117">Получение коллекции объектов RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="35ed5-117">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="35ed5-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="35ed5-118">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="35ed5-119">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="35ed5-119">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="35ed5-120">Обновление объекта RangeFormat.</span><span class="sxs-lookup"><span data-stu-id="35ed5-120">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="35ed5-121">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="35ed5-121">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="35ed5-122">Нет</span><span class="sxs-lookup"><span data-stu-id="35ed5-122">None</span></span>|<span data-ttu-id="35ed5-123">Изменяет ширину столбцов текущего диапазона на оптимальную с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="35ed5-123">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="35ed5-124">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="35ed5-124">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="35ed5-125">Нет</span><span class="sxs-lookup"><span data-stu-id="35ed5-125">None</span></span>|<span data-ttu-id="35ed5-126">Изменяет высоту строк текущего диапазона на оптимальную с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="35ed5-126">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="35ed5-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="35ed5-127">Properties</span></span>
| <span data-ttu-id="35ed5-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="35ed5-128">Property</span></span>     | <span data-ttu-id="35ed5-129">Тип</span><span class="sxs-lookup"><span data-stu-id="35ed5-129">Type</span></span>   |<span data-ttu-id="35ed5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="35ed5-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35ed5-131">columnWidth</span><span class="sxs-lookup"><span data-stu-id="35ed5-131">columnWidth</span></span>|<span data-ttu-id="35ed5-132">double</span><span class="sxs-lookup"><span data-stu-id="35ed5-132">double</span></span>|<span data-ttu-id="35ed5-p101">Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="35ed5-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="35ed5-135">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="35ed5-135">horizontalAlignment</span></span>|<span data-ttu-id="35ed5-136">string</span><span class="sxs-lookup"><span data-stu-id="35ed5-136">string</span></span>|<span data-ttu-id="35ed5-137">Представляет выравнивание по горизонтали для указанного объекта.</span><span class="sxs-lookup"><span data-stu-id="35ed5-137">Represents the horizontal alignment for the specified object.</span></span> <span data-ttu-id="35ed5-138">Возможные `General`значения:, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`,. `Distributed`</span><span class="sxs-lookup"><span data-stu-id="35ed5-138">The possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="35ed5-139">rowHeight</span><span class="sxs-lookup"><span data-stu-id="35ed5-139">rowHeight</span></span>|<span data-ttu-id="35ed5-140">double</span><span class="sxs-lookup"><span data-stu-id="35ed5-140">double</span></span>|<span data-ttu-id="35ed5-p103">Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="35ed5-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="35ed5-143">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="35ed5-143">verticalAlignment</span></span>|<span data-ttu-id="35ed5-144">string</span><span class="sxs-lookup"><span data-stu-id="35ed5-144">string</span></span>|<span data-ttu-id="35ed5-145">Представляет выравнивание по вертикали для указанного объекта.</span><span class="sxs-lookup"><span data-stu-id="35ed5-145">Represents the vertical alignment for the specified object.</span></span> <span data-ttu-id="35ed5-146">Допустимые значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="35ed5-146">The possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="35ed5-147">wrapText</span><span class="sxs-lookup"><span data-stu-id="35ed5-147">wrapText</span></span>|<span data-ttu-id="35ed5-148">boolean</span><span class="sxs-lookup"><span data-stu-id="35ed5-148">boolean</span></span>|<span data-ttu-id="35ed5-p105">Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.</span><span class="sxs-lookup"><span data-stu-id="35ed5-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="35ed5-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="35ed5-151">Relationships</span></span>
| <span data-ttu-id="35ed5-152">Отношение</span><span class="sxs-lookup"><span data-stu-id="35ed5-152">Relationship</span></span> | <span data-ttu-id="35ed5-153">Тип</span><span class="sxs-lookup"><span data-stu-id="35ed5-153">Type</span></span>   |<span data-ttu-id="35ed5-154">Описание</span><span class="sxs-lookup"><span data-stu-id="35ed5-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35ed5-155">borders</span><span class="sxs-lookup"><span data-stu-id="35ed5-155">borders</span></span>|<span data-ttu-id="35ed5-156">Коллекция [воркбукранжебордер](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="35ed5-156">[WorkbookRangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="35ed5-157">Коллекция объектов границы, которые применяются к общему выделенному диапазону. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35ed5-157">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="35ed5-158">fill</span><span class="sxs-lookup"><span data-stu-id="35ed5-158">fill</span></span>|[<span data-ttu-id="35ed5-159">Воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="35ed5-159">WorkbookRangeFill</span></span>](rangefill.md)|<span data-ttu-id="35ed5-p106">Возвращает объект заливки, определенный для всего диапазона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35ed5-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="35ed5-162">font</span><span class="sxs-lookup"><span data-stu-id="35ed5-162">font</span></span>|[<span data-ttu-id="35ed5-163">Воркбукранжефонт</span><span class="sxs-lookup"><span data-stu-id="35ed5-163">WorkbookRangeFont</span></span>](rangefont.md)|<span data-ttu-id="35ed5-164">Возвращает объект шрифта, определенный для общего выбранного диапазона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35ed5-164">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="35ed5-165">protection</span><span class="sxs-lookup"><span data-stu-id="35ed5-165">protection</span></span>|[<span data-ttu-id="35ed5-166">Воркбукформатпротектион</span><span class="sxs-lookup"><span data-stu-id="35ed5-166">WorkbookFormatProtection</span></span>](formatprotection.md)|<span data-ttu-id="35ed5-167">Возвращает объект защиты формата для диапазона.</span><span class="sxs-lookup"><span data-stu-id="35ed5-167">Returns the format protection object for a range.</span></span> <span data-ttu-id="35ed5-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35ed5-168">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35ed5-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35ed5-169">JSON representation</span></span>

<span data-ttu-id="35ed5-170">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35ed5-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFormat"
}-->

```json
{
  "columnWidth": 1024,
  "horizontalAlignment": "string",
  "rowHeight": 1024,
  "verticalAlignment": "string",
  "wrapText": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
