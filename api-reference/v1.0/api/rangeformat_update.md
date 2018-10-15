# <a name="update-rangeformat"></a><span data-ttu-id="67b06-101">Обновление объекта RangeFormat</span><span class="sxs-lookup"><span data-stu-id="67b06-101">Update rangeformat</span></span>

<span data-ttu-id="67b06-102">Обновление свойств объекта rangeformat.</span><span class="sxs-lookup"><span data-stu-id="67b06-102">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="67b06-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67b06-103">Permissions</span></span>
<span data-ttu-id="67b06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="67b06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="67b06-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67b06-106">Permission type</span></span>      | <span data-ttu-id="67b06-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67b06-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67b06-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67b06-108">Delegated (work or school account)</span></span> | <span data-ttu-id="67b06-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67b06-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="67b06-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67b06-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67b06-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67b06-111">Not supported.</span></span>    |
|<span data-ttu-id="67b06-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67b06-112">Application</span></span> | <span data-ttu-id="67b06-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67b06-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67b06-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67b06-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="request-headers"></a><span data-ttu-id="67b06-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67b06-115">Request headers</span></span>
| <span data-ttu-id="67b06-116">Имя</span><span class="sxs-lookup"><span data-stu-id="67b06-116">Name</span></span>       | <span data-ttu-id="67b06-117">Описание</span><span class="sxs-lookup"><span data-stu-id="67b06-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="67b06-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67b06-118">Authorization</span></span>  | <span data-ttu-id="67b06-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67b06-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="67b06-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="67b06-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="67b06-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="67b06-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="67b06-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67b06-124">Request body</span></span>
<span data-ttu-id="67b06-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="67b06-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="67b06-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="67b06-128">Property</span></span>     | <span data-ttu-id="67b06-129">Тип</span><span class="sxs-lookup"><span data-stu-id="67b06-129">Type</span></span>   |<span data-ttu-id="67b06-130">Описание</span><span class="sxs-lookup"><span data-stu-id="67b06-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67b06-131">columnWidth</span><span class="sxs-lookup"><span data-stu-id="67b06-131">columnWidth</span></span>|<span data-ttu-id="67b06-132">double</span><span class="sxs-lookup"><span data-stu-id="67b06-132">double</span></span>|<span data-ttu-id="67b06-p105">Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="67b06-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="67b06-135">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="67b06-135">horizontalAlignment</span></span>|<span data-ttu-id="67b06-136">string (строка)</span><span class="sxs-lookup"><span data-stu-id="67b06-136">string</span></span>|<span data-ttu-id="67b06-137">Представляет горизонтальное выравнивание для указанного объекта.</span><span class="sxs-lookup"><span data-stu-id="67b06-137">Represents the horizontal alignment for the specified object. Possible values are: , , , , , , , .</span></span> <span data-ttu-id="67b06-138">Возможные значения: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="67b06-138">The possible values are `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`, , , , or .</span></span>|
|<span data-ttu-id="67b06-139">rowHeight</span><span class="sxs-lookup"><span data-stu-id="67b06-139">rowHeight</span></span>|<span data-ttu-id="67b06-140">double</span><span class="sxs-lookup"><span data-stu-id="67b06-140">double</span></span>|<span data-ttu-id="67b06-p107">Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="67b06-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="67b06-143">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="67b06-143">verticalAlignment</span></span>|<span data-ttu-id="67b06-144">string (строка)</span><span class="sxs-lookup"><span data-stu-id="67b06-144">string</span></span>|<span data-ttu-id="67b06-145">Представляет вертикальное выравнивание для указанного объекта.</span><span class="sxs-lookup"><span data-stu-id="67b06-145">Represents the vertical alignment for the specified object. Possible values are: , , , , .</span></span> <span data-ttu-id="67b06-146">Возможные значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="67b06-146">The possible values are `Top`, `Center`, `Bottom`, `Justify`, `Distributed`, , , , , , , or .</span></span>|
|<span data-ttu-id="67b06-147">wrapText</span><span class="sxs-lookup"><span data-stu-id="67b06-147">wrapText</span></span>|<span data-ttu-id="67b06-148">boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="67b06-148">boolean</span></span>|<span data-ttu-id="67b06-p109">Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.</span><span class="sxs-lookup"><span data-stu-id="67b06-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="67b06-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="67b06-151">Response</span></span>

