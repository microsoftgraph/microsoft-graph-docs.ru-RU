# <a name="update-rangeformat"></a><span data-ttu-id="da9d9-101">Обновление объекта RangeFormat</span><span class="sxs-lookup"><span data-stu-id="da9d9-101">Update rangeformat</span></span>

<span data-ttu-id="da9d9-102">Обновление свойств объекта rangeformat.</span><span class="sxs-lookup"><span data-stu-id="da9d9-102">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="da9d9-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da9d9-103">Permissions</span></span>
<span data-ttu-id="da9d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="da9d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="da9d9-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da9d9-106">Permission type</span></span>      | <span data-ttu-id="da9d9-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da9d9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da9d9-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da9d9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="da9d9-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da9d9-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="da9d9-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da9d9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da9d9-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da9d9-111">Not supported.</span></span>    |
|<span data-ttu-id="da9d9-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da9d9-112">Application</span></span> | <span data-ttu-id="da9d9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da9d9-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da9d9-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da9d9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="da9d9-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da9d9-115">Optional request headers</span></span>
| <span data-ttu-id="da9d9-116">Имя</span><span class="sxs-lookup"><span data-stu-id="da9d9-116">Name</span></span>       | <span data-ttu-id="da9d9-117">Описание</span><span class="sxs-lookup"><span data-stu-id="da9d9-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="da9d9-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da9d9-118">Authorization</span></span>  | <span data-ttu-id="da9d9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da9d9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da9d9-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da9d9-121">Request body</span></span>
<span data-ttu-id="da9d9-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="da9d9-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="da9d9-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="da9d9-125">Property</span></span>     | <span data-ttu-id="da9d9-126">Тип</span><span class="sxs-lookup"><span data-stu-id="da9d9-126">Type</span></span>   |<span data-ttu-id="da9d9-127">Описание</span><span class="sxs-lookup"><span data-stu-id="da9d9-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da9d9-128">columnWidth</span><span class="sxs-lookup"><span data-stu-id="da9d9-128">columnWidth</span></span>|<span data-ttu-id="da9d9-129">double</span><span class="sxs-lookup"><span data-stu-id="da9d9-129">double</span></span>|<span data-ttu-id="da9d9-p104">Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="da9d9-p104">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="da9d9-132">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="da9d9-132">horizontalAlignment</span></span>|<span data-ttu-id="da9d9-133">string</span><span class="sxs-lookup"><span data-stu-id="da9d9-133">string</span></span>|<span data-ttu-id="da9d9-p105">Представляет горизонтальное выравнивание для указанного объекта. Возможные значения: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="da9d9-p105">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="da9d9-136">rowHeight</span><span class="sxs-lookup"><span data-stu-id="da9d9-136">rowHeight</span></span>|<span data-ttu-id="da9d9-137">double</span><span class="sxs-lookup"><span data-stu-id="da9d9-137">double</span></span>|<span data-ttu-id="da9d9-p106">Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="da9d9-p106">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="da9d9-140">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="da9d9-140">verticalAlignment</span></span>|<span data-ttu-id="da9d9-141">string</span><span class="sxs-lookup"><span data-stu-id="da9d9-141">string</span></span>|<span data-ttu-id="da9d9-p107">Представляет вертикальное выравнивание для указанного объекта. Возможные значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="da9d9-p107">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="da9d9-144">wrapText</span><span class="sxs-lookup"><span data-stu-id="da9d9-144">wrapText</span></span>|<span data-ttu-id="da9d9-145">boolean</span><span class="sxs-lookup"><span data-stu-id="da9d9-145">boolean</span></span>|<span data-ttu-id="da9d9-p108">Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.</span><span class="sxs-lookup"><span data-stu-id="da9d9-p108">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="da9d9-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="da9d9-148">Response</span></span>

<span data-ttu-id="da9d9-149">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [RangeFormat](../resources/rangeformat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="da9d9-149">If successful, this method returns a `200 OK` response code and updated [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da9d9-150">Пример</span><span class="sxs-lookup"><span data-stu-id="da9d9-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da9d9-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="da9d9-151">Request</span></span>
<span data-ttu-id="da9d9-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da9d9-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format
Content-type: application/json
Content-length: 96

{
  "columnWidth": 99,
  "horizontalAlignment": "horizontalAlignment-value",
  "rowHeight": 99
}
```
##### <a name="response"></a><span data-ttu-id="da9d9-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="da9d9-153">Response</span></span>
<span data-ttu-id="da9d9-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="da9d9-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 96

{
  "columnWidth": 99,
  "horizontalAlignment": "horizontalAlignment-value",
  "rowHeight": 99
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