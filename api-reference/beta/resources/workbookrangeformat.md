---
title: Тип ресурса Воркбукранжеформат
description: Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 27024cdc75358d80849b7fa67ff6262faadbbe46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519171"
---
# <a name="workbookrangeformat-resource-type"></a><span data-ttu-id="5e822-103">Тип ресурса Воркбукранжеформат</span><span class="sxs-lookup"><span data-stu-id="5e822-103">workbookRangeFormat resource type</span></span>

<span data-ttu-id="5e822-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e822-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e822-105">Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.</span><span class="sxs-lookup"><span data-stu-id="5e822-105">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="5e822-106">Методы</span><span class="sxs-lookup"><span data-stu-id="5e822-106">Methods</span></span>

| <span data-ttu-id="5e822-107">Метод</span><span class="sxs-lookup"><span data-stu-id="5e822-107">Method</span></span>           | <span data-ttu-id="5e822-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5e822-108">Return Type</span></span>    |<span data-ttu-id="5e822-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5e822-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5e822-110">Получение Воркбукранжеформат</span><span class="sxs-lookup"><span data-stu-id="5e822-110">Get workbookRangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="5e822-111">воркбукранжеформат</span><span class="sxs-lookup"><span data-stu-id="5e822-111">workbookRangeFormat</span></span>](workbookrangeformat.md) |<span data-ttu-id="5e822-112">Чтение свойств и связей объекта rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="5e822-112">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="5e822-113">Создание Воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="5e822-113">Create workbookRangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="5e822-114">воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="5e822-114">workbookRangeBorder</span></span>](workbookrangeborder.md)| <span data-ttu-id="5e822-115">Создание объекта RangeBorder путем добавления в коллекцию границ.</span><span class="sxs-lookup"><span data-stu-id="5e822-115">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="5e822-116">Список границ</span><span class="sxs-lookup"><span data-stu-id="5e822-116">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="5e822-117">Коллекция [воркбукранжебордер](workbookrangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="5e822-117">[workbookRangeBorder](workbookrangeborder.md) collection</span></span>| <span data-ttu-id="5e822-118">Получение коллекции объектов RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="5e822-118">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="5e822-119">Обновление</span><span class="sxs-lookup"><span data-stu-id="5e822-119">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="5e822-120">воркбукранжеформат</span><span class="sxs-lookup"><span data-stu-id="5e822-120">workbookRangeFormat</span></span>](workbookrangeformat.md) |<span data-ttu-id="5e822-121">Обновление объекта RangeFormat.</span><span class="sxs-lookup"><span data-stu-id="5e822-121">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="5e822-122">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="5e822-122">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="5e822-123">Нет</span><span class="sxs-lookup"><span data-stu-id="5e822-123">None</span></span>|<span data-ttu-id="5e822-124">Изменяет ширину столбцов текущего диапазона на оптимальную с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="5e822-124">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="5e822-125">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="5e822-125">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="5e822-126">Нет</span><span class="sxs-lookup"><span data-stu-id="5e822-126">None</span></span>|<span data-ttu-id="5e822-127">Изменяет высоту строк текущего диапазона на оптимальную с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="5e822-127">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e822-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e822-128">Properties</span></span>
| <span data-ttu-id="5e822-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e822-129">Property</span></span>     | <span data-ttu-id="5e822-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5e822-130">Type</span></span>   |<span data-ttu-id="5e822-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5e822-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e822-132">columnWidth</span><span class="sxs-lookup"><span data-stu-id="5e822-132">columnWidth</span></span>|<span data-ttu-id="5e822-133">double</span><span class="sxs-lookup"><span data-stu-id="5e822-133">double</span></span>|<span data-ttu-id="5e822-p101">Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="5e822-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="5e822-136">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="5e822-136">horizontalAlignment</span></span>|<span data-ttu-id="5e822-137">string</span><span class="sxs-lookup"><span data-stu-id="5e822-137">string</span></span>|<span data-ttu-id="5e822-p102">Представляет горизонтальное выравнивание для указанного объекта. Возможные значения: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="5e822-p102">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="5e822-140">rowHeight</span><span class="sxs-lookup"><span data-stu-id="5e822-140">rowHeight</span></span>|<span data-ttu-id="5e822-141">double</span><span class="sxs-lookup"><span data-stu-id="5e822-141">double</span></span>|<span data-ttu-id="5e822-p103">Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="5e822-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="5e822-144">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="5e822-144">verticalAlignment</span></span>|<span data-ttu-id="5e822-145">string</span><span class="sxs-lookup"><span data-stu-id="5e822-145">string</span></span>|<span data-ttu-id="5e822-p104">Представляет вертикальное выравнивание для указанного объекта. Возможные значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="5e822-p104">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="5e822-148">wrapText</span><span class="sxs-lookup"><span data-stu-id="5e822-148">wrapText</span></span>|<span data-ttu-id="5e822-149">boolean</span><span class="sxs-lookup"><span data-stu-id="5e822-149">boolean</span></span>|<span data-ttu-id="5e822-p105">Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.</span><span class="sxs-lookup"><span data-stu-id="5e822-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e822-152">Связи</span><span class="sxs-lookup"><span data-stu-id="5e822-152">Relationships</span></span>
| <span data-ttu-id="5e822-153">Связь</span><span class="sxs-lookup"><span data-stu-id="5e822-153">Relationship</span></span> | <span data-ttu-id="5e822-154">Тип</span><span class="sxs-lookup"><span data-stu-id="5e822-154">Type</span></span>   |<span data-ttu-id="5e822-155">Описание</span><span class="sxs-lookup"><span data-stu-id="5e822-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e822-156">borders</span><span class="sxs-lookup"><span data-stu-id="5e822-156">borders</span></span>|<span data-ttu-id="5e822-157">Коллекция [воркбукранжебордер](workbookrangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="5e822-157">[workbookRangeBorder](workbookrangeborder.md) collection</span></span>|<span data-ttu-id="5e822-158">Коллекция объектов границы, которые применяются к общему выделенному диапазону. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e822-158">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="5e822-159">fill</span><span class="sxs-lookup"><span data-stu-id="5e822-159">fill</span></span>|[<span data-ttu-id="5e822-160">воркбукранжефилл</span><span class="sxs-lookup"><span data-stu-id="5e822-160">workbookRangeFill</span></span>](workbookrangefill.md)|<span data-ttu-id="5e822-p106">Возвращает объект заливки, определенный для всего диапазона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e822-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="5e822-163">font</span><span class="sxs-lookup"><span data-stu-id="5e822-163">font</span></span>|[<span data-ttu-id="5e822-164">воркбукранжефонт</span><span class="sxs-lookup"><span data-stu-id="5e822-164">workbookRangeFont</span></span>](workbookrangefont.md)|<span data-ttu-id="5e822-165">Возвращает объект шрифта, определенный для общего выбранного диапазона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e822-165">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="5e822-166">protection</span><span class="sxs-lookup"><span data-stu-id="5e822-166">protection</span></span>|[<span data-ttu-id="5e822-167">formatProtection</span><span class="sxs-lookup"><span data-stu-id="5e822-167">formatProtection</span></span>](formatprotection.md)|<span data-ttu-id="5e822-168">Возвращает объект защиты формата для диапазона.</span><span class="sxs-lookup"><span data-stu-id="5e822-168">Returns the format protection object for a range.</span></span> <span data-ttu-id="5e822-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e822-169">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e822-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e822-170">JSON representation</span></span>

<span data-ttu-id="5e822-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e822-171">Here is a JSON representation of the resource.</span></span>

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
