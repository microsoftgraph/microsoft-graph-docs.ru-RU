# <a name="update-formatprotection"></a><span data-ttu-id="cad45-101">Обновление объекта FormatProtection</span><span class="sxs-lookup"><span data-stu-id="cad45-101">Update formatprotection</span></span>

<span data-ttu-id="cad45-102">Обновление свойств объекта FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="cad45-102">Update the properties of formatprotection object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cad45-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="cad45-103">Prerequisites</span></span>
<span data-ttu-id="cad45-104">Для применения этого API требуются указанные **области**:</span><span class="sxs-lookup"><span data-stu-id="cad45-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="cad45-105">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="cad45-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="cad45-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cad45-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/protection
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="cad45-107">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cad45-107">Optional request headers</span></span>
| <span data-ttu-id="cad45-108">Имя</span><span class="sxs-lookup"><span data-stu-id="cad45-108">Name</span></span>       | <span data-ttu-id="cad45-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cad45-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cad45-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cad45-110">Authorization</span></span>  | <span data-ttu-id="cad45-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cad45-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cad45-113">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cad45-113">Request body</span></span>
<span data-ttu-id="cad45-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="cad45-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cad45-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="cad45-117">Property</span></span>     | <span data-ttu-id="cad45-118">Тип</span><span class="sxs-lookup"><span data-stu-id="cad45-118">Type</span></span>   |<span data-ttu-id="cad45-119">Описание</span><span class="sxs-lookup"><span data-stu-id="cad45-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cad45-120">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="cad45-120">formulaHidden</span></span>|<span data-ttu-id="cad45-121">boolean</span><span class="sxs-lookup"><span data-stu-id="cad45-121">boolean</span></span>|<span data-ttu-id="cad45-p103">Указывает, скрывает ли Excel формулу для ячеек в диапазоне. Значение NULL указывает, что для всего диапазона не задан единый параметр скрытия формулы.</span><span class="sxs-lookup"><span data-stu-id="cad45-p103">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="cad45-124">locked</span><span class="sxs-lookup"><span data-stu-id="cad45-124">locked</span></span>|<span data-ttu-id="cad45-125">boolean</span><span class="sxs-lookup"><span data-stu-id="cad45-125">boolean</span></span>|<span data-ttu-id="cad45-p104">Указывает, блокирует ли Excel ячейки в объекте. Значение NULL указывает, что для всего диапазона не задан единый параметр блокировки.</span><span class="sxs-lookup"><span data-stu-id="cad45-p104">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="cad45-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="cad45-128">Response</span></span>

<span data-ttu-id="cad45-129">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [FormatProtection](../resources/formatprotection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cad45-129">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cad45-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cad45-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cad45-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cad45-131">Request</span></span>
<span data-ttu-id="cad45-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cad45-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_formatprotection"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/protection
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
##### <a name="response"></a><span data-ttu-id="cad45-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="cad45-133">Response</span></span>
<span data-ttu-id="cad45-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cad45-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update formatprotection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->