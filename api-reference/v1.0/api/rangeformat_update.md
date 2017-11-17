# <a name="update-rangeformat"></a><span data-ttu-id="59d61-101">Обновление объекта RangeFormat</span><span class="sxs-lookup"><span data-stu-id="59d61-101">Update rangeformat</span></span>

<span data-ttu-id="59d61-102">Обновление свойств объекта rangeformat.</span><span class="sxs-lookup"><span data-stu-id="59d61-102">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="59d61-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59d61-103">Permissions</span></span>
<span data-ttu-id="59d61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="59d61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="59d61-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59d61-106">Permission type</span></span>      | <span data-ttu-id="59d61-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59d61-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59d61-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59d61-108">Delegated (work or school account)</span></span> | <span data-ttu-id="59d61-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59d61-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="59d61-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59d61-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59d61-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59d61-111">Not supported.</span></span>    |
|<span data-ttu-id="59d61-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59d61-112">Application</span></span> | <span data-ttu-id="59d61-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59d61-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59d61-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59d61-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="59d61-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59d61-115">Optional request headers</span></span>
| <span data-ttu-id="59d61-116">Имя</span><span class="sxs-lookup"><span data-stu-id="59d61-116">Name</span></span>       | <span data-ttu-id="59d61-117">Описание</span><span class="sxs-lookup"><span data-stu-id="59d61-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="59d61-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59d61-118">Authorization</span></span>  | <span data-ttu-id="59d61-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59d61-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59d61-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59d61-121">Request body</span></span>
<span data-ttu-id="59d61-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="59d61-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="59d61-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="59d61-125">Property</span></span>     | <span data-ttu-id="59d61-126">Тип</span><span class="sxs-lookup"><span data-stu-id="59d61-126">Type</span></span>   |<span data-ttu-id="59d61-127">Описание</span><span class="sxs-lookup"><span data-stu-id="59d61-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59d61-128">columnWidth</span><span class="sxs-lookup"><span data-stu-id="59d61-128">columnWidth</span></span>|<span data-ttu-id="59d61-129">double</span><span class="sxs-lookup"><span data-stu-id="59d61-129">double</span></span>|<span data-ttu-id="59d61-p104">Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="59d61-p104">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="59d61-132">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="59d61-132">horizontalAlignment</span></span>|<span data-ttu-id="59d61-133">string</span><span class="sxs-lookup"><span data-stu-id="59d61-133">string</span></span>|<span data-ttu-id="59d61-p105">Представляет горизонтальное выравнивание для указанного объекта. Возможные значения: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="59d61-p105">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="59d61-136">rowHeight</span><span class="sxs-lookup"><span data-stu-id="59d61-136">rowHeight</span></span>|<span data-ttu-id="59d61-137">double</span><span class="sxs-lookup"><span data-stu-id="59d61-137">double</span></span>|<span data-ttu-id="59d61-p106">Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="59d61-p106">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="59d61-140">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="59d61-140">verticalAlignment</span></span>|<span data-ttu-id="59d61-141">string</span><span class="sxs-lookup"><span data-stu-id="59d61-141">string</span></span>|<span data-ttu-id="59d61-p107">Представляет вертикальное выравнивание для указанного объекта. Возможные значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="59d61-p107">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="59d61-144">wrapText</span><span class="sxs-lookup"><span data-stu-id="59d61-144">wrapText</span></span>|<span data-ttu-id="59d61-145">boolean</span><span class="sxs-lookup"><span data-stu-id="59d61-145">boolean</span></span>|<span data-ttu-id="59d61-p108">Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.</span><span class="sxs-lookup"><span data-stu-id="59d61-p108">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="59d61-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d61-148">Response</span></span>

