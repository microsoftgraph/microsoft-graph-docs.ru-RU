# <a name="update-tablecolumn"></a><span data-ttu-id="4fede-101">Обновление объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="4fede-101">Update tablecolumn</span></span>

<span data-ttu-id="4fede-102">Обновление свойств объекта tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="4fede-102">Update the properties of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4fede-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4fede-103">Permissions</span></span>
<span data-ttu-id="4fede-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4fede-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4fede-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fede-106">Permission type</span></span>      | <span data-ttu-id="4fede-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fede-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4fede-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fede-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4fede-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4fede-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4fede-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fede-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fede-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fede-111">Not supported.</span></span>    |
|<span data-ttu-id="4fede-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fede-112">Application</span></span> | <span data-ttu-id="4fede-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fede-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fede-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fede-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/columns/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="4fede-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4fede-115">Optional request headers</span></span>
| <span data-ttu-id="4fede-116">Имя</span><span class="sxs-lookup"><span data-stu-id="4fede-116">Name</span></span>       | <span data-ttu-id="4fede-117">Описание</span><span class="sxs-lookup"><span data-stu-id="4fede-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4fede-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4fede-118">Authorization</span></span>  | <span data-ttu-id="4fede-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fede-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4fede-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4fede-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="4fede-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4fede-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fede-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4fede-124">Request body</span></span>
<span data-ttu-id="4fede-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4fede-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4fede-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fede-128">Property</span></span>     | <span data-ttu-id="4fede-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4fede-129">Type</span></span>   |<span data-ttu-id="4fede-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4fede-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4fede-131">values</span><span class="sxs-lookup"><span data-stu-id="4fede-131">values</span></span>|<span data-ttu-id="4fede-132">json</span><span class="sxs-lookup"><span data-stu-id="4fede-132">json</span></span>|<span data-ttu-id="4fede-p105">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="4fede-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="4fede-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fede-136">Response</span></span>

<span data-ttu-id="4fede-137">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [TableColumn](../resources/tablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4fede-137">If successful, this method returns a `200 OK` response code and updated [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4fede-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4fede-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4fede-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fede-139">Request</span></span>
<span data-ttu-id="4fede-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4fede-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablecolumn"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
Content-type: application/json
Content-length: 81

{
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="4fede-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fede-141">Response</span></span>
<span data-ttu-id="4fede-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4fede-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tablecolumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->