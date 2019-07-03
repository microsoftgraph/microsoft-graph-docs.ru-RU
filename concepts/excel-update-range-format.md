---
title: Обновление формата диапазона в Excel с помощью Microsoft Graph
description: В приведенных ниже примерах показано, как обновить свойства RangeFormat, RangeFill и RangeFont указанного диапазона.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 9874a24848126cfd065158a318699606fc02e352
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460807"
---
# <a name="update-a-range-format-in-excel-with-microsoft-graph"></a><span data-ttu-id="16d8e-103">Обновление формата диапазона в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="16d8e-103">Update a range format in Excel with Microsoft Graph</span></span>

<span data-ttu-id="16d8e-104">В приведенных ниже примерах показано, как обновить свойства [RangeFormat](/graph/api/resources/rangeformat?view=graph-rest-1.0), [RangeFill](/graph/api/resources/rangefill?view=graph-rest-1.0) и [RangeFont](/graph/api/resources/rangefont?view=graph-rest-1.0) указанного диапазона.</span><span class="sxs-lookup"><span data-stu-id="16d8e-104">The following examples demonstrate how to update properties of the [RangeFormat](/graph/api/resources/rangeformat?view=graph-rest-1.0), [RangeFill](/graph/api/resources/rangefill?view=graph-rest-1.0), and [RangeFont](/graph/api/resources/rangefont?view=graph-rest-1.0) properties of a specified range.</span></span>

<span data-ttu-id="16d8e-105">В результате этого набора запросов создается таблица с тремя ячейками, отформатированными так же, как три ячейки на приведенном ниже рисунке.</span><span class="sxs-lookup"><span data-stu-id="16d8e-105">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Таблица-диаграмма Excel с тремя ячейками, свойства Format, Fill и Font которых были обновлены.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="16d8e-107">Запрос</span><span class="sxs-lookup"><span data-stu-id="16d8e-107">Request</span></span>
<span data-ttu-id="16d8e-108">Этот запрос обновляет выравнивание по вертикали, высоту строк и столбцов первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="16d8e-108">This request updates the vertical alignment, row height, and column height of the first cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="16d8e-109">HTTP</span><span class="sxs-lookup"><span data-stu-id="16d8e-109">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="16d8e-110">C#</span><span class="sxs-lookup"><span data-stu-id="16d8e-110">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16d8e-111">Javascript</span><span class="sxs-lookup"><span data-stu-id="16d8e-111">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="16d8e-112">Цель — C</span><span class="sxs-lookup"><span data-stu-id="16d8e-112">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="16d8e-113">Отклик</span><span class="sxs-lookup"><span data-stu-id="16d8e-113">Response</span></span>
<span data-ttu-id="16d8e-p101">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16d8e-p101">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "General",
    "rowHeight": 49,
    "verticalAlignment": "Top",
    "wrapText": false
}
```

##### <a name="request"></a><span data-ttu-id="16d8e-117">Запрос</span><span class="sxs-lookup"><span data-stu-id="16d8e-117">Request</span></span>
<span data-ttu-id="16d8e-118">Этот запрос обновляет начертание, размер и цвет шрифта в первой ячейке.</span><span class="sxs-lookup"><span data-stu-id="16d8e-118">This request updates the font style, size, and color of the first cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="16d8e-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="16d8e-119">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_font"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/font
Content-type: application/json

{
  "bold": true,
  "color": "#4B180E",
  "size": 26
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="16d8e-120">C#</span><span class="sxs-lookup"><span data-stu-id="16d8e-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16d8e-121">Javascript</span><span class="sxs-lookup"><span data-stu-id="16d8e-121">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="16d8e-122">Цель — C</span><span class="sxs-lookup"><span data-stu-id="16d8e-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="16d8e-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="16d8e-123">Response</span></span>
<span data-ttu-id="16d8e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16d8e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": true,
    "color": "#4B180E",
    "italic": false,
    "name": "Calibri",
    "size": 26,
    "underline": "None"
}
```

##### <a name="request"></a><span data-ttu-id="16d8e-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="16d8e-127">Request</span></span>
<span data-ttu-id="16d8e-128">Этот запрос обновляет цвет заливки первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="16d8e-128">This request updates the background color of the first cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="16d8e-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="16d8e-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="16d8e-130">C#</span><span class="sxs-lookup"><span data-stu-id="16d8e-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16d8e-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="16d8e-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="16d8e-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="16d8e-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="16d8e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="16d8e-133">Response</span></span>
<span data-ttu-id="16d8e-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16d8e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#FF0000"
}
```
##### <a name="request"></a><span data-ttu-id="16d8e-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="16d8e-137">Request</span></span>
<span data-ttu-id="16d8e-138">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="16d8e-138">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="16d8e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="16d8e-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Center",
  "verticalAlignment": "Center",
  "rowHeight": 49,
  "wrapText": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="16d8e-140">C#</span><span class="sxs-lookup"><span data-stu-id="16d8e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16d8e-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="16d8e-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="16d8e-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="16d8e-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="16d8e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="16d8e-143">Response</span></span>
<span data-ttu-id="16d8e-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16d8e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "Center",
    "rowHeight": 49,
    "verticalAlignment": "Center",
    "wrapText": false
}
```

