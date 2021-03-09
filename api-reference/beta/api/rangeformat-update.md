---
title: Обновление объекта RangeFormat
description: Обновление свойств объекта rangeformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 745eeb59d12ad3a779a8769095a5a3125cada813
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577445"
---
# <a name="update-rangeformat"></a><span data-ttu-id="5c634-103">Обновление объекта RangeFormat</span><span class="sxs-lookup"><span data-stu-id="5c634-103">Update rangeformat</span></span>

<span data-ttu-id="5c634-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c634-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c634-105">Обновление свойств объекта rangeformat.</span><span class="sxs-lookup"><span data-stu-id="5c634-105">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5c634-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c634-106">Permissions</span></span>
<span data-ttu-id="5c634-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c634-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c634-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c634-109">Permission type</span></span>      | <span data-ttu-id="5c634-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c634-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c634-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c634-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5c634-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c634-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5c634-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c634-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c634-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c634-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5c634-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c634-115">Application</span></span> | <span data-ttu-id="5c634-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c634-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c634-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c634-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range/format
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range/format
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="5c634-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c634-118">Optional request headers</span></span>
| <span data-ttu-id="5c634-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5c634-119">Name</span></span>       | <span data-ttu-id="5c634-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5c634-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5c634-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c634-121">Authorization</span></span>  | <span data-ttu-id="5c634-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c634-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5c634-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5c634-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="5c634-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="5c634-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c634-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c634-127">Request body</span></span>
<span data-ttu-id="5c634-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5c634-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5c634-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c634-131">Property</span></span>     | <span data-ttu-id="5c634-132">Тип</span><span class="sxs-lookup"><span data-stu-id="5c634-132">Type</span></span>   |<span data-ttu-id="5c634-133">Описание</span><span class="sxs-lookup"><span data-stu-id="5c634-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c634-134">columnWidth</span><span class="sxs-lookup"><span data-stu-id="5c634-134">columnWidth</span></span>|<span data-ttu-id="5c634-135">double</span><span class="sxs-lookup"><span data-stu-id="5c634-135">double</span></span>|<span data-ttu-id="5c634-p105">Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="5c634-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="5c634-138">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="5c634-138">horizontalAlignment</span></span>|<span data-ttu-id="5c634-139">string</span><span class="sxs-lookup"><span data-stu-id="5c634-139">string</span></span>|<span data-ttu-id="5c634-p106">Представляет горизонтальное выравнивание для указанного объекта. Возможные значения: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="5c634-p106">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="5c634-142">rowHeight</span><span class="sxs-lookup"><span data-stu-id="5c634-142">rowHeight</span></span>|<span data-ttu-id="5c634-143">double</span><span class="sxs-lookup"><span data-stu-id="5c634-143">double</span></span>|<span data-ttu-id="5c634-p107">Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="5c634-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="5c634-146">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="5c634-146">verticalAlignment</span></span>|<span data-ttu-id="5c634-147">string</span><span class="sxs-lookup"><span data-stu-id="5c634-147">string</span></span>|<span data-ttu-id="5c634-p108">Представляет вертикальное выравнивание для указанного объекта. Возможные значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="5c634-p108">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="5c634-150">wrapText</span><span class="sxs-lookup"><span data-stu-id="5c634-150">wrapText</span></span>|<span data-ttu-id="5c634-151">boolean</span><span class="sxs-lookup"><span data-stu-id="5c634-151">boolean</span></span>|<span data-ttu-id="5c634-p109">Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.</span><span class="sxs-lookup"><span data-stu-id="5c634-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="5c634-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c634-154">Response</span></span>

