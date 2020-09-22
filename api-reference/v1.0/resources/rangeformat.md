---
title: Тип ресурса RangeFormat
description: Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f78b0cfbbf709c7b398560c80282dc9ed2985092
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037068"
---
# <a name="rangeformat-resource-type"></a><span data-ttu-id="551ea-103">Тип ресурса RangeFormat</span><span class="sxs-lookup"><span data-stu-id="551ea-103">RangeFormat resource type</span></span>

<span data-ttu-id="551ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="551ea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="551ea-105">Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.</span><span class="sxs-lookup"><span data-stu-id="551ea-105">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="551ea-106">Методы</span><span class="sxs-lookup"><span data-stu-id="551ea-106">Methods</span></span>

| <span data-ttu-id="551ea-107">Метод</span><span class="sxs-lookup"><span data-stu-id="551ea-107">Method</span></span>           | <span data-ttu-id="551ea-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="551ea-108">Return Type</span></span>    |<span data-ttu-id="551ea-109">Описание</span><span class="sxs-lookup"><span data-stu-id="551ea-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="551ea-110">Получение объекта RangeFormat</span><span class="sxs-lookup"><span data-stu-id="551ea-110">Get RangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="551ea-111">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="551ea-111">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="551ea-112">Чтение свойств и связей объекта rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="551ea-112">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="551ea-113">Создание объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="551ea-113">Create RangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="551ea-114">воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="551ea-114">WorkbookRangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="551ea-115">Создание объекта RangeBorder путем добавления в коллекцию границ.</span><span class="sxs-lookup"><span data-stu-id="551ea-115">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="551ea-116">Список границ</span><span class="sxs-lookup"><span data-stu-id="551ea-116">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="551ea-117">Коллекция [воркбукранжебордер](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="551ea-117">[WorkbookRangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="551ea-118">Получение коллекции объектов RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="551ea-118">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="551ea-119">Обновление</span><span class="sxs-lookup"><span data-stu-id="551ea-119">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="551ea-120">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="551ea-120">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="551ea-121">Обновление объекта RangeFormat.</span><span class="sxs-lookup"><span data-stu-id="551ea-121">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="551ea-122">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="551ea-122">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="551ea-123">Нет</span><span class="sxs-lookup"><span data-stu-id="551ea-123">None</span></span>|<span data-ttu-id="551ea-124">Изменяет ширину столбцов текущего диапазона на оптимальную с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="551ea-124">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="551ea-125">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="551ea-125">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="551ea-126">Нет</span><span class="sxs-lookup"><span data-stu-id="551ea-126">None</span></span>|<span data-ttu-id="551ea-127">Изменяет высоту строк текущего диапазона на оптимальную с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="551ea-127">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="551ea-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="551ea-128">Properties</span></span>
| <span data-ttu-id="551ea-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="551ea-129">Property</span></span>     | <span data-ttu-id="551ea-130">Тип</span><span class="sxs-lookup"><span data-stu-id="551ea-130">Type</span></span>   |<span data-ttu-id="551ea-131">Описание</span><span class="sxs-lookup"><span data-stu-id="551ea-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="551ea-132">columnWidth</span><span class="sxs-lookup"><span data-stu-id="551ea-132">columnWidth</span></span>|<span data-ttu-id="551ea-133">double</span><span class="sxs-lookup"><span data-stu-id="551ea-133">double</span></span>|<span data-ttu-id="551ea-p101">Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="551ea-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="551ea-136">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="551ea-136">horizontalAlignment</span></span>|<span data-ttu-id="551ea-137">string</span><span class="sxs-lookup"><span data-stu-id="551ea-137">string</span></span>|<span data-ttu-id="551ea-138">Представляет выравнивание по горизонтали для указанного объекта.</span><span class="sxs-lookup"><span data-stu-id="551ea-138">Represents the horizontal alignment for the specified object.</span></span> <span data-ttu-id="551ea-139">Возможные значения:,, `General` `Left` ,, `Center` `Right` `Fill` , `Justify` , `CenterAcrossSelection` , `Distributed` .</span><span class="sxs-lookup"><span data-stu-id="551ea-139">The possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="551ea-140">rowHeight</span><span class="sxs-lookup"><span data-stu-id="551ea-140">rowHeight</span></span>|<span data-ttu-id="551ea-141">double</span><span class="sxs-lookup"><span data-stu-id="551ea-141">double</span></span>|<span data-ttu-id="551ea-p103">Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="551ea-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="551ea-144">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="551ea-144">verticalAlignment</span></span>|<span data-ttu-id="551ea-145">string</span><span class="sxs-lookup"><span data-stu-id="551ea-145">string</span></span>|<span data-ttu-id="551ea-146">Представляет выравнивание по вертикали для указанного объекта.</span><span class="sxs-lookup"><span data-stu-id="551ea-146">Represents the vertical alignment for the specified object.</span></span> <span data-ttu-id="551ea-147">Допустимые значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="551ea-147">The possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="551ea-148">wrapText</span><span class="sxs-lookup"><span data-stu-id="551ea-148">wrapText</span></span>|<span data-ttu-id="551ea-149">boolean</span><span class="sxs-lookup"><span data-stu-id="551ea-149">boolean</span></span>|<span data-ttu-id="551ea-p105">Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.</span><span class="sxs-lookup"><span data-stu-id="551ea-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="551ea-152">Связи</span><span class="sxs-lookup"><span data-stu-id="551ea-152">Relationships</span></span>
| <span data-ttu-id="551ea-153">Связь</span><span class="sxs-lookup"><span data-stu-id="551ea-153">Relationship</span></span> | <span data-ttu-id="551ea-154">Тип</span><span class="sxs-lookup"><span data-stu-id="551ea-154">Type</span></span>   |<span data-ttu-id="551ea-155">Описание</span><span class="sxs-lookup"><span data-stu-id="551ea-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="551ea-156">borders</span><span class="sxs-lookup"><span data-stu-id="551ea-156">borders</span></span>|<span data-ttu-id="551ea-157">Коллекция [воркбукранжебордер](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="551ea-157">[WorkbookRangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="551ea-158">Коллекция объектов границы, которые применяются к общему выделенному диапазону. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="551ea-158">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="551ea-159">fill</span><span class="sxs-lookup"><span data-stu-id="551ea-159">fill</span></span>|[<span data-ttu-id="551ea-160">воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="551ea-160">WorkbookRangeFill</span></span>](rangefill.md)|<span data-ttu-id="551ea-p106">Возвращает объект заливки, определенный для всего диапазона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="551ea-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="551ea-163">font</span><span class="sxs-lookup"><span data-stu-id="551ea-163">font</span></span>|[<span data-ttu-id="551ea-164">воркбукранжефонт</span><span class="sxs-lookup"><span data-stu-id="551ea-164">WorkbookRangeFont</span></span>](rangefont.md)|<span data-ttu-id="551ea-165">Возвращает объект шрифта, определенный для общего выбранного диапазона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="551ea-165">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="551ea-166">protection</span><span class="sxs-lookup"><span data-stu-id="551ea-166">protection</span></span>|[<span data-ttu-id="551ea-167">воркбукформатпротектион</span><span class="sxs-lookup"><span data-stu-id="551ea-167">WorkbookFormatProtection</span></span>](formatprotection.md)|<span data-ttu-id="551ea-168">Возвращает объект защиты формата для диапазона.</span><span class="sxs-lookup"><span data-stu-id="551ea-168">Returns the format protection object for a range.</span></span> <span data-ttu-id="551ea-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="551ea-169">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="551ea-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="551ea-170">JSON representation</span></span>

<span data-ttu-id="551ea-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="551ea-171">Here is a JSON representation of the resource.</span></span>

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

