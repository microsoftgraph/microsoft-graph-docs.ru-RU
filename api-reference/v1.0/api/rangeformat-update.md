---
title: Обновление объекта RangeFormat
description: Обновление свойств объекта rangeformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 31023749e119722c0f393fe8def05edf2a3e23a4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263625"
---
# <a name="update-rangeformat"></a><span data-ttu-id="d3912-103">Обновление объекта RangeFormat</span><span class="sxs-lookup"><span data-stu-id="d3912-103">Update rangeformat</span></span>

<span data-ttu-id="d3912-104">Обновление свойств объекта rangeformat.</span><span class="sxs-lookup"><span data-stu-id="d3912-104">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d3912-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3912-105">Permissions</span></span>
<span data-ttu-id="d3912-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3912-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3912-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3912-108">Permission type</span></span>      | <span data-ttu-id="d3912-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3912-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3912-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3912-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d3912-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3912-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d3912-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3912-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3912-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3912-113">Not supported.</span></span>    |
|<span data-ttu-id="d3912-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3912-114">Application</span></span> | <span data-ttu-id="d3912-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3912-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3912-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3912-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="request-headers"></a><span data-ttu-id="d3912-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3912-117">Request headers</span></span>
| <span data-ttu-id="d3912-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d3912-118">Name</span></span>       | <span data-ttu-id="d3912-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d3912-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d3912-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3912-120">Authorization</span></span>  | <span data-ttu-id="d3912-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3912-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d3912-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d3912-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d3912-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d3912-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3912-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d3912-126">Request body</span></span>
<span data-ttu-id="d3912-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d3912-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d3912-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3912-130">Property</span></span>     | <span data-ttu-id="d3912-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d3912-131">Type</span></span>   |<span data-ttu-id="d3912-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d3912-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3912-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="d3912-133">columnWidth</span></span>|<span data-ttu-id="d3912-134">double</span><span class="sxs-lookup"><span data-stu-id="d3912-134">double</span></span>|<span data-ttu-id="d3912-p105">Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="d3912-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="d3912-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="d3912-137">horizontalAlignment</span></span>|<span data-ttu-id="d3912-138">string</span><span class="sxs-lookup"><span data-stu-id="d3912-138">string</span></span>|<span data-ttu-id="d3912-139">Представляет выравнивание по горизонтали для указанного объекта.</span><span class="sxs-lookup"><span data-stu-id="d3912-139">Represents the horizontal alignment for the specified object.</span></span> <span data-ttu-id="d3912-140">Возможные `General`значения:, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`,. `Distributed`</span><span class="sxs-lookup"><span data-stu-id="d3912-140">The possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="d3912-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="d3912-141">rowHeight</span></span>|<span data-ttu-id="d3912-142">double</span><span class="sxs-lookup"><span data-stu-id="d3912-142">double</span></span>|<span data-ttu-id="d3912-p107">Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="d3912-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="d3912-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="d3912-145">verticalAlignment</span></span>|<span data-ttu-id="d3912-146">string</span><span class="sxs-lookup"><span data-stu-id="d3912-146">string</span></span>|<span data-ttu-id="d3912-147">Представляет выравнивание по вертикали для указанного объекта.</span><span class="sxs-lookup"><span data-stu-id="d3912-147">Represents the vertical alignment for the specified object.</span></span> <span data-ttu-id="d3912-148">Допустимые значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="d3912-148">The possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="d3912-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="d3912-149">wrapText</span></span>|<span data-ttu-id="d3912-150">boolean</span><span class="sxs-lookup"><span data-stu-id="d3912-150">boolean</span></span>|<span data-ttu-id="d3912-p109">Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.</span><span class="sxs-lookup"><span data-stu-id="d3912-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="d3912-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3912-153">Response</span></span>