<span data-ttu-id="5c634-155">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [workbookRangeFormat](../resources/workbookrangeformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5c634-155">If successful, this method returns a `200 OK` response code and updated [workbookRangeFormat](../resources/workbookrangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5c634-156">Пример</span><span class="sxs-lookup"><span data-stu-id="5c634-156">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="5c634-157">Обновляет свойства Format, Fill и Font в трех ячейках таблицы</span><span class="sxs-lookup"><span data-stu-id="5c634-157">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="5c634-158">В следующих примерах показано, как обновлять свойства свойств [книгиRangeFormat,](../resources/workbookrangeformat.md) [workbookRangeFill](../resources/workbookrangefill.md)и свойств [книгиRangeFont](../resources/workbookrangefont.md) указанного диапазона.</span><span class="sxs-lookup"><span data-stu-id="5c634-158">The following examples demonstrate how to update properties of the [workbookRangeFormat](../resources/workbookrangeformat.md), [workbookRangeFill](../resources/workbookrangefill.md), and [workbookRangeFont](../resources/workbookrangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="5c634-159">В результате этого набора запросов создается таблица с тремя ячейками, отформатированными так же, как три ячейки на приведенном ниже рисунке.</span><span class="sxs-lookup"><span data-stu-id="5c634-159">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Таблица-диаграмма Excel с тремя ячейками, свойства Format, Fill и Font которых были обновлены.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="5c634-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c634-161">Request</span></span>
<span data-ttu-id="5c634-162">Этот запрос обновляет выравнивание по вертикали, высоту строк и столбцов первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="5c634-162">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5c634-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c634-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5c634-164">C#</span><span class="sxs-lookup"><span data-stu-id="5c634-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c634-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c634-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c634-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c634-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c634-167">Java</span><span class="sxs-lookup"><span data-stu-id="5c634-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c634-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c634-168">Response</span></span>
<span data-ttu-id="5c634-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5c634-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="5c634-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c634-172">Request</span></span>
<span data-ttu-id="5c634-173">Этот запрос обновляет начертание, размер и цвет шрифта в первой ячейке.</span><span class="sxs-lookup"><span data-stu-id="5c634-173">This request updates the font style, size, and color of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5c634-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c634-174">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5c634-175">C#</span><span class="sxs-lookup"><span data-stu-id="5c634-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c634-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c634-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c634-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c634-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c634-178">Java</span><span class="sxs-lookup"><span data-stu-id="5c634-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c634-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c634-179">Response</span></span>
<span data-ttu-id="5c634-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5c634-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="5c634-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c634-183">Request</span></span>
<span data-ttu-id="5c634-184">Этот запрос обновляет цвет заливки первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="5c634-184">This request updates the background color of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5c634-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c634-185">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5c634-186">C#</span><span class="sxs-lookup"><span data-stu-id="5c634-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c634-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c634-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c634-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c634-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c634-189">Java</span><span class="sxs-lookup"><span data-stu-id="5c634-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c634-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c634-190">Response</span></span>
<span data-ttu-id="5c634-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5c634-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="5c634-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c634-194">Request</span></span>
<span data-ttu-id="5c634-195">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="5c634-195">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5c634-196">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c634-196">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5c634-197">C#</span><span class="sxs-lookup"><span data-stu-id="5c634-197">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c634-198">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c634-198">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c634-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c634-199">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c634-200">Java</span><span class="sxs-lookup"><span data-stu-id="5c634-200">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c634-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c634-201">Response</span></span>
<span data-ttu-id="5c634-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5c634-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="5c634-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c634-205">Request</span></span>
<span data-ttu-id="5c634-206">Этот запрос обновляет начертание и размер шрифта во второй ячейке.</span><span class="sxs-lookup"><span data-stu-id="5c634-206">This request updates the font style and size of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5c634-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c634-207">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5c634-208">C#</span><span class="sxs-lookup"><span data-stu-id="5c634-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c634-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c634-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c634-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c634-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c634-211">Java</span><span class="sxs-lookup"><span data-stu-id="5c634-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c634-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c634-212">Response</span></span>
<span data-ttu-id="5c634-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5c634-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="5c634-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c634-216">Request</span></span>
<span data-ttu-id="5c634-217">Этот запрос обновляет цвет заливки второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="5c634-217">This request updates the background color of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5c634-218">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c634-218">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5c634-219">C#</span><span class="sxs-lookup"><span data-stu-id="5c634-219">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c634-220">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c634-220">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c634-221">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c634-221">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c634-222">Java</span><span class="sxs-lookup"><span data-stu-id="5c634-222">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c634-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c634-223">Response</span></span>
<span data-ttu-id="5c634-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5c634-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="5c634-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c634-227">Request</span></span>
<span data-ttu-id="5c634-228">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="5c634-228">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5c634-229">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c634-229">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5c634-230">C#</span><span class="sxs-lookup"><span data-stu-id="5c634-230">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c634-231">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c634-231">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c634-232">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c634-232">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c634-233">Java</span><span class="sxs-lookup"><span data-stu-id="5c634-233">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c634-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c634-234">Response</span></span>
<span data-ttu-id="5c634-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5c634-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="5c634-238">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c634-238">Request</span></span>
<span data-ttu-id="5c634-239">Этот запрос обновляет начертание, размер и цвет шрифта в третьей ячейке.</span><span class="sxs-lookup"><span data-stu-id="5c634-239">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="5c634-240">Обратите внимание: свойство подчеркивания (Underline) принимает значения **Single** или **Double**.</span><span class="sxs-lookup"><span data-stu-id="5c634-240">Note that the underline property takes **Single** or **Double** as values.</span></span>


# <a name="http"></a>[<span data-ttu-id="5c634-241">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c634-241">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5c634-242">C#</span><span class="sxs-lookup"><span data-stu-id="5c634-242">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c634-243">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c634-243">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c634-244">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c634-244">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c634-245">Java</span><span class="sxs-lookup"><span data-stu-id="5c634-245">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c634-246">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c634-246">Response</span></span>
<span data-ttu-id="5c634-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5c634-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="5c634-250">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c634-250">Request</span></span>
<span data-ttu-id="5c634-251">Этот запрос обновляет цвет заливки третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="5c634-251">This request updates the background color of the third cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="5c634-252">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c634-252">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5c634-253">C#</span><span class="sxs-lookup"><span data-stu-id="5c634-253">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c634-254">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c634-254">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c634-255">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c634-255">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c634-256">Java</span><span class="sxs-lookup"><span data-stu-id="5c634-256">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c634-257">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c634-257">Response</span></span>
<span data-ttu-id="5c634-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c634-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


