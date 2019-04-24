---
title: Обновление объекта RangeFormat
description: Обновление свойств объекта rangeformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 649a0c88779ab54c8e4cb8ab93238be3ee000a4d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32452844"
---
# <a name="update-rangeformat"></a><span data-ttu-id="94a13-103">Обновление объекта RangeFormat</span><span class="sxs-lookup"><span data-stu-id="94a13-103">Update rangeformat</span></span>

<span data-ttu-id="94a13-104">Обновление свойств объекта rangeformat.</span><span class="sxs-lookup"><span data-stu-id="94a13-104">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="94a13-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94a13-105">Permissions</span></span>
<span data-ttu-id="94a13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94a13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94a13-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94a13-108">Permission type</span></span>      | <span data-ttu-id="94a13-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94a13-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94a13-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94a13-110">Delegated (work or school account)</span></span> | <span data-ttu-id="94a13-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94a13-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="94a13-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94a13-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94a13-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94a13-113">Not supported.</span></span>    |
|<span data-ttu-id="94a13-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94a13-114">Application</span></span> | <span data-ttu-id="94a13-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94a13-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94a13-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94a13-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="request-headers"></a><span data-ttu-id="94a13-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94a13-117">Request headers</span></span>
| <span data-ttu-id="94a13-118">Имя</span><span class="sxs-lookup"><span data-stu-id="94a13-118">Name</span></span>       | <span data-ttu-id="94a13-119">Описание</span><span class="sxs-lookup"><span data-stu-id="94a13-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="94a13-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94a13-120">Authorization</span></span>  | <span data-ttu-id="94a13-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94a13-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94a13-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="94a13-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="94a13-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="94a13-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94a13-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94a13-126">Request body</span></span>
<span data-ttu-id="94a13-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="94a13-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="94a13-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="94a13-130">Property</span></span>     | <span data-ttu-id="94a13-131">Тип</span><span class="sxs-lookup"><span data-stu-id="94a13-131">Type</span></span>   |<span data-ttu-id="94a13-132">Описание</span><span class="sxs-lookup"><span data-stu-id="94a13-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94a13-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="94a13-133">columnWidth</span></span>|<span data-ttu-id="94a13-134">double</span><span class="sxs-lookup"><span data-stu-id="94a13-134">double</span></span>|<span data-ttu-id="94a13-p105">Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="94a13-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="94a13-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="94a13-137">horizontalAlignment</span></span>|<span data-ttu-id="94a13-138">строка</span><span class="sxs-lookup"><span data-stu-id="94a13-138">string</span></span>|<span data-ttu-id="94a13-139">Представляет выравнивание по горизонтали для указанного объекта.</span><span class="sxs-lookup"><span data-stu-id="94a13-139">Represents the horizontal alignment for the specified object.</span></span> <span data-ttu-id="94a13-140">Возможные `General`значения:, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`,. `Distributed`</span><span class="sxs-lookup"><span data-stu-id="94a13-140">The possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="94a13-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="94a13-141">rowHeight</span></span>|<span data-ttu-id="94a13-142">double</span><span class="sxs-lookup"><span data-stu-id="94a13-142">double</span></span>|<span data-ttu-id="94a13-p107">Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="94a13-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="94a13-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="94a13-145">verticalAlignment</span></span>|<span data-ttu-id="94a13-146">string</span><span class="sxs-lookup"><span data-stu-id="94a13-146">string</span></span>|<span data-ttu-id="94a13-147">Представляет выравнивание по вертикали для указанного объекта.</span><span class="sxs-lookup"><span data-stu-id="94a13-147">Represents the vertical alignment for the specified object.</span></span> <span data-ttu-id="94a13-148">Допустимые значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="94a13-148">The possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="94a13-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="94a13-149">wrapText</span></span>|<span data-ttu-id="94a13-150">boolean</span><span class="sxs-lookup"><span data-stu-id="94a13-150">boolean</span></span>|<span data-ttu-id="94a13-p109">Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.</span><span class="sxs-lookup"><span data-stu-id="94a13-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="94a13-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="94a13-153">Response</span></span>

<span data-ttu-id="94a13-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукранжеформат](../resources/rangeformat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="94a13-154">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94a13-155">Пример</span><span class="sxs-lookup"><span data-stu-id="94a13-155">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="94a13-156">Обновляет свойства Format, Fill и Font в трех ячейках таблицы</span><span class="sxs-lookup"><span data-stu-id="94a13-156">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="94a13-157">В следующих примерах показано, как обновить свойства [воркбукранжеформат](../resources/rangeformat.md), [воркбукранжефилл](../resources/rangefill.md)и [воркбукранжефонт](../resources/rangefont.md) указанного диапазона.</span><span class="sxs-lookup"><span data-stu-id="94a13-157">The following examples demonstrate how to update properties of the [WorkbookRangeFormat](../resources/rangeformat.md), [WorkbookRangeFill](../resources/rangefill.md), and [WorkbookRangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="94a13-158">В результате этого набора запросов создается таблица с тремя ячейками, отформатированными так же, как три ячейки на приведенном ниже рисунке.</span><span class="sxs-lookup"><span data-stu-id="94a13-158">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Таблица-диаграмма Excel с тремя ячейками, свойства Format, Fill и Font которых были обновлены.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="94a13-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="94a13-160">Request</span></span>
<span data-ttu-id="94a13-161">Этот запрос обновляет выравнивание по вертикали, высоту строк и столбцов первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="94a13-161">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="94a13-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="94a13-162">Response</span></span>
<span data-ttu-id="94a13-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94a13-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="94a13-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="94a13-166">Request</span></span>
<span data-ttu-id="94a13-167">Этот запрос обновляет начертание, размер и цвет шрифта в первой ячейке.</span><span class="sxs-lookup"><span data-stu-id="94a13-167">This request updates the font style, size, and color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="94a13-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="94a13-168">Response</span></span>
<span data-ttu-id="94a13-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94a13-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="94a13-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="94a13-172">Request</span></span>
<span data-ttu-id="94a13-173">Этот запрос обновляет цвет заливки первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="94a13-173">This request updates the background color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="94a13-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="94a13-174">Response</span></span>
<span data-ttu-id="94a13-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94a13-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="94a13-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="94a13-178">Request</span></span>
<span data-ttu-id="94a13-179">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="94a13-179">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="94a13-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="94a13-180">Response</span></span>
<span data-ttu-id="94a13-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94a13-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="94a13-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="94a13-184">Request</span></span>
<span data-ttu-id="94a13-185">Этот запрос обновляет начертание и размер шрифта во второй ячейке.</span><span class="sxs-lookup"><span data-stu-id="94a13-185">This request updates the font style and size of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="94a13-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="94a13-186">Response</span></span>
<span data-ttu-id="94a13-p114">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94a13-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="94a13-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="94a13-190">Request</span></span>
<span data-ttu-id="94a13-191">Этот запрос обновляет цвет заливки второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="94a13-191">This request updates the background color of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="94a13-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="94a13-192">Response</span></span>
<span data-ttu-id="94a13-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94a13-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="94a13-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="94a13-196">Request</span></span>
<span data-ttu-id="94a13-197">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="94a13-197">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="94a13-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="94a13-198">Response</span></span>
<span data-ttu-id="94a13-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94a13-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="94a13-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="94a13-202">Request</span></span>
<span data-ttu-id="94a13-203">Этот запрос обновляет начертание, размер и цвет шрифта в третьей ячейке.</span><span class="sxs-lookup"><span data-stu-id="94a13-203">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="94a13-204">Обратите внимание: свойство подчеркивания (Underline) принимает значения **Single** или **Double**.</span><span class="sxs-lookup"><span data-stu-id="94a13-204">Note that the underline property takes **Single** or **Double** as values.</span></span>

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
##### <a name="response"></a><span data-ttu-id="94a13-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="94a13-205">Response</span></span>
<span data-ttu-id="94a13-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94a13-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="94a13-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="94a13-209">Request</span></span>
<span data-ttu-id="94a13-210">Этот запрос обновляет цвет заливки третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="94a13-210">This request updates the background color of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="94a13-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="94a13-211">Response</span></span>
<span data-ttu-id="94a13-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94a13-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
