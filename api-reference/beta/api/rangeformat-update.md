---
title: Обновление объекта RangeFormat
description: Обновление свойств объекта rangeformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7a0605195d10cd1a50a99d71280f47881650f7d7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978289"
---
# <a name="update-rangeformat"></a><span data-ttu-id="82e8f-103">Обновление объекта RangeFormat</span><span class="sxs-lookup"><span data-stu-id="82e8f-103">Update rangeformat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82e8f-104">Обновление свойств объекта rangeformat.</span><span class="sxs-lookup"><span data-stu-id="82e8f-104">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="82e8f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82e8f-105">Permissions</span></span>
<span data-ttu-id="82e8f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82e8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82e8f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82e8f-108">Permission type</span></span>      | <span data-ttu-id="82e8f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82e8f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82e8f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82e8f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="82e8f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82e8f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="82e8f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82e8f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82e8f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82e8f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="82e8f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82e8f-114">Application</span></span> | <span data-ttu-id="82e8f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82e8f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82e8f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82e8f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="82e8f-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82e8f-117">Optional request headers</span></span>
| <span data-ttu-id="82e8f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="82e8f-118">Name</span></span>       | <span data-ttu-id="82e8f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="82e8f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="82e8f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82e8f-120">Authorization</span></span>  | <span data-ttu-id="82e8f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82e8f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="82e8f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="82e8f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="82e8f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="82e8f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82e8f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="82e8f-126">Request body</span></span>
<span data-ttu-id="82e8f-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="82e8f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="82e8f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="82e8f-130">Property</span></span>     | <span data-ttu-id="82e8f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="82e8f-131">Type</span></span>   |<span data-ttu-id="82e8f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="82e8f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82e8f-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="82e8f-133">columnWidth</span></span>|<span data-ttu-id="82e8f-134">double</span><span class="sxs-lookup"><span data-stu-id="82e8f-134">double</span></span>|<span data-ttu-id="82e8f-p105">Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="82e8f-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="82e8f-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="82e8f-137">horizontalAlignment</span></span>|<span data-ttu-id="82e8f-138">string</span><span class="sxs-lookup"><span data-stu-id="82e8f-138">string</span></span>|<span data-ttu-id="82e8f-p106">Представляет горизонтальное выравнивание для указанного объекта. Возможные значения: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="82e8f-p106">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="82e8f-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="82e8f-141">rowHeight</span></span>|<span data-ttu-id="82e8f-142">double</span><span class="sxs-lookup"><span data-stu-id="82e8f-142">double</span></span>|<span data-ttu-id="82e8f-p107">Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="82e8f-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="82e8f-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="82e8f-145">verticalAlignment</span></span>|<span data-ttu-id="82e8f-146">string</span><span class="sxs-lookup"><span data-stu-id="82e8f-146">string</span></span>|<span data-ttu-id="82e8f-p108">Представляет вертикальное выравнивание для указанного объекта. Возможные значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="82e8f-p108">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="82e8f-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="82e8f-149">wrapText</span></span>|<span data-ttu-id="82e8f-150">boolean</span><span class="sxs-lookup"><span data-stu-id="82e8f-150">boolean</span></span>|<span data-ttu-id="82e8f-p109">Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.</span><span class="sxs-lookup"><span data-stu-id="82e8f-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="82e8f-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="82e8f-153">Response</span></span>

