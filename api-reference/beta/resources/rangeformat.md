---
title: Тип ресурса RangeFormat
description: Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: b4018995e37ff40ae014b54d08b77bbed73d6fe2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937350"
---
# <a name="rangeformat-resource-type"></a><span data-ttu-id="345de-103">Тип ресурса RangeFormat</span><span class="sxs-lookup"><span data-stu-id="345de-103">RangeFormat resource type</span></span>

> <span data-ttu-id="345de-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="345de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="345de-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="345de-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="345de-106">Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.</span><span class="sxs-lookup"><span data-stu-id="345de-106">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="345de-107">Методы</span><span class="sxs-lookup"><span data-stu-id="345de-107">Methods</span></span>

| <span data-ttu-id="345de-108">Метод</span><span class="sxs-lookup"><span data-stu-id="345de-108">Method</span></span>           | <span data-ttu-id="345de-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="345de-109">Return Type</span></span>    |<span data-ttu-id="345de-110">Описание</span><span class="sxs-lookup"><span data-stu-id="345de-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="345de-111">Получение объекта RangeFormat</span><span class="sxs-lookup"><span data-stu-id="345de-111">Get RangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="345de-112">RangeFormat</span><span class="sxs-lookup"><span data-stu-id="345de-112">RangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="345de-113">Чтение свойств и связей объекта rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="345de-113">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="345de-114">Создание объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="345de-114">Create RangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="345de-115">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="345de-115">RangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="345de-116">Создание объекта RangeBorder путем добавления в коллекцию границ.</span><span class="sxs-lookup"><span data-stu-id="345de-116">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="345de-117">Список границ</span><span class="sxs-lookup"><span data-stu-id="345de-117">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="345de-118">Коллекция объектов [RangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="345de-118">[RangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="345de-119">Получение коллекции объектов RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="345de-119">Get a RangeBorder object collection.</span></span>|
|<span data-ttu-id="345de-120">[обновление](../api/rangeformat-update.md).</span><span class="sxs-lookup"><span data-stu-id="345de-120">[Update](../api/rangeformat-update.md)</span></span> | [<span data-ttu-id="345de-121">RangeFormat</span><span class="sxs-lookup"><span data-stu-id="345de-121">RangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="345de-122">Обновление объекта RangeFormat.</span><span class="sxs-lookup"><span data-stu-id="345de-122">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="345de-123">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="345de-123">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="345de-124">Нет</span><span class="sxs-lookup"><span data-stu-id="345de-124">None</span></span>|<span data-ttu-id="345de-125">Изменяет ширину столбцов текущего диапазона на оптимальную с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="345de-125">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="345de-126">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="345de-126">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="345de-127">Нет</span><span class="sxs-lookup"><span data-stu-id="345de-127">None</span></span>|<span data-ttu-id="345de-128">Изменяет высоту строк текущего диапазона на оптимальную с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="345de-128">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="345de-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="345de-129">Properties</span></span>
| <span data-ttu-id="345de-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="345de-130">Property</span></span>     | <span data-ttu-id="345de-131">Тип</span><span class="sxs-lookup"><span data-stu-id="345de-131">Type</span></span>   |<span data-ttu-id="345de-132">Описание</span><span class="sxs-lookup"><span data-stu-id="345de-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="345de-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="345de-133">columnWidth</span></span>|<span data-ttu-id="345de-134">double</span><span class="sxs-lookup"><span data-stu-id="345de-134">double</span></span>|<span data-ttu-id="345de-p102">Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="345de-p102">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="345de-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="345de-137">horizontalAlignment</span></span>|<span data-ttu-id="345de-138">строка</span><span class="sxs-lookup"><span data-stu-id="345de-138">string</span></span>|<span data-ttu-id="345de-p103">Представляет горизонтальное выравнивание для указанного объекта. Возможные значения: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="345de-p103">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="345de-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="345de-141">rowHeight</span></span>|<span data-ttu-id="345de-142">double</span><span class="sxs-lookup"><span data-stu-id="345de-142">double</span></span>|<span data-ttu-id="345de-p104">Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="345de-p104">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="345de-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="345de-145">verticalAlignment</span></span>|<span data-ttu-id="345de-146">строка</span><span class="sxs-lookup"><span data-stu-id="345de-146">string</span></span>|<span data-ttu-id="345de-p105">Представляет вертикальное выравнивание для указанного объекта. Возможные значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="345de-p105">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="345de-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="345de-149">wrapText</span></span>|<span data-ttu-id="345de-150">boolean</span><span class="sxs-lookup"><span data-stu-id="345de-150">boolean</span></span>|<span data-ttu-id="345de-p106">Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.</span><span class="sxs-lookup"><span data-stu-id="345de-p106">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="345de-153">Связи</span><span class="sxs-lookup"><span data-stu-id="345de-153">Relationships</span></span>
| <span data-ttu-id="345de-154">Связь</span><span class="sxs-lookup"><span data-stu-id="345de-154">Relationship</span></span> | <span data-ttu-id="345de-155">Тип</span><span class="sxs-lookup"><span data-stu-id="345de-155">Type</span></span>   |<span data-ttu-id="345de-156">Описание</span><span class="sxs-lookup"><span data-stu-id="345de-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="345de-157">borders</span><span class="sxs-lookup"><span data-stu-id="345de-157">borders</span></span>|<span data-ttu-id="345de-158">Коллекция объектов [RangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="345de-158">[RangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="345de-159">Коллекция объектов границ, которые применяются к общему выделенному диапазону. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="345de-159">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="345de-160">fill</span><span class="sxs-lookup"><span data-stu-id="345de-160">fill</span></span>|[<span data-ttu-id="345de-161">RangeFill</span><span class="sxs-lookup"><span data-stu-id="345de-161">RangeFill</span></span>](rangefill.md)|<span data-ttu-id="345de-p107">Возвращает объект заливки, определенный для всего диапазона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="345de-p107">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="345de-164">font</span><span class="sxs-lookup"><span data-stu-id="345de-164">font</span></span>|[<span data-ttu-id="345de-165">RangeFont</span><span class="sxs-lookup"><span data-stu-id="345de-165">RangeFont</span></span>](rangefont.md)|<span data-ttu-id="345de-166">Возвращает объект шрифта, определенный для общего выбранного диапазона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="345de-166">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="345de-167">protection</span><span class="sxs-lookup"><span data-stu-id="345de-167">protection</span></span>|[<span data-ttu-id="345de-168">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="345de-168">FormatProtection</span></span>](formatprotection.md)|<span data-ttu-id="345de-p108">Возвращает объект защиты формата для диапазона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="345de-p108">Returns the format protection object for a range. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="345de-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="345de-171">JSON representation</span></span>

<span data-ttu-id="345de-172">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="345de-172">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
