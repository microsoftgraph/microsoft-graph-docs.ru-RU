# <a name="update-range"></a><span data-ttu-id="9cb56-101">Обновление диапазона</span><span class="sxs-lookup"><span data-stu-id="9cb56-101">Update range</span></span>

<span data-ttu-id="9cb56-102">Обновление свойств объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="9cb56-102">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9cb56-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9cb56-103">Permissions</span></span>
<span data-ttu-id="9cb56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9cb56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9cb56-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9cb56-106">Permission type</span></span>      | <span data-ttu-id="9cb56-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9cb56-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cb56-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9cb56-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9cb56-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cb56-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9cb56-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9cb56-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cb56-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cb56-111">Not supported.</span></span>    |
|<span data-ttu-id="9cb56-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9cb56-112">Application</span></span> | <span data-ttu-id="9cb56-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cb56-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cb56-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9cb56-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range
PATCH /workbook/worksheets/{id|name}/range(address='<address>')
PATCH /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="9cb56-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9cb56-115">Optional request headers</span></span>
| <span data-ttu-id="9cb56-116">Имя</span><span class="sxs-lookup"><span data-stu-id="9cb56-116">Name</span></span>       | <span data-ttu-id="9cb56-117">Описание</span><span class="sxs-lookup"><span data-stu-id="9cb56-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9cb56-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9cb56-118">Authorization</span></span>  | <span data-ttu-id="9cb56-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9cb56-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cb56-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9cb56-121">Request body</span></span>
<span data-ttu-id="9cb56-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9cb56-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9cb56-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cb56-125">Property</span></span>     | <span data-ttu-id="9cb56-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9cb56-126">Type</span></span>   |<span data-ttu-id="9cb56-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9cb56-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9cb56-128">columnHidden</span><span class="sxs-lookup"><span data-stu-id="9cb56-128">columnHidden</span></span>|<span data-ttu-id="9cb56-129">boolean</span><span class="sxs-lookup"><span data-stu-id="9cb56-129">boolean</span></span>|<span data-ttu-id="9cb56-130">Указывает, скрыты ли все столбцы текущего диапазона.</span><span class="sxs-lookup"><span data-stu-id="9cb56-130">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="9cb56-131">formulas</span><span class="sxs-lookup"><span data-stu-id="9cb56-131">formulas</span></span>|<span data-ttu-id="9cb56-132">json</span><span class="sxs-lookup"><span data-stu-id="9cb56-132">json</span></span>|<span data-ttu-id="9cb56-133">Представляет формулу в формате A1.</span><span class="sxs-lookup"><span data-stu-id="9cb56-133">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="9cb56-134">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="9cb56-134">formulasLocal</span></span>|<span data-ttu-id="9cb56-135">json</span><span class="sxs-lookup"><span data-stu-id="9cb56-135">json</span></span>|<span data-ttu-id="9cb56-p104">Представляет формулу в нотации стиля A1 на языке пользователя и в соответствии с его языковым стандартом. Например, английская формула =SUM(A1, 1.5) превратится в "=СУММ(A1; 1,5)" на русском языке.</span><span class="sxs-lookup"><span data-stu-id="9cb56-p104">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="9cb56-138">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="9cb56-138">formulasR1C1</span></span>|<span data-ttu-id="9cb56-139">json</span><span class="sxs-lookup"><span data-stu-id="9cb56-139">json</span></span>|<span data-ttu-id="9cb56-140">Представляет формулу в формате R1C1.</span><span class="sxs-lookup"><span data-stu-id="9cb56-140">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="9cb56-141">numberFormat</span><span class="sxs-lookup"><span data-stu-id="9cb56-141">numberFormat</span></span>|<span data-ttu-id="9cb56-142">json</span><span class="sxs-lookup"><span data-stu-id="9cb56-142">json</span></span>|<span data-ttu-id="9cb56-143">Представляет код числового формата Excel для данной ячейки.</span><span class="sxs-lookup"><span data-stu-id="9cb56-143">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="9cb56-144">rowHidden</span><span class="sxs-lookup"><span data-stu-id="9cb56-144">rowHidden</span></span>|<span data-ttu-id="9cb56-145">boolean</span><span class="sxs-lookup"><span data-stu-id="9cb56-145">boolean</span></span>|<span data-ttu-id="9cb56-146">Указывает, скрыты ли все строки текущего диапазона.</span><span class="sxs-lookup"><span data-stu-id="9cb56-146">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="9cb56-147">values</span><span class="sxs-lookup"><span data-stu-id="9cb56-147">values</span></span>|<span data-ttu-id="9cb56-148">json</span><span class="sxs-lookup"><span data-stu-id="9cb56-148">json</span></span>|<span data-ttu-id="9cb56-p105">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="9cb56-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="9cb56-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cb56-152">Response</span></span>

<span data-ttu-id="9cb56-153">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [Range](../resources/range.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9cb56-153">If successful, this method returns a `200 OK` response code and updated [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9cb56-154">Пример</span><span class="sxs-lookup"><span data-stu-id="9cb56-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cb56-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="9cb56-155">Request</span></span>
<span data-ttu-id="9cb56-p106">Ниже приведен пример запроса. Он обновляет диапазон — значения числовой формат и формулу. Значение `null` сообщает API, что в данном случае нужно пропустить ячейку. Значения, числовые форматы и формулы можно обновлять по отдельности или в одном вызове API.</span><span class="sxs-lookup"><span data-stu-id="9cb56-p106">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_range"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets('sheet1')/range(address='A1:B2')
Content-type: application/json
Content-length: 169

{
"values" : [["Hello", "100"],["1/1/2016", null]],
"formula" : [[null, null], [null, "=B1*2"]],
"numberFormat" : [[null,null], ["m-ddd", null]]
}
```
##### <a name="response"></a><span data-ttu-id="9cb56-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cb56-160">Response</span></span>
<span data-ttu-id="9cb56-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9cb56-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
  "tocPath": ""
}-->