<span data-ttu-id="67b06-152">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [WorkbookRangeFormat](../resources/rangeformat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="67b06-152">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="67b06-153">Пример</span><span class="sxs-lookup"><span data-stu-id="67b06-153">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="67b06-154">Обновление свойств формата (Format), заливки (Fill) и шрифта (Font) в трех ячейках таблицы</span><span class="sxs-lookup"><span data-stu-id="67b06-154">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="67b06-155">Следующие примеры демонстрируют обновление свойств [WorkbookRangeFormat](../resources/rangeformat.md), [WorkbookRangeFill](../resources/rangefill.md) и [WorkbookRangeFont](../resources/rangefont.md) указанного диапазона.</span><span class="sxs-lookup"><span data-stu-id="67b06-155">The following examples demonstrate how to update properties of the [RangeFormat](../resources/rangeformat.md), [RangeFill](../resources/rangefill.md), and [RangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="67b06-156">В результате этого набора запросов создается таблица с тремя ячейками, отформатированными так же, как три ячейки на приведенном ниже рисунке.</span><span class="sxs-lookup"><span data-stu-id="67b06-156">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Таблица-диаграмма Excel с тремя ячейками, свойства Format, Fill и Font которых были обновлены.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="67b06-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="67b06-158">Request</span></span>
<span data-ttu-id="67b06-159">Этот запрос обновляет выравнивание по вертикали, высоту строк и столбцов первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="67b06-159">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="67b06-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="67b06-160">Response</span></span>
<span data-ttu-id="67b06-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67b06-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="67b06-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="67b06-164">Request</span></span>
<span data-ttu-id="67b06-165">Этот запрос обновляет начертание, размер и цвет шрифта в первой ячейке.</span><span class="sxs-lookup"><span data-stu-id="67b06-165">This request updates the font style, size, and color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="67b06-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="67b06-166">Response</span></span>
<span data-ttu-id="67b06-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67b06-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="67b06-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="67b06-170">Request</span></span>
<span data-ttu-id="67b06-171">Этот запрос обновляет цвет заливки первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="67b06-171">This request updates the background color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="67b06-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="67b06-172">Response</span></span>
<span data-ttu-id="67b06-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67b06-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="67b06-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="67b06-176">Request</span></span>
<span data-ttu-id="67b06-177">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="67b06-177">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="67b06-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="67b06-178">Response</span></span>
<span data-ttu-id="67b06-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67b06-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="67b06-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="67b06-182">Request</span></span>
<span data-ttu-id="67b06-183">Этот запрос обновляет начертание и размер шрифта во второй ячейке.</span><span class="sxs-lookup"><span data-stu-id="67b06-183">This request updates the font style and size of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="67b06-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="67b06-184">Response</span></span>
<span data-ttu-id="67b06-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67b06-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="67b06-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="67b06-188">Request</span></span>
<span data-ttu-id="67b06-189">Этот запрос обновляет цвет заливки второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="67b06-189">This request updates the background color of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="67b06-190">Ответ</span><span class="sxs-lookup"><span data-stu-id="67b06-190">Response</span></span>
<span data-ttu-id="67b06-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67b06-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="67b06-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="67b06-194">Request</span></span>
<span data-ttu-id="67b06-195">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="67b06-195">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="67b06-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="67b06-196">Response</span></span>
<span data-ttu-id="67b06-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67b06-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="67b06-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="67b06-200">Request</span></span>
<span data-ttu-id="67b06-201">Этот запрос обновляет начертание, размер и цвет шрифта в третьей ячейке.</span><span class="sxs-lookup"><span data-stu-id="67b06-201">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="67b06-202">Обратите внимание: свойство подчеркивания (Underline) принимает значения **Single** или **Double**.</span><span class="sxs-lookup"><span data-stu-id="67b06-202">Note that the underline property takes **Single** or **Double** as values.</span></span>

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
##### <a name="response"></a><span data-ttu-id="67b06-203">Ответ</span><span class="sxs-lookup"><span data-stu-id="67b06-203">Response</span></span>
<span data-ttu-id="67b06-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67b06-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="67b06-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="67b06-207">Request</span></span>
<span data-ttu-id="67b06-208">Этот запрос обновляет цвет заливки третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="67b06-208">This request updates the background color of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="67b06-209">Ответ</span><span class="sxs-lookup"><span data-stu-id="67b06-209">Response</span></span>
<span data-ttu-id="67b06-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67b06-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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