##### <a name="request"></a><span data-ttu-id="16d8e-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="16d8e-147">Request</span></span>
<span data-ttu-id="16d8e-148">Этот запрос обновляет начертание и размер шрифта во второй ячейке.</span><span class="sxs-lookup"><span data-stu-id="16d8e-148">This request updates the font style and size of the second cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="16d8e-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="16d8e-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_font_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/font
Content-type: application/json

{
  "italic": true,
  "size": 26
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="16d8e-150">C#</span><span class="sxs-lookup"><span data-stu-id="16d8e-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16d8e-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="16d8e-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="16d8e-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="16d8e-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="16d8e-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="16d8e-153">Response</span></span>
<span data-ttu-id="16d8e-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16d8e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": false,
    "color": "#000000",
    "italic": true,
    "name": "Calibri",
    "size": 26,
    "underline": "None"
}
```

##### <a name="request"></a><span data-ttu-id="16d8e-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="16d8e-157">Request</span></span>
<span data-ttu-id="16d8e-158">Этот запрос обновляет цвет заливки второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="16d8e-158">This request updates the background color of the second cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="16d8e-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="16d8e-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="16d8e-160">C#</span><span class="sxs-lookup"><span data-stu-id="16d8e-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16d8e-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="16d8e-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="16d8e-162">Цель — C</span><span class="sxs-lookup"><span data-stu-id="16d8e-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="16d8e-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="16d8e-163">Response</span></span>
<span data-ttu-id="16d8e-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16d8e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#00FF00"
}
```

##### <a name="request"></a><span data-ttu-id="16d8e-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="16d8e-167">Request</span></span>
<span data-ttu-id="16d8e-168">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="16d8e-168">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="16d8e-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="16d8e-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Right",
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="16d8e-170">C#</span><span class="sxs-lookup"><span data-stu-id="16d8e-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16d8e-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="16d8e-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="16d8e-172">Цель — C</span><span class="sxs-lookup"><span data-stu-id="16d8e-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="16d8e-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="16d8e-173">Response</span></span>
<span data-ttu-id="16d8e-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16d8e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "Right",
    "rowHeight": 49,
    "verticalAlignment": "Top",
    "wrapText": false
}
```

##### <a name="request"></a><span data-ttu-id="16d8e-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="16d8e-177">Request</span></span>
<span data-ttu-id="16d8e-178">Этот запрос обновляет начертание, размер и цвет шрифта в третьей ячейке.</span><span class="sxs-lookup"><span data-stu-id="16d8e-178">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="16d8e-179">Обратите внимание: свойство подчеркивания (Underline) принимает значения **Single** или **Double**.</span><span class="sxs-lookup"><span data-stu-id="16d8e-179">Note that the underline property takes **Single** or **Double** as values.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="16d8e-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="16d8e-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_font_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/font
Content-type: application/json

{
  "underline": "Single",
  "color": "#FFFFFF",
  "size": 26
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="16d8e-181">C#</span><span class="sxs-lookup"><span data-stu-id="16d8e-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16d8e-182">Javascript</span><span class="sxs-lookup"><span data-stu-id="16d8e-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="16d8e-183">Цель — C</span><span class="sxs-lookup"><span data-stu-id="16d8e-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="16d8e-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="16d8e-184">Response</span></span>
<span data-ttu-id="16d8e-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16d8e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": false,
    "color": "#FFFFFF",
    "italic": false,
    "name": "Calibri",
    "size": 26,
    "underline": "Single"
}
```

##### <a name="request"></a><span data-ttu-id="16d8e-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="16d8e-188">Request</span></span>
<span data-ttu-id="16d8e-189">Этот запрос обновляет цвет заливки третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="16d8e-189">This request updates the background color of the third cell.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="16d8e-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="16d8e-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="16d8e-191">C#</span><span class="sxs-lookup"><span data-stu-id="16d8e-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16d8e-192">Javascript</span><span class="sxs-lookup"><span data-stu-id="16d8e-192">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="16d8e-193">Цель — C</span><span class="sxs-lookup"><span data-stu-id="16d8e-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="16d8e-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="16d8e-194">Response</span></span>
<span data-ttu-id="16d8e-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="16d8e-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#0000FF"
}
```


## <a name="see-also"></a><span data-ttu-id="16d8e-198">См. также</span><span class="sxs-lookup"><span data-stu-id="16d8e-198">See also</span></span>
* [<span data-ttu-id="16d8e-199">Управление сеансами в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="16d8e-199">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="16d8e-200">Запись в книгу Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="16d8e-200">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="16d8e-201">Использование функций книг в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="16d8e-201">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="16d8e-202">Показ изображения диаграммы в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="16d8e-202">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="16d8e-203">Использование REST API для Excel</span><span class="sxs-lookup"><span data-stu-id="16d8e-203">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update a range format in Excel with Microsoft Graph",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
