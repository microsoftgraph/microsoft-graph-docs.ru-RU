# <a name="update-range"></a><span data-ttu-id="fcf1d-101">Обновление диапазона</span><span class="sxs-lookup"><span data-stu-id="fcf1d-101">Update range</span></span>

<span data-ttu-id="fcf1d-102">Обновление свойств объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="fcf1d-102">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fcf1d-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fcf1d-103">Permissions</span></span>
<span data-ttu-id="fcf1d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fcf1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fcf1d-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcf1d-106">Permission type</span></span>      | <span data-ttu-id="fcf1d-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcf1d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcf1d-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcf1d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fcf1d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fcf1d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fcf1d-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcf1d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcf1d-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcf1d-111">Not supported.</span></span>    |
|<span data-ttu-id="fcf1d-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcf1d-112">Application</span></span> | <span data-ttu-id="fcf1d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcf1d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fcf1d-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcf1d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range
PATCH /workbook/worksheets/{id|name}/range(address='<address>')
PATCH /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="fcf1d-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcf1d-115">Optional request headers</span></span>
| <span data-ttu-id="fcf1d-116">Имя</span><span class="sxs-lookup"><span data-stu-id="fcf1d-116">Name</span></span>       | <span data-ttu-id="fcf1d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="fcf1d-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fcf1d-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fcf1d-118">Authorization</span></span>  | <span data-ttu-id="fcf1d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcf1d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fcf1d-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fcf1d-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="fcf1d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="fcf1d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcf1d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcf1d-124">Request body</span></span>
<span data-ttu-id="fcf1d-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="fcf1d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fcf1d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcf1d-128">Property</span></span>     | <span data-ttu-id="fcf1d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="fcf1d-129">Type</span></span>   |<span data-ttu-id="fcf1d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="fcf1d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fcf1d-131">columnHidden</span><span class="sxs-lookup"><span data-stu-id="fcf1d-131">columnHidden</span></span>|<span data-ttu-id="fcf1d-132">boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="fcf1d-132">boolean</span></span>|<span data-ttu-id="fcf1d-133">Указывает, скрыты ли все столбцы текущего диапазона.</span><span class="sxs-lookup"><span data-stu-id="fcf1d-133">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="fcf1d-134">formulas</span><span class="sxs-lookup"><span data-stu-id="fcf1d-134">formulas</span></span>|<span data-ttu-id="fcf1d-135">Json</span><span class="sxs-lookup"><span data-stu-id="fcf1d-135">Json</span></span>|<span data-ttu-id="fcf1d-136">Представляет формулу в формате A1.</span><span class="sxs-lookup"><span data-stu-id="fcf1d-136">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="fcf1d-137">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="fcf1d-137">formulasLocal</span></span>|<span data-ttu-id="fcf1d-138">Json</span><span class="sxs-lookup"><span data-stu-id="fcf1d-138">Json</span></span>|<span data-ttu-id="fcf1d-p105">Представляет формулу в нотации стиля A1 на языке пользователя и в соответствии с его языковым стандартом. Например, английская формула =SUM(A1, 1.5) превратится в "=СУММ(A1; 1,5)" на русском языке.</span><span class="sxs-lookup"><span data-stu-id="fcf1d-p105">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="fcf1d-141">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="fcf1d-141">formulasR1C1</span></span>|<span data-ttu-id="fcf1d-142">Json</span><span class="sxs-lookup"><span data-stu-id="fcf1d-142">Json</span></span>|<span data-ttu-id="fcf1d-143">Представляет формулу в формате R1C1.</span><span class="sxs-lookup"><span data-stu-id="fcf1d-143">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="fcf1d-144">numberFormat</span><span class="sxs-lookup"><span data-stu-id="fcf1d-144">numberFormat</span></span>|<span data-ttu-id="fcf1d-145">Json</span><span class="sxs-lookup"><span data-stu-id="fcf1d-145">Json</span></span>|<span data-ttu-id="fcf1d-146">Представляет код числового формата Excel для данной ячейки.</span><span class="sxs-lookup"><span data-stu-id="fcf1d-146">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="fcf1d-147">rowHidden</span><span class="sxs-lookup"><span data-stu-id="fcf1d-147">rowHidden</span></span>|<span data-ttu-id="fcf1d-148">boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="fcf1d-148">boolean</span></span>|<span data-ttu-id="fcf1d-149">Указывает, скрыты ли все строки текущего диапазона.</span><span class="sxs-lookup"><span data-stu-id="fcf1d-149">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="fcf1d-150">values</span><span class="sxs-lookup"><span data-stu-id="fcf1d-150">values</span></span>|<span data-ttu-id="fcf1d-151">Json</span><span class="sxs-lookup"><span data-stu-id="fcf1d-151">Json</span></span>|<span data-ttu-id="fcf1d-p106">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="fcf1d-p106">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="fcf1d-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcf1d-155">Response</span></span>

<span data-ttu-id="fcf1d-156">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [Range](../resources/range.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fcf1d-156">If successful, this method returns a `200 OK` response code and updated [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fcf1d-157">Пример</span><span class="sxs-lookup"><span data-stu-id="fcf1d-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fcf1d-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcf1d-158">Request</span></span>
<span data-ttu-id="fcf1d-p107">Ниже приведен пример запроса. Он обновляет диапазон — значения числовой формат и формулу. Значение `null` сообщает API, что в данном случае нужно пропустить ячейку. Значения, числовые форматы и формулы можно обновлять по отдельности или в одном вызове API.</span><span class="sxs-lookup"><span data-stu-id="fcf1d-p107">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_range"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='A1:B2')
Content-type: application/json
Content-length: 169

{
"values" : [["Hello", "100"],["1/1/2016", null]],
"formula" : [[null, null], [null, "=B1*2"]],
"numberFormat" : [[null,null], ["m-ddd", null]]
}
```
##### <a name="response"></a><span data-ttu-id="fcf1d-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcf1d-163">Response</span></span>
<span data-ttu-id="fcf1d-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fcf1d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update range",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/range_update.md/update_range/numberFormat:
      Inconsistent types between parameter (Collection) and table (None)",
    "Warning: /api-reference/v1.0/api/range_update.md/update_range/values:
      Inconsistent types between parameter (Collection) and table (None)",
    "Error: /api-reference/v1.0/api/range_update.md/update_range/numberFormat:
      Type mismatch between example and table. Parameter name: numberFormat; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not.",
    "Error: /api-reference/v1.0/api/range_update.md/update_range/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->
