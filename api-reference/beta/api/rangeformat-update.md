---
title: Обновление объекта RangeFormat
description: Обновление свойств объекта rangeformat.
ms.openlocfilehash: ce0632d127036e18e4f4f52a3b776734f8b00002
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082150"
---
# <a name="update-rangeformat"></a><span data-ttu-id="d214a-103">Обновление объекта RangeFormat</span><span class="sxs-lookup"><span data-stu-id="d214a-103">Update rangeformat</span></span>

> <span data-ttu-id="d214a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d214a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d214a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d214a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d214a-106">Обновление свойств объекта rangeformat.</span><span class="sxs-lookup"><span data-stu-id="d214a-106">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d214a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d214a-107">Permissions</span></span>
<span data-ttu-id="d214a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d214a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d214a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d214a-110">Permission type</span></span>      | <span data-ttu-id="d214a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d214a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d214a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d214a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d214a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d214a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d214a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d214a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d214a-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d214a-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d214a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d214a-116">Application</span></span> | <span data-ttu-id="d214a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d214a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d214a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d214a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="d214a-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d214a-119">Optional request headers</span></span>
| <span data-ttu-id="d214a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d214a-120">Name</span></span>       | <span data-ttu-id="d214a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d214a-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d214a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d214a-122">Authorization</span></span>  | <span data-ttu-id="d214a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d214a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d214a-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d214a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d214a-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d214a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d214a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d214a-128">Request body</span></span>
<span data-ttu-id="d214a-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d214a-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d214a-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="d214a-132">Property</span></span>     | <span data-ttu-id="d214a-133">Тип</span><span class="sxs-lookup"><span data-stu-id="d214a-133">Type</span></span>   |<span data-ttu-id="d214a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="d214a-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d214a-135">columnWidth</span><span class="sxs-lookup"><span data-stu-id="d214a-135">columnWidth</span></span>|<span data-ttu-id="d214a-136">double</span><span class="sxs-lookup"><span data-stu-id="d214a-136">double</span></span>|<span data-ttu-id="d214a-p106">Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="d214a-p106">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="d214a-139">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="d214a-139">horizontalAlignment</span></span>|<span data-ttu-id="d214a-140">string</span><span class="sxs-lookup"><span data-stu-id="d214a-140">string</span></span>|<span data-ttu-id="d214a-p107">Представляет горизонтальное выравнивание для указанного объекта. Возможные значения: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="d214a-p107">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="d214a-143">rowHeight</span><span class="sxs-lookup"><span data-stu-id="d214a-143">rowHeight</span></span>|<span data-ttu-id="d214a-144">double</span><span class="sxs-lookup"><span data-stu-id="d214a-144">double</span></span>|<span data-ttu-id="d214a-p108">Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="d214a-p108">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="d214a-147">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="d214a-147">verticalAlignment</span></span>|<span data-ttu-id="d214a-148">string</span><span class="sxs-lookup"><span data-stu-id="d214a-148">string</span></span>|<span data-ttu-id="d214a-p109">Представляет вертикальное выравнивание для указанного объекта. Возможные значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="d214a-p109">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="d214a-151">wrapText</span><span class="sxs-lookup"><span data-stu-id="d214a-151">wrapText</span></span>|<span data-ttu-id="d214a-152">boolean</span><span class="sxs-lookup"><span data-stu-id="d214a-152">boolean</span></span>|<span data-ttu-id="d214a-p110">Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.</span><span class="sxs-lookup"><span data-stu-id="d214a-p110">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="d214a-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="d214a-155">Response</span></span>