<span data-ttu-id="d3912-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукранжеформат](../resources/rangeformat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3912-154">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d3912-155">Пример</span><span class="sxs-lookup"><span data-stu-id="d3912-155">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="d3912-156">Обновляет свойства Format, Fill и Font в трех ячейках таблицы</span><span class="sxs-lookup"><span data-stu-id="d3912-156">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="d3912-157">В следующих примерах показано, как обновить свойства [воркбукранжеформат](../resources/rangeformat.md), [воркбукранжефилл](../resources/rangefill.md)и [воркбукранжефонт](../resources/rangefont.md) указанного диапазона.</span><span class="sxs-lookup"><span data-stu-id="d3912-157">The following examples demonstrate how to update properties of the [WorkbookRangeFormat](../resources/rangeformat.md), [WorkbookRangeFill](../resources/rangefill.md), and [WorkbookRangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="d3912-158">В результате этого набора запросов создается таблица с тремя ячейками, отформатированными так же, как три ячейки на приведенном ниже рисунке.</span><span class="sxs-lookup"><span data-stu-id="d3912-158">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Таблица-диаграмма Excel с тремя ячейками, свойства Format, Fill и Font которых были обновлены.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="d3912-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3912-160">Request</span></span>
<span data-ttu-id="d3912-161">Этот запрос обновляет выравнивание по вертикали, высоту строк и столбцов первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="d3912-161">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="d3912-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3912-162">Response</span></span>
<span data-ttu-id="d3912-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3912-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3912-166">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d3912-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3912-167">C#</span><span class="sxs-lookup"><span data-stu-id="d3912-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3912-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3912-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d3912-169">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d3912-169">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="d3912-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3912-170">Request</span></span>
<span data-ttu-id="d3912-171">Этот запрос обновляет начертание, размер и цвет шрифта в первой ячейке.</span><span class="sxs-lookup"><span data-stu-id="d3912-171">This request updates the font style, size, and color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="d3912-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3912-172">Response</span></span>
<span data-ttu-id="d3912-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3912-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3912-176">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d3912-176">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3912-177">C#</span><span class="sxs-lookup"><span data-stu-id="d3912-177">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3912-178">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3912-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d3912-179">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d3912-179">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_font-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="d3912-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3912-180">Request</span></span>
<span data-ttu-id="d3912-181">Этот запрос обновляет цвет заливки первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="d3912-181">This request updates the background color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="d3912-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3912-182">Response</span></span>
<span data-ttu-id="d3912-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3912-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3912-186">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d3912-186">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3912-187">C#</span><span class="sxs-lookup"><span data-stu-id="d3912-187">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3912-188">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3912-188">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d3912-189">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d3912-189">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
##### <a name="request"></a><span data-ttu-id="d3912-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3912-190">Request</span></span>
<span data-ttu-id="d3912-191">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="d3912-191">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="d3912-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3912-192">Response</span></span>
<span data-ttu-id="d3912-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3912-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3912-196">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d3912-196">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3912-197">C#</span><span class="sxs-lookup"><span data-stu-id="d3912-197">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3912-198">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3912-198">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_two-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d3912-199">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d3912-199">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_two-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="d3912-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3912-200">Request</span></span>
<span data-ttu-id="d3912-201">Этот запрос обновляет начертание и размер шрифта во второй ячейке.</span><span class="sxs-lookup"><span data-stu-id="d3912-201">This request updates the font style and size of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="d3912-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3912-202">Response</span></span>
<span data-ttu-id="d3912-p114">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3912-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3912-206">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d3912-206">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3912-207">C#</span><span class="sxs-lookup"><span data-stu-id="d3912-207">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3912-208">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3912-208">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_two-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d3912-209">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d3912-209">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_two-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="d3912-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3912-210">Request</span></span>
<span data-ttu-id="d3912-211">Этот запрос обновляет цвет заливки второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="d3912-211">This request updates the background color of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="d3912-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3912-212">Response</span></span>
<span data-ttu-id="d3912-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3912-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3912-216">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d3912-216">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3912-217">C#</span><span class="sxs-lookup"><span data-stu-id="d3912-217">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3912-218">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3912-218">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_two-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d3912-219">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d3912-219">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_two-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="d3912-220">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3912-220">Request</span></span>
<span data-ttu-id="d3912-221">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="d3912-221">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="d3912-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3912-222">Response</span></span>
<span data-ttu-id="d3912-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3912-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3912-226">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d3912-226">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3912-227">C#</span><span class="sxs-lookup"><span data-stu-id="d3912-227">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3912-228">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3912-228">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_three-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d3912-229">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d3912-229">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_three-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="d3912-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3912-230">Request</span></span>
<span data-ttu-id="d3912-231">Этот запрос обновляет начертание, размер и цвет шрифта в третьей ячейке.</span><span class="sxs-lookup"><span data-stu-id="d3912-231">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="d3912-232">Обратите внимание: свойство подчеркивания (Underline) принимает значения **Single** или **Double**.</span><span class="sxs-lookup"><span data-stu-id="d3912-232">Note that the underline property takes **Single** or **Double** as values.</span></span>

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
##### <a name="response"></a><span data-ttu-id="d3912-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3912-233">Response</span></span>
<span data-ttu-id="d3912-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3912-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3912-237">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d3912-237">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3912-238">C#</span><span class="sxs-lookup"><span data-stu-id="d3912-238">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3912-239">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3912-239">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_three-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d3912-240">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d3912-240">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_three-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="d3912-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3912-241">Request</span></span>
<span data-ttu-id="d3912-242">Этот запрос обновляет цвет заливки третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="d3912-242">This request updates the background color of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="d3912-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3912-243">Response</span></span>
<span data-ttu-id="d3912-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3912-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3912-247">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d3912-247">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3912-248">C#</span><span class="sxs-lookup"><span data-stu-id="d3912-248">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3912-249">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3912-249">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_three-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d3912-250">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d3912-250">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_three-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: update_rangeformat_font_three/underline:
      Expected type String but actual was Single. Property: underline, actual value: 'Single'"
  ],
  "tocPath": ""
}-->
