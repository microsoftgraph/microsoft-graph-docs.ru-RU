---
title: Обновление формата диапазона в Excel с помощью Microsoft Graph
description: В приведенных ниже примерах показано, как обновить свойства RangeFormat, RangeFill и RangeFont указанного диапазона.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: ae373ef28a77584d403adda5d4c948fa4c1325ec
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050180"
---
# <a name="update-a-range-format-in-excel-with-microsoft-graph"></a><span data-ttu-id="92e78-103">Обновление формата диапазона в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="92e78-103">Update a range format in Excel with Microsoft Graph</span></span>

<span data-ttu-id="92e78-104">В приведенных ниже примерах показано, как обновить свойства [RangeFormat](/graph/api/resources/rangeformat?view=graph-rest-1.0), [RangeFill](/graph/api/resources/rangefill?view=graph-rest-1.0) и [RangeFont](/graph/api/resources/rangefont?view=graph-rest-1.0) указанного диапазона.</span><span class="sxs-lookup"><span data-stu-id="92e78-104">The following examples demonstrate how to update properties of the [RangeFormat](/graph/api/resources/rangeformat?view=graph-rest-1.0), [RangeFill](/graph/api/resources/rangefill?view=graph-rest-1.0), and [RangeFont](/graph/api/resources/rangefont?view=graph-rest-1.0) properties of a specified range.</span></span>

<span data-ttu-id="92e78-105">В результате этого набора запросов создается таблица с тремя ячейками, отформатированными так же, как три ячейки на приведенном ниже рисунке.</span><span class="sxs-lookup"><span data-stu-id="92e78-105">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Таблица-диаграмма Excel с тремя ячейками, свойства Format, Fill и Font которых были обновлены.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="92e78-107">Запрос</span><span class="sxs-lookup"><span data-stu-id="92e78-107">Request</span></span>
<span data-ttu-id="92e78-108">Этот запрос обновляет выравнивание по вертикали, высоту строк и столбцов первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="92e78-108">This request updates the vertical alignment, row height, and column height of the first cell.</span></span>


# <a name="http"></a>[<span data-ttu-id="92e78-109">HTTP</span><span class="sxs-lookup"><span data-stu-id="92e78-109">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="92e78-110">C#</span><span class="sxs-lookup"><span data-stu-id="92e78-110">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92e78-111">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92e78-111">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92e78-112">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92e78-112">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92e78-113">Java</span><span class="sxs-lookup"><span data-stu-id="92e78-113">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="92e78-114">Отклик</span><span class="sxs-lookup"><span data-stu-id="92e78-114">Response</span></span>
<span data-ttu-id="92e78-115">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92e78-115">Here is an example of the response.</span></span> <span data-ttu-id="92e78-116">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="92e78-116">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="92e78-117">Запрос</span><span class="sxs-lookup"><span data-stu-id="92e78-117">Request</span></span>
<span data-ttu-id="92e78-118">Этот запрос обновляет начертание, размер и цвет шрифта в первой ячейке.</span><span class="sxs-lookup"><span data-stu-id="92e78-118">This request updates the font style, size, and color of the first cell.</span></span>


# <a name="http"></a>[<span data-ttu-id="92e78-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="92e78-119">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="92e78-120">C#</span><span class="sxs-lookup"><span data-stu-id="92e78-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92e78-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92e78-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92e78-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92e78-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92e78-123">Java</span><span class="sxs-lookup"><span data-stu-id="92e78-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="92e78-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="92e78-124">Response</span></span>
<span data-ttu-id="92e78-125">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92e78-125">Here is an example of the response.</span></span> <span data-ttu-id="92e78-126">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="92e78-126">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="92e78-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="92e78-127">Request</span></span>
<span data-ttu-id="92e78-128">Этот запрос обновляет цвет заливки первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="92e78-128">This request updates the background color of the first cell.</span></span>


# <a name="http"></a>[<span data-ttu-id="92e78-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="92e78-129">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="92e78-130">C#</span><span class="sxs-lookup"><span data-stu-id="92e78-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92e78-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92e78-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92e78-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92e78-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92e78-133">Java</span><span class="sxs-lookup"><span data-stu-id="92e78-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="92e78-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="92e78-134">Response</span></span>
<span data-ttu-id="92e78-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92e78-135">Here is an example of the response.</span></span> <span data-ttu-id="92e78-136">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="92e78-136">Note: The response object shown here might be shortened for readability.</span></span>
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
##### <a name="request"></a><span data-ttu-id="92e78-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="92e78-137">Request</span></span>
<span data-ttu-id="92e78-138">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="92e78-138">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span>