<span data-ttu-id="d214a-156">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [RangeFormat](../resources/rangeformat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d214a-156">If successful, this method returns a `200 OK` response code and updated [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d214a-157">Пример</span><span class="sxs-lookup"><span data-stu-id="d214a-157">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="d214a-158">Обновляет свойства Format, Fill и Font в трех ячейках таблицы</span><span class="sxs-lookup"><span data-stu-id="d214a-158">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="d214a-159">В приведенных ниже примерах показано, как обновить свойства [RangeFormat](../resources/rangeformat.md), [RangeFill](../resources/rangefill.md) и [RangeFont](../resources/rangefont.md) указанного диапазона.</span><span class="sxs-lookup"><span data-stu-id="d214a-159">The following examples demonstrate how to update properties of the [RangeFormat](../resources/rangeformat.md), [RangeFill](../resources/rangefill.md), and [RangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="d214a-160">В результате этого набора запросов создается таблица с тремя ячейками, отформатированными так же, как три ячейки на приведенном ниже рисунке.</span><span class="sxs-lookup"><span data-stu-id="d214a-160">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Таблица-диаграмма Excel с тремя ячейками, свойства Format, Fill и Font которых были обновлены.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="d214a-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="d214a-162">Request</span></span>
<span data-ttu-id="d214a-163">Этот запрос обновляет выравнивание по вертикали, высоту строк и столбцов первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="d214a-163">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="d214a-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="d214a-164">Response</span></span>
<span data-ttu-id="d214a-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d214a-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
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

##### <a name="request"></a><span data-ttu-id="d214a-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="d214a-168">Request</span></span>
<span data-ttu-id="d214a-169">Этот запрос обновляет начертание, размер и цвет шрифта в первой ячейке.</span><span class="sxs-lookup"><span data-stu-id="d214a-169">This request updates the font style, size, and color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="d214a-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="d214a-170">Response</span></span>
<span data-ttu-id="d214a-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d214a-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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

##### <a name="request"></a><span data-ttu-id="d214a-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="d214a-174">Request</span></span>
<span data-ttu-id="d214a-175">Этот запрос обновляет цвет заливки первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="d214a-175">This request updates the background color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
##### <a name="response"></a><span data-ttu-id="d214a-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="d214a-176">Response</span></span>
<span data-ttu-id="d214a-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d214a-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#FF0000"
}
```
##### <a name="request"></a><span data-ttu-id="d214a-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="d214a-180">Request</span></span>
<span data-ttu-id="d214a-181">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="d214a-181">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="d214a-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="d214a-182">Response</span></span>
<span data-ttu-id="d214a-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d214a-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
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

##### <a name="request"></a><span data-ttu-id="d214a-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="d214a-186">Request</span></span>
<span data-ttu-id="d214a-187">Этот запрос обновляет начертание и размер шрифта во второй ячейке.</span><span class="sxs-lookup"><span data-stu-id="d214a-187">This request updates the font style and size of the second cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="d214a-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="d214a-188">Response</span></span>
<span data-ttu-id="d214a-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d214a-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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

##### <a name="request"></a><span data-ttu-id="d214a-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="d214a-192">Request</span></span>
<span data-ttu-id="d214a-193">Этот запрос обновляет цвет заливки второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="d214a-193">This request updates the background color of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
##### <a name="response"></a><span data-ttu-id="d214a-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="d214a-194">Response</span></span>
<span data-ttu-id="d214a-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d214a-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#00FF00"
}
```

##### <a name="request"></a><span data-ttu-id="d214a-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="d214a-198">Request</span></span>
<span data-ttu-id="d214a-199">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="d214a-199">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="d214a-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="d214a-200">Response</span></span>
<span data-ttu-id="d214a-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d214a-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
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

##### <a name="request"></a><span data-ttu-id="d214a-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="d214a-204">Request</span></span>
<span data-ttu-id="d214a-205">Этот запрос обновляет начертание, размер и цвет шрифта в третьей ячейке.</span><span class="sxs-lookup"><span data-stu-id="d214a-205">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="d214a-206">Обратите внимание: свойство подчеркивания (Underline) принимает значения **Single** или **Double**.</span><span class="sxs-lookup"><span data-stu-id="d214a-206">Note that the underline property takes **Single** or **Double** as values.</span></span>

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="d214a-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="d214a-207">Response</span></span>
<span data-ttu-id="d214a-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d214a-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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

##### <a name="request"></a><span data-ttu-id="d214a-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="d214a-211">Request</span></span>
<span data-ttu-id="d214a-212">Этот запрос обновляет цвет заливки третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="d214a-212">This request updates the background color of the third cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
##### <a name="response"></a><span data-ttu-id="d214a-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="d214a-213">Response</span></span>
<span data-ttu-id="d214a-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="d214a-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
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
  "tocPath": ""
}-->