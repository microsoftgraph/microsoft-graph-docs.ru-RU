---
title: Тип ресурса Воркбукранжеформат
description: Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 3ee55e1a398dab1727dfdc24d9ebd5c66b7440d3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33349012"
---
# <a name="workbookrangeformat-resource-type"></a><span data-ttu-id="65aaf-103">Тип ресурса Воркбукранжеформат</span><span class="sxs-lookup"><span data-stu-id="65aaf-103">workbookRangeFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65aaf-104">Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.</span><span class="sxs-lookup"><span data-stu-id="65aaf-104">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="65aaf-105">Методы</span><span class="sxs-lookup"><span data-stu-id="65aaf-105">Methods</span></span>

| <span data-ttu-id="65aaf-106">Метод</span><span class="sxs-lookup"><span data-stu-id="65aaf-106">Method</span></span>           | <span data-ttu-id="65aaf-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="65aaf-107">Return Type</span></span>    |<span data-ttu-id="65aaf-108">Описание</span><span class="sxs-lookup"><span data-stu-id="65aaf-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="65aaf-109">Получение Воркбукранжеформат</span><span class="sxs-lookup"><span data-stu-id="65aaf-109">Get workbookRangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="65aaf-110">Воркбукранжеформат</span><span class="sxs-lookup"><span data-stu-id="65aaf-110">workbookRangeFormat</span></span>](workbookrangeformat.md) |<span data-ttu-id="65aaf-111">Чтение свойств и связей объекта rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="65aaf-111">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="65aaf-112">Создание Воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="65aaf-112">Create workbookRangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="65aaf-113">Воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="65aaf-113">workbookRangeBorder</span></span>](workbookrangeborder.md)| <span data-ttu-id="65aaf-114">Создание объекта RangeBorder путем добавления в коллекцию границ.</span><span class="sxs-lookup"><span data-stu-id="65aaf-114">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="65aaf-115">Список границ</span><span class="sxs-lookup"><span data-stu-id="65aaf-115">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="65aaf-116">Коллекция [воркбукранжебордер](workbookrangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="65aaf-116">[workbookRangeBorder](workbookrangeborder.md) collection</span></span>| <span data-ttu-id="65aaf-117">Получение коллекции объектов RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="65aaf-117">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="65aaf-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="65aaf-118">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="65aaf-119">Воркбукранжеформат</span><span class="sxs-lookup"><span data-stu-id="65aaf-119">workbookRangeFormat</span></span>](workbookrangeformat.md) |<span data-ttu-id="65aaf-120">Обновление объекта RangeFormat.</span><span class="sxs-lookup"><span data-stu-id="65aaf-120">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="65aaf-121">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="65aaf-121">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="65aaf-122">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="65aaf-122">None</span></span>|<span data-ttu-id="65aaf-123">Изменяет ширину столбцов текущего диапазона на оптимальную с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="65aaf-123">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="65aaf-124">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="65aaf-124">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="65aaf-125">Нет</span><span class="sxs-lookup"><span data-stu-id="65aaf-125">None</span></span>|<span data-ttu-id="65aaf-126">Изменяет высоту строк текущего диапазона на оптимальную с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="65aaf-126">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="65aaf-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="65aaf-127">Properties</span></span>
| <span data-ttu-id="65aaf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="65aaf-128">Property</span></span>     | <span data-ttu-id="65aaf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="65aaf-129">Type</span></span>   |<span data-ttu-id="65aaf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="65aaf-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65aaf-131">columnWidth</span><span class="sxs-lookup"><span data-stu-id="65aaf-131">columnWidth</span></span>|<span data-ttu-id="65aaf-132">double</span><span class="sxs-lookup"><span data-stu-id="65aaf-132">double</span></span>|<span data-ttu-id="65aaf-p101">Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="65aaf-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="65aaf-135">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="65aaf-135">horizontalAlignment</span></span>|<span data-ttu-id="65aaf-136">string</span><span class="sxs-lookup"><span data-stu-id="65aaf-136">string</span></span>|<span data-ttu-id="65aaf-p102">Представляет горизонтальное выравнивание для указанного объекта. Возможные значения: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="65aaf-p102">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="65aaf-139">rowHeight</span><span class="sxs-lookup"><span data-stu-id="65aaf-139">rowHeight</span></span>|<span data-ttu-id="65aaf-140">double</span><span class="sxs-lookup"><span data-stu-id="65aaf-140">double</span></span>|<span data-ttu-id="65aaf-p103">Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="65aaf-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="65aaf-143">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="65aaf-143">verticalAlignment</span></span>|<span data-ttu-id="65aaf-144">string</span><span class="sxs-lookup"><span data-stu-id="65aaf-144">string</span></span>|<span data-ttu-id="65aaf-p104">Представляет вертикальное выравнивание для указанного объекта. Возможные значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="65aaf-p104">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="65aaf-147">wrapText</span><span class="sxs-lookup"><span data-stu-id="65aaf-147">wrapText</span></span>|<span data-ttu-id="65aaf-148">boolean</span><span class="sxs-lookup"><span data-stu-id="65aaf-148">boolean</span></span>|<span data-ttu-id="65aaf-p105">Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.</span><span class="sxs-lookup"><span data-stu-id="65aaf-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="65aaf-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="65aaf-151">Relationships</span></span>
| <span data-ttu-id="65aaf-152">Отношение</span><span class="sxs-lookup"><span data-stu-id="65aaf-152">Relationship</span></span> | <span data-ttu-id="65aaf-153">Тип</span><span class="sxs-lookup"><span data-stu-id="65aaf-153">Type</span></span>   |<span data-ttu-id="65aaf-154">Описание</span><span class="sxs-lookup"><span data-stu-id="65aaf-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65aaf-155">borders</span><span class="sxs-lookup"><span data-stu-id="65aaf-155">borders</span></span>|<span data-ttu-id="65aaf-156">Коллекция [воркбукранжебордер](workbookrangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="65aaf-156">[workbookRangeBorder](workbookrangeborder.md) collection</span></span>|<span data-ttu-id="65aaf-157">Коллекция объектов границы, которые применяются к общему выделенному диапазону. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65aaf-157">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="65aaf-158">fill</span><span class="sxs-lookup"><span data-stu-id="65aaf-158">fill</span></span>|[<span data-ttu-id="65aaf-159">Воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="65aaf-159">workbookRangeFill</span></span>](workbookrangefill.md)|<span data-ttu-id="65aaf-p106">Возвращает объект заливки, определенный для всего диапазона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65aaf-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="65aaf-162">font</span><span class="sxs-lookup"><span data-stu-id="65aaf-162">font</span></span>|[<span data-ttu-id="65aaf-163">Воркбукранжефонт</span><span class="sxs-lookup"><span data-stu-id="65aaf-163">workbookRangeFont</span></span>](workbookrangefont.md)|<span data-ttu-id="65aaf-164">Возвращает объект шрифта, определенный для общего выбранного диапазона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65aaf-164">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="65aaf-165">protection</span><span class="sxs-lookup"><span data-stu-id="65aaf-165">protection</span></span>|[<span data-ttu-id="65aaf-166">formatProtection</span><span class="sxs-lookup"><span data-stu-id="65aaf-166">formatProtection</span></span>](formatprotection.md)|<span data-ttu-id="65aaf-167">Возвращает объект защиты формата для диапазона.</span><span class="sxs-lookup"><span data-stu-id="65aaf-167">Returns the format protection object for a range.</span></span> <span data-ttu-id="65aaf-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65aaf-168">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65aaf-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65aaf-169">JSON representation</span></span>

<span data-ttu-id="65aaf-170">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65aaf-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