<span data-ttu-id="59d61-149">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [RangeFormat](../resources/rangeformat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="59d61-149">If successful, this method returns a `200 OK` response code and updated [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59d61-150">Пример</span><span class="sxs-lookup"><span data-stu-id="59d61-150">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="59d61-151">Обновляет свойства Format, Fill и Font в трех ячейках таблицы</span><span class="sxs-lookup"><span data-stu-id="59d61-151">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="59d61-152">В приведенных ниже примерах показано, как обновить свойства [RangeFormat](../resources/rangeformat.md), [RangeFill](../resources/rangefill.md) и [RangeFont](../resources/rangefont.md) указанного диапазона.</span><span class="sxs-lookup"><span data-stu-id="59d61-152">The following examples demonstrate how to update properties of the [RangeFormat](../resources/rangeformat.md), [RangeFill](../resources/rangefill.md), and [RangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="59d61-153">В результате этого набора запросов создается таблица с тремя ячейками, отформатированными так же, как три ячейки на приведенном ниже рисунке.</span><span class="sxs-lookup"><span data-stu-id="59d61-153">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Таблица-диаграмма Excel с тремя ячейками, свойства Format, Fill и Font которых были обновлены.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="59d61-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="59d61-155">Request</span></span>
<span data-ttu-id="59d61-156">Этот запрос обновляет выравнивание по вертикали, высоту строк и столбцов первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="59d61-156">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="59d61-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d61-157">Response</span></span>
<span data-ttu-id="59d61-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="59d61-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="59d61-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="59d61-161">Request</span></span>
<span data-ttu-id="59d61-162">Этот запрос обновляет начертание, размер и цвет шрифта в первой ячейке.</span><span class="sxs-lookup"><span data-stu-id="59d61-162">This request updates the font style, size, and color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="59d61-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d61-163">Response</span></span>
<span data-ttu-id="59d61-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="59d61-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="59d61-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="59d61-167">Request</span></span>
<span data-ttu-id="59d61-168">Этот запрос обновляет цвет заливки первой ячейки.</span><span class="sxs-lookup"><span data-stu-id="59d61-168">This request updates the background color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="59d61-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d61-169">Response</span></span>
<span data-ttu-id="59d61-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="59d61-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="59d61-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="59d61-173">Request</span></span>
<span data-ttu-id="59d61-174">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="59d61-174">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="59d61-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d61-175">Response</span></span>
<span data-ttu-id="59d61-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="59d61-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="59d61-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="59d61-179">Request</span></span>
<span data-ttu-id="59d61-180">Этот запрос обновляет начертание и размер шрифта во второй ячейке.</span><span class="sxs-lookup"><span data-stu-id="59d61-180">This request updates the font style and size of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="59d61-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d61-181">Response</span></span>
<span data-ttu-id="59d61-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="59d61-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="59d61-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="59d61-185">Request</span></span>
<span data-ttu-id="59d61-186">Этот запрос обновляет цвет заливки второй ячейки.</span><span class="sxs-lookup"><span data-stu-id="59d61-186">This request updates the background color of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="59d61-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d61-187">Response</span></span>
<span data-ttu-id="59d61-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="59d61-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="59d61-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="59d61-191">Request</span></span>
<span data-ttu-id="59d61-192">Этот запрос обновляет выравнивание по вертикали и горизонтали, высоту строк и столбцов третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="59d61-192">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="59d61-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d61-193">Response</span></span>
<span data-ttu-id="59d61-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="59d61-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="59d61-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="59d61-197">Request</span></span>
<span data-ttu-id="59d61-198">Этот запрос обновляет начертание, размер и цвет шрифта в третьей ячейке.</span><span class="sxs-lookup"><span data-stu-id="59d61-198">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="59d61-199">Обратите внимание: свойство подчеркивания (Underline) принимает значения **Single** или **Double**.</span><span class="sxs-lookup"><span data-stu-id="59d61-199">Note that the underline property takes **Single** or **Double** as values.</span></span>

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
##### <a name="response"></a><span data-ttu-id="59d61-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d61-200">Response</span></span>
<span data-ttu-id="59d61-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="59d61-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="59d61-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="59d61-204">Request</span></span>
<span data-ttu-id="59d61-205">Этот запрос обновляет цвет заливки третьей ячейки.</span><span class="sxs-lookup"><span data-stu-id="59d61-205">This request updates the background color of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="59d61-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d61-206">Response</span></span>
<span data-ttu-id="59d61-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="59d61-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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