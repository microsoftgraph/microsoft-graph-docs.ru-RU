---
title: Обновление объекта RangeFormat
description: Обновление свойств объекта rangeformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 70b3d598923583b297028a6f9adf31abf9288452
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050390"
---
# <a name="update-rangeformat"></a><span data-ttu-id="4f6bb-103">Обновление объекта RangeFormat</span><span class="sxs-lookup"><span data-stu-id="4f6bb-103">Update rangeformat</span></span>

<span data-ttu-id="4f6bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f6bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4f6bb-105">Обновление свойств объекта rangeformat.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-105">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4f6bb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f6bb-106">Permissions</span></span>
<span data-ttu-id="4f6bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f6bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f6bb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f6bb-109">Permission type</span></span>      | <span data-ttu-id="4f6bb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f6bb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f6bb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f6bb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4f6bb-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f6bb-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4f6bb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f6bb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f6bb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-114">Not supported.</span></span>    |
|<span data-ttu-id="4f6bb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f6bb-115">Application</span></span> | <span data-ttu-id="4f6bb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f6bb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f6bb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range/format
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range/format
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="request-headers"></a><span data-ttu-id="4f6bb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f6bb-118">Request headers</span></span>
| <span data-ttu-id="4f6bb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4f6bb-119">Name</span></span>       | <span data-ttu-id="4f6bb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4f6bb-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4f6bb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f6bb-121">Authorization</span></span>  | <span data-ttu-id="4f6bb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4f6bb-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4f6bb-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="4f6bb-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f6bb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f6bb-127">Request body</span></span>
<span data-ttu-id="4f6bb-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4f6bb-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f6bb-131">Property</span></span>     | <span data-ttu-id="4f6bb-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4f6bb-132">Type</span></span>   |<span data-ttu-id="4f6bb-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4f6bb-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f6bb-134">columnWidth</span><span class="sxs-lookup"><span data-stu-id="4f6bb-134">columnWidth</span></span>|<span data-ttu-id="4f6bb-135">double</span><span class="sxs-lookup"><span data-stu-id="4f6bb-135">double</span></span>|<span data-ttu-id="4f6bb-p105">Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="4f6bb-138">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="4f6bb-138">horizontalAlignment</span></span>|<span data-ttu-id="4f6bb-139">string</span><span class="sxs-lookup"><span data-stu-id="4f6bb-139">string</span></span>|<span data-ttu-id="4f6bb-140">Представляет выравнивание по горизонтали для указанного объекта.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-140">Represents the horizontal alignment for the specified object.</span></span> <span data-ttu-id="4f6bb-141">Возможные значения: `General` `Left` , , , , , , `Center` `Right` `Fill` `Justify` `CenterAcrossSelection` `Distributed` .</span><span class="sxs-lookup"><span data-stu-id="4f6bb-141">The possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="4f6bb-142">rowHeight</span><span class="sxs-lookup"><span data-stu-id="4f6bb-142">rowHeight</span></span>|<span data-ttu-id="4f6bb-143">double</span><span class="sxs-lookup"><span data-stu-id="4f6bb-143">double</span></span>|<span data-ttu-id="4f6bb-p107">Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="4f6bb-146">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="4f6bb-146">verticalAlignment</span></span>|<span data-ttu-id="4f6bb-147">string</span><span class="sxs-lookup"><span data-stu-id="4f6bb-147">string</span></span>|<span data-ttu-id="4f6bb-148">Представляет выравнивание по вертикали для указанного объекта.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-148">Represents the vertical alignment for the specified object.</span></span> <span data-ttu-id="4f6bb-149">Допустимые значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-149">The possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="4f6bb-150">wrapText</span><span class="sxs-lookup"><span data-stu-id="4f6bb-150">wrapText</span></span>|<span data-ttu-id="4f6bb-151">boolean</span><span class="sxs-lookup"><span data-stu-id="4f6bb-151">boolean</span></span>|<span data-ttu-id="4f6bb-p109">Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="4f6bb-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6bb-154">Response</span></span>

<span data-ttu-id="4f6bb-155">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [WorkbookRangeFormat](../resources/rangeformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-155">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4f6bb-156">Пример</span><span class="sxs-lookup"><span data-stu-id="4f6bb-156">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="4f6bb-157">Обновляет свойства Format, Fill и Font в трех ячейках таблицы</span><span class="sxs-lookup"><span data-stu-id="4f6bb-157">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="4f6bb-158">В следующих примерах показано, как обновлять свойства свойств [Свойств WorkbookRangeFormat,](../resources/rangeformat.md) [WorkbookRangeFill](../resources/rangefill.md)и [WorkbookRangeFont](../resources/rangefont.md) указанного диапазона.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-158">The following examples demonstrate how to update properties of the [WorkbookRangeFormat](../resources/rangeformat.md), [WorkbookRangeFill](../resources/rangefill.md), and [WorkbookRangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="4f6bb-159">В результате этого набора запросов создается таблица с тремя ячейками, отформатированными так же, как три ячейки на приведенном ниже рисунке.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-159">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Таблица-диаграмма Excel с тремя ячейками, свойства Format, Fill и Font которых были обновлены.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="4f6bb-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6bb-161">Request</span></span>
<span data-ttu-id="4f6bb-162">Этот запрос обновляет выравнивание по вертикали, высоту строк и столбцов первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-162">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="4f6bb-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f6bb-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
# <a name="c"></a>[<span data-ttu-id="4f6bb-164">C#</span><span class="sxs-lookup"><span data-stu-id="4f6bb-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f6bb-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f6bb-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f6bb-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f6bb-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f6bb-167">Java</span><span class="sxs-lookup"><span data-stu-id="4f6bb-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4f6bb-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6bb-168">Response</span></span>
<span data-ttu-id="4f6bb-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-169">Here is an example of the response.</span></span> <span data-ttu-id="4f6bb-170">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-170">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="4f6bb-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6bb-171">Request</span></span>
<span data-ttu-id="4f6bb-172">Этот запрос обновляет начертание, размер и цвет шрифта в первой ячейке.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-172">This request updates the font style, size, and color of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="4f6bb-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f6bb-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format/font
Content-type: application/json

{
  "bold": true,
  "color": "#4B180E",
  "size": 26
}
```
# <a name="c"></a>[<span data-ttu-id="4f6bb-174">C#</span><span class="sxs-lookup"><span data-stu-id="4f6bb-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f6bb-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f6bb-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f6bb-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f6bb-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f6bb-177">Java</span><span class="sxs-lookup"><span data-stu-id="4f6bb-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4f6bb-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6bb-178">Response</span></span>
<span data-ttu-id="4f6bb-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-179">Here is an example of the response.</span></span> <span data-ttu-id="4f6bb-180">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-180">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="4f6bb-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6bb-181">Request</span></span>
<span data-ttu-id="4f6bb-182">Этот запрос обновляет цвет заливки первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-182">This request updates the background color of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="4f6bb-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f6bb-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
# <a name="c"></a>[<span data-ttu-id="4f6bb-184">C#</span><span class="sxs-lookup"><span data-stu-id="4f6bb-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f6bb-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f6bb-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f6bb-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f6bb-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f6bb-187">Java</span><span class="sxs-lookup"><span data-stu-id="4f6bb-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4f6bb-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6bb-188">Response</span></span>
<span data-ttu-id="4f6bb-189">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-189">Here is an example of the response.</span></span> <span data-ttu-id="4f6bb-190">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-190">Note: The response object shown here might be shortened for readability.</span></span>
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
##### <a name="request"></a><span data-ttu-id="4f6bb-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6bb-191">Request</span></span>
<span data-ttu-id="4f6bb-192">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-192">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="4f6bb-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f6bb-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Center",
  "verticalAlignment": "Center",
  "rowHeight": 49,
  "wrapText": false
}
```
# <a name="c"></a>[<span data-ttu-id="4f6bb-194">C#</span><span class="sxs-lookup"><span data-stu-id="4f6bb-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f6bb-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f6bb-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f6bb-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f6bb-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f6bb-197">Java</span><span class="sxs-lookup"><span data-stu-id="4f6bb-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4f6bb-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6bb-198">Response</span></span>
<span data-ttu-id="4f6bb-199">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-199">Here is an example of the response.</span></span> <span data-ttu-id="4f6bb-200">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-200">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="4f6bb-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6bb-201">Request</span></span>
<span data-ttu-id="4f6bb-202">Этот запрос обновляет начертание и размер шрифта во второй ячейке.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-202">This request updates the font style and size of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="4f6bb-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f6bb-203">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format/font
Content-type: application/json

{
  "italic": true,
  "size": 26
}
```
# <a name="c"></a>[<span data-ttu-id="4f6bb-204">C#</span><span class="sxs-lookup"><span data-stu-id="4f6bb-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f6bb-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f6bb-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f6bb-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f6bb-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f6bb-207">Java</span><span class="sxs-lookup"><span data-stu-id="4f6bb-207">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4f6bb-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6bb-208">Response</span></span>
<span data-ttu-id="4f6bb-209">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-209">Here is an example of the response.</span></span> <span data-ttu-id="4f6bb-210">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-210">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="4f6bb-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6bb-211">Request</span></span>
<span data-ttu-id="4f6bb-212">Этот запрос обновляет цвет заливки второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-212">This request updates the background color of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="4f6bb-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f6bb-213">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
# <a name="c"></a>[<span data-ttu-id="4f6bb-214">C#</span><span class="sxs-lookup"><span data-stu-id="4f6bb-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f6bb-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f6bb-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f6bb-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f6bb-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f6bb-217">Java</span><span class="sxs-lookup"><span data-stu-id="4f6bb-217">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4f6bb-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6bb-218">Response</span></span>
<span data-ttu-id="4f6bb-219">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-219">Here is an example of the response.</span></span> <span data-ttu-id="4f6bb-220">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-220">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="4f6bb-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6bb-221">Request</span></span>
<span data-ttu-id="4f6bb-222">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-222">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="4f6bb-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f6bb-223">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Right",
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
# <a name="c"></a>[<span data-ttu-id="4f6bb-224">C#</span><span class="sxs-lookup"><span data-stu-id="4f6bb-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f6bb-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f6bb-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f6bb-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f6bb-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f6bb-227">Java</span><span class="sxs-lookup"><span data-stu-id="4f6bb-227">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4f6bb-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6bb-228">Response</span></span>
<span data-ttu-id="4f6bb-229">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-229">Here is an example of the response.</span></span> <span data-ttu-id="4f6bb-230">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-230">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="4f6bb-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6bb-231">Request</span></span>
<span data-ttu-id="4f6bb-232">Этот запрос обновляет начертание, размер и цвет шрифта в третьей ячейке.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-232">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="4f6bb-233">Обратите внимание: свойство подчеркивания (Underline) принимает значения **Single** или **Double**.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-233">Note that the underline property takes **Single** or **Double** as values.</span></span>


# <a name="http"></a>[<span data-ttu-id="4f6bb-234">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f6bb-234">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format/font
Content-type: application/json

{
  "underline": "Single",
  "color": "#FFFFFF",
  "size": 26
}
```
# <a name="c"></a>[<span data-ttu-id="4f6bb-235">C#</span><span class="sxs-lookup"><span data-stu-id="4f6bb-235">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f6bb-236">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f6bb-236">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f6bb-237">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f6bb-237">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f6bb-238">Java</span><span class="sxs-lookup"><span data-stu-id="4f6bb-238">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4f6bb-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6bb-239">Response</span></span>
<span data-ttu-id="4f6bb-240">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-240">Here is an example of the response.</span></span> <span data-ttu-id="4f6bb-241">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-241">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="4f6bb-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6bb-242">Request</span></span>
<span data-ttu-id="4f6bb-243">Этот запрос обновляет цвет заливки третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-243">This request updates the background color of the third cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="4f6bb-244">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f6bb-244">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
# <a name="c"></a>[<span data-ttu-id="4f6bb-245">C#</span><span class="sxs-lookup"><span data-stu-id="4f6bb-245">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f6bb-246">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f6bb-246">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f6bb-247">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f6bb-247">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f6bb-248">Java</span><span class="sxs-lookup"><span data-stu-id="4f6bb-248">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4f6bb-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6bb-249">Response</span></span>
<span data-ttu-id="4f6bb-250">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-250">Here is an example of the response.</span></span> <span data-ttu-id="4f6bb-251">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4f6bb-251">Note: The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: update_rangeformat_font_three/underline:
      Expected type String but actual was Single. Property: underline, actual value: 'Single'"
  ],
  "tocPath": ""
}-->

