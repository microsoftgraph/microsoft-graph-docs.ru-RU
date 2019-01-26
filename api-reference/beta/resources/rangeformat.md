---
title: Тип ресурса rangeFormat
description: Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 1394153a09a30c273280dab5469a40e2e0c2c4ad
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572425"
---
# <a name="rangeformat-resource-type"></a><span data-ttu-id="31292-103">Тип ресурса RangeFormat</span><span class="sxs-lookup"><span data-stu-id="31292-103">RangeFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31292-104">Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.</span><span class="sxs-lookup"><span data-stu-id="31292-104">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="31292-105">Методы</span><span class="sxs-lookup"><span data-stu-id="31292-105">Methods</span></span>

| <span data-ttu-id="31292-106">Метод</span><span class="sxs-lookup"><span data-stu-id="31292-106">Method</span></span>           | <span data-ttu-id="31292-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="31292-107">Return Type</span></span>    |<span data-ttu-id="31292-108">Описание</span><span class="sxs-lookup"><span data-stu-id="31292-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="31292-109">Получение объекта RangeFormat</span><span class="sxs-lookup"><span data-stu-id="31292-109">Get RangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="31292-110">RangeFormat</span><span class="sxs-lookup"><span data-stu-id="31292-110">RangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="31292-111">Чтение свойств и связей объекта rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="31292-111">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="31292-112">Создание объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="31292-112">Create RangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="31292-113">rangeBorder</span><span class="sxs-lookup"><span data-stu-id="31292-113">rangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="31292-114">Создание объекта RangeBorder путем добавления в коллекцию границ.</span><span class="sxs-lookup"><span data-stu-id="31292-114">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="31292-115">Список границ</span><span class="sxs-lookup"><span data-stu-id="31292-115">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="31292-116">[rangeBorder](rangeborder.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="31292-116">[rangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="31292-117">Получение коллекции объектов RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="31292-117">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="31292-118">Update</span><span class="sxs-lookup"><span data-stu-id="31292-118">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="31292-119">rangeFormat</span><span class="sxs-lookup"><span data-stu-id="31292-119">rangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="31292-120">Обновление объекта RangeFormat.</span><span class="sxs-lookup"><span data-stu-id="31292-120">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="31292-121">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="31292-121">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="31292-122">Нет</span><span class="sxs-lookup"><span data-stu-id="31292-122">None</span></span>|<span data-ttu-id="31292-123">Изменяет ширину столбцов текущего диапазона на оптимальную с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="31292-123">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="31292-124">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="31292-124">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="31292-125">Нет</span><span class="sxs-lookup"><span data-stu-id="31292-125">None</span></span>|<span data-ttu-id="31292-126">Изменяет высоту строк текущего диапазона на оптимальную с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="31292-126">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="31292-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="31292-127">Properties</span></span>
| <span data-ttu-id="31292-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="31292-128">Property</span></span>     | <span data-ttu-id="31292-129">Тип</span><span class="sxs-lookup"><span data-stu-id="31292-129">Type</span></span>   |<span data-ttu-id="31292-130">Описание</span><span class="sxs-lookup"><span data-stu-id="31292-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31292-131">columnWidth</span><span class="sxs-lookup"><span data-stu-id="31292-131">columnWidth</span></span>|<span data-ttu-id="31292-132">double</span><span class="sxs-lookup"><span data-stu-id="31292-132">double</span></span>|<span data-ttu-id="31292-p101">Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="31292-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="31292-135">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="31292-135">horizontalAlignment</span></span>|<span data-ttu-id="31292-136">string</span><span class="sxs-lookup"><span data-stu-id="31292-136">string</span></span>|<span data-ttu-id="31292-p102">Представляет горизонтальное выравнивание для указанного объекта. Возможные значения: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="31292-p102">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="31292-139">rowHeight</span><span class="sxs-lookup"><span data-stu-id="31292-139">rowHeight</span></span>|<span data-ttu-id="31292-140">double</span><span class="sxs-lookup"><span data-stu-id="31292-140">double</span></span>|<span data-ttu-id="31292-p103">Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="31292-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="31292-143">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="31292-143">verticalAlignment</span></span>|<span data-ttu-id="31292-144">string</span><span class="sxs-lookup"><span data-stu-id="31292-144">string</span></span>|<span data-ttu-id="31292-p104">Представляет вертикальное выравнивание для указанного объекта. Возможные значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="31292-p104">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="31292-147">wrapText</span><span class="sxs-lookup"><span data-stu-id="31292-147">wrapText</span></span>|<span data-ttu-id="31292-148">boolean</span><span class="sxs-lookup"><span data-stu-id="31292-148">boolean</span></span>|<span data-ttu-id="31292-p105">Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.</span><span class="sxs-lookup"><span data-stu-id="31292-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="31292-151">Связи</span><span class="sxs-lookup"><span data-stu-id="31292-151">Relationships</span></span>
| <span data-ttu-id="31292-152">Связь</span><span class="sxs-lookup"><span data-stu-id="31292-152">Relationship</span></span> | <span data-ttu-id="31292-153">Тип</span><span class="sxs-lookup"><span data-stu-id="31292-153">Type</span></span>   |<span data-ttu-id="31292-154">Описание</span><span class="sxs-lookup"><span data-stu-id="31292-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31292-155">borders</span><span class="sxs-lookup"><span data-stu-id="31292-155">borders</span></span>|<span data-ttu-id="31292-156">[rangeBorder](rangeborder.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="31292-156">[rangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="31292-157">Коллекция объектов границ, которые применяются к общему выделенному диапазону. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31292-157">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="31292-158">fill</span><span class="sxs-lookup"><span data-stu-id="31292-158">fill</span></span>|[<span data-ttu-id="31292-159">rangeFill</span><span class="sxs-lookup"><span data-stu-id="31292-159">rangeFill</span></span>](rangefill.md)|<span data-ttu-id="31292-p106">Возвращает объект заливки, определенный для всего диапазона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31292-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="31292-162">font</span><span class="sxs-lookup"><span data-stu-id="31292-162">font</span></span>|[<span data-ttu-id="31292-163">rangeFont</span><span class="sxs-lookup"><span data-stu-id="31292-163">rangeFont</span></span>](rangefont.md)|<span data-ttu-id="31292-164">Возвращает объект шрифта, определенный для общего выбранного диапазона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31292-164">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="31292-165">protection</span><span class="sxs-lookup"><span data-stu-id="31292-165">protection</span></span>|[<span data-ttu-id="31292-166">formatProtection</span><span class="sxs-lookup"><span data-stu-id="31292-166">formatProtection</span></span>](formatprotection.md)|<span data-ttu-id="31292-p107">Возвращает объект защиты формата для диапазона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31292-p107">Returns the format protection object for a range. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="31292-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31292-169">JSON representation</span></span>

<span data-ttu-id="31292-170">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31292-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFormat"
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
<!--
{
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangeformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