<span data-ttu-id="82e8f-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукранжеформат](../resources/workbookrangeformat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82e8f-154">If successful, this method returns a `200 OK` response code and updated [workbookRangeFormat](../resources/workbookrangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="82e8f-155">Пример</span><span class="sxs-lookup"><span data-stu-id="82e8f-155">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="82e8f-156">Обновляет свойства Format, Fill и Font в трех ячейках таблицы</span><span class="sxs-lookup"><span data-stu-id="82e8f-156">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="82e8f-157">В следующих примерах показано, как обновить свойства [воркбукранжеформат](../resources/workbookrangeformat.md), [воркбукранжефилл](../resources/workbookrangefill.md)и [воркбукранжефонт](../resources/workbookrangefont.md) указанного диапазона.</span><span class="sxs-lookup"><span data-stu-id="82e8f-157">The following examples demonstrate how to update properties of the [workbookRangeFormat](../resources/workbookrangeformat.md), [workbookRangeFill](../resources/workbookrangefill.md), and [workbookRangeFont](../resources/workbookrangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="82e8f-158">В результате этого набора запросов создается таблица с тремя ячейками, отформатированными так же, как три ячейки на приведенном ниже рисунке.</span><span class="sxs-lookup"><span data-stu-id="82e8f-158">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Таблица-диаграмма Excel с тремя ячейками, свойства Format, Fill и Font которых были обновлены.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="82e8f-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="82e8f-160">Request</span></span>
<span data-ttu-id="82e8f-161">Этот запрос обновляет выравнивание по вертикали, высоту строк и столбцов первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="82e8f-161">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="82e8f-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="82e8f-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82e8f-163">C#</span><span class="sxs-lookup"><span data-stu-id="82e8f-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82e8f-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="82e8f-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82e8f-165">Цель — C</span><span class="sxs-lookup"><span data-stu-id="82e8f-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="82e8f-166">Java</span><span class="sxs-lookup"><span data-stu-id="82e8f-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="82e8f-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="82e8f-167">Response</span></span>
<span data-ttu-id="82e8f-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82e8f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="82e8f-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="82e8f-171">Request</span></span>
<span data-ttu-id="82e8f-172">Этот запрос обновляет начертание, размер и цвет шрифта в первой ячейке.</span><span class="sxs-lookup"><span data-stu-id="82e8f-172">This request updates the font style, size, and color of the first cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="82e8f-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="82e8f-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/font
Content-type: application/json

{
  "bold": true,
  "color": "#4B180E",
  "size": 26
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82e8f-174">C#</span><span class="sxs-lookup"><span data-stu-id="82e8f-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82e8f-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="82e8f-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82e8f-176">Цель — C</span><span class="sxs-lookup"><span data-stu-id="82e8f-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="82e8f-177">Java</span><span class="sxs-lookup"><span data-stu-id="82e8f-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="82e8f-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="82e8f-178">Response</span></span>
<span data-ttu-id="82e8f-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82e8f-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="82e8f-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="82e8f-182">Request</span></span>
<span data-ttu-id="82e8f-183">Этот запрос обновляет цвет заливки первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="82e8f-183">This request updates the background color of the first cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="82e8f-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="82e8f-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82e8f-185">C#</span><span class="sxs-lookup"><span data-stu-id="82e8f-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82e8f-186">Javascript</span><span class="sxs-lookup"><span data-stu-id="82e8f-186">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82e8f-187">Цель — C</span><span class="sxs-lookup"><span data-stu-id="82e8f-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="82e8f-188">Java</span><span class="sxs-lookup"><span data-stu-id="82e8f-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="82e8f-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="82e8f-189">Response</span></span>
<span data-ttu-id="82e8f-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82e8f-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="82e8f-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="82e8f-193">Request</span></span>
<span data-ttu-id="82e8f-194">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="82e8f-194">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="82e8f-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="82e8f-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_two"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Center",
  "verticalAlignment": "Center",
  "rowHeight": 49,
  "wrapText": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82e8f-196">C#</span><span class="sxs-lookup"><span data-stu-id="82e8f-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82e8f-197">Javascript</span><span class="sxs-lookup"><span data-stu-id="82e8f-197">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82e8f-198">Цель — C</span><span class="sxs-lookup"><span data-stu-id="82e8f-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="82e8f-199">Java</span><span class="sxs-lookup"><span data-stu-id="82e8f-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="82e8f-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="82e8f-200">Response</span></span>
<span data-ttu-id="82e8f-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82e8f-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="82e8f-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="82e8f-204">Request</span></span>
<span data-ttu-id="82e8f-205">Этот запрос обновляет начертание и размер шрифта во второй ячейке.</span><span class="sxs-lookup"><span data-stu-id="82e8f-205">This request updates the font style and size of the second cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="82e8f-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="82e8f-206">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_two"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/font
Content-type: application/json

{
  "italic": true,
  "size": 26
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82e8f-207">C#</span><span class="sxs-lookup"><span data-stu-id="82e8f-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82e8f-208">Javascript</span><span class="sxs-lookup"><span data-stu-id="82e8f-208">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82e8f-209">Цель — C</span><span class="sxs-lookup"><span data-stu-id="82e8f-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="82e8f-210">Java</span><span class="sxs-lookup"><span data-stu-id="82e8f-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="82e8f-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="82e8f-211">Response</span></span>
<span data-ttu-id="82e8f-p114">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82e8f-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="82e8f-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="82e8f-215">Request</span></span>
<span data-ttu-id="82e8f-216">Этот запрос обновляет цвет заливки второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="82e8f-216">This request updates the background color of the second cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="82e8f-217">HTTP</span><span class="sxs-lookup"><span data-stu-id="82e8f-217">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82e8f-218">C#</span><span class="sxs-lookup"><span data-stu-id="82e8f-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82e8f-219">Javascript</span><span class="sxs-lookup"><span data-stu-id="82e8f-219">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82e8f-220">Цель — C</span><span class="sxs-lookup"><span data-stu-id="82e8f-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="82e8f-221">Java</span><span class="sxs-lookup"><span data-stu-id="82e8f-221">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="82e8f-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="82e8f-222">Response</span></span>
<span data-ttu-id="82e8f-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82e8f-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="82e8f-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="82e8f-226">Request</span></span>
<span data-ttu-id="82e8f-227">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="82e8f-227">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="82e8f-228">HTTP</span><span class="sxs-lookup"><span data-stu-id="82e8f-228">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_three"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Right",
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82e8f-229">C#</span><span class="sxs-lookup"><span data-stu-id="82e8f-229">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82e8f-230">Javascript</span><span class="sxs-lookup"><span data-stu-id="82e8f-230">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82e8f-231">Цель — C</span><span class="sxs-lookup"><span data-stu-id="82e8f-231">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="82e8f-232">Java</span><span class="sxs-lookup"><span data-stu-id="82e8f-232">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="82e8f-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="82e8f-233">Response</span></span>
<span data-ttu-id="82e8f-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82e8f-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="82e8f-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="82e8f-237">Request</span></span>
<span data-ttu-id="82e8f-238">Этот запрос обновляет начертание, размер и цвет шрифта в третьей ячейке.</span><span class="sxs-lookup"><span data-stu-id="82e8f-238">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="82e8f-239">Обратите внимание: свойство подчеркивания (Underline) принимает значения **Single** или **Double**.</span><span class="sxs-lookup"><span data-stu-id="82e8f-239">Note that the underline property takes **Single** or **Double** as values.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="82e8f-240">HTTP</span><span class="sxs-lookup"><span data-stu-id="82e8f-240">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_three"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/font
Content-type: application/json

{
  "underline": "Single",
  "color": "#FFFFFF",
  "size": 26
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82e8f-241">C#</span><span class="sxs-lookup"><span data-stu-id="82e8f-241">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82e8f-242">Javascript</span><span class="sxs-lookup"><span data-stu-id="82e8f-242">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82e8f-243">Цель — C</span><span class="sxs-lookup"><span data-stu-id="82e8f-243">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="82e8f-244">Java</span><span class="sxs-lookup"><span data-stu-id="82e8f-244">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="82e8f-245">Отклик</span><span class="sxs-lookup"><span data-stu-id="82e8f-245">Response</span></span>
<span data-ttu-id="82e8f-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82e8f-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="82e8f-249">Запрос</span><span class="sxs-lookup"><span data-stu-id="82e8f-249">Request</span></span>
<span data-ttu-id="82e8f-250">Этот запрос обновляет цвет заливки третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="82e8f-250">This request updates the background color of the third cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="82e8f-251">HTTP</span><span class="sxs-lookup"><span data-stu-id="82e8f-251">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82e8f-252">C#</span><span class="sxs-lookup"><span data-stu-id="82e8f-252">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82e8f-253">Javascript</span><span class="sxs-lookup"><span data-stu-id="82e8f-253">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82e8f-254">Цель — C</span><span class="sxs-lookup"><span data-stu-id="82e8f-254">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="82e8f-255">Java</span><span class="sxs-lookup"><span data-stu-id="82e8f-255">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="82e8f-256">Отклик</span><span class="sxs-lookup"><span data-stu-id="82e8f-256">Response</span></span>
<span data-ttu-id="82e8f-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82e8f-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: update_rangeformat_font_three/underline:\r\n       Expected type String but actual was Single. Property: underline, actual value: 'Single'"
  ]
}
-->