# <a name="http"></a>[<span data-ttu-id="92e78-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="92e78-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="92e78-140">C#</span><span class="sxs-lookup"><span data-stu-id="92e78-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92e78-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92e78-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92e78-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92e78-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92e78-143">Java</span><span class="sxs-lookup"><span data-stu-id="92e78-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="92e78-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="92e78-144">Response</span></span>
<span data-ttu-id="92e78-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92e78-145">Here is an example of the response.</span></span> <span data-ttu-id="92e78-146">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="92e78-146">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="92e78-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="92e78-147">Request</span></span>
<span data-ttu-id="92e78-148">Этот запрос обновляет начертание и размер шрифта во второй ячейке.</span><span class="sxs-lookup"><span data-stu-id="92e78-148">This request updates the font style and size of the second cell.</span></span>


# <a name="http"></a>[<span data-ttu-id="92e78-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="92e78-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="92e78-150">C#</span><span class="sxs-lookup"><span data-stu-id="92e78-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92e78-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92e78-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92e78-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92e78-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92e78-153">Java</span><span class="sxs-lookup"><span data-stu-id="92e78-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="92e78-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="92e78-154">Response</span></span>
<span data-ttu-id="92e78-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92e78-155">Here is an example of the response.</span></span> <span data-ttu-id="92e78-156">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="92e78-156">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="92e78-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="92e78-157">Request</span></span>
<span data-ttu-id="92e78-158">Этот запрос обновляет цвет заливки второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="92e78-158">This request updates the background color of the second cell.</span></span>


# <a name="http"></a>[<span data-ttu-id="92e78-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="92e78-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="92e78-160">C#</span><span class="sxs-lookup"><span data-stu-id="92e78-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92e78-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92e78-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92e78-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92e78-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92e78-163">Java</span><span class="sxs-lookup"><span data-stu-id="92e78-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="92e78-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="92e78-164">Response</span></span>
<span data-ttu-id="92e78-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92e78-165">Here is an example of the response.</span></span> <span data-ttu-id="92e78-166">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="92e78-166">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="92e78-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="92e78-167">Request</span></span>
<span data-ttu-id="92e78-168">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="92e78-168">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span>


# <a name="http"></a>[<span data-ttu-id="92e78-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="92e78-169">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="92e78-170">C#</span><span class="sxs-lookup"><span data-stu-id="92e78-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92e78-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92e78-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92e78-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92e78-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92e78-173">Java</span><span class="sxs-lookup"><span data-stu-id="92e78-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="92e78-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="92e78-174">Response</span></span>
<span data-ttu-id="92e78-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92e78-175">Here is an example of the response.</span></span> <span data-ttu-id="92e78-176">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="92e78-176">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="92e78-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="92e78-177">Request</span></span>
<span data-ttu-id="92e78-178">Этот запрос обновляет начертание, размер и цвет шрифта в третьей ячейке.</span><span class="sxs-lookup"><span data-stu-id="92e78-178">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="92e78-179">Обратите внимание: свойство подчеркивания (Underline) принимает значения **Single** или **Double**.</span><span class="sxs-lookup"><span data-stu-id="92e78-179">Note that the underline property takes **Single** or **Double** as values.</span></span>


# <a name="http"></a>[<span data-ttu-id="92e78-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="92e78-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="92e78-181">C#</span><span class="sxs-lookup"><span data-stu-id="92e78-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92e78-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92e78-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92e78-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92e78-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92e78-184">Java</span><span class="sxs-lookup"><span data-stu-id="92e78-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="92e78-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="92e78-185">Response</span></span>
<span data-ttu-id="92e78-186">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92e78-186">Here is an example of the response.</span></span> <span data-ttu-id="92e78-187">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="92e78-187">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="92e78-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="92e78-188">Request</span></span>
<span data-ttu-id="92e78-189">Этот запрос обновляет цвет заливки третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="92e78-189">This request updates the background color of the third cell.</span></span>


# <a name="http"></a>[<span data-ttu-id="92e78-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="92e78-190">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="92e78-191">C#</span><span class="sxs-lookup"><span data-stu-id="92e78-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92e78-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92e78-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92e78-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92e78-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92e78-194">Java</span><span class="sxs-lookup"><span data-stu-id="92e78-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="92e78-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="92e78-195">Response</span></span>
<span data-ttu-id="92e78-196">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92e78-196">Here is an example of the response.</span></span> <span data-ttu-id="92e78-197">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="92e78-197">Note: The response object shown here might be shortened for readability.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="92e78-198">См. также</span><span class="sxs-lookup"><span data-stu-id="92e78-198">See also</span></span>
* [<span data-ttu-id="92e78-199">Управление сеансами в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="92e78-199">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="92e78-200">Запись в книгу Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="92e78-200">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="92e78-201">Использование функций книг в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="92e78-201">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="92e78-202">Показ изображения диаграммы в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="92e78-202">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="92e78-203">Использование REST API для Excel</span><span class="sxs-lookup"><span data-stu-id="92e78-203">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
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
