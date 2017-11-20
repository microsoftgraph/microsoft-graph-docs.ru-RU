# <a name="update-tablerow"></a><span data-ttu-id="a65ef-101">Обновление объекта tableRow</span><span class="sxs-lookup"><span data-stu-id="a65ef-101">Update tablerow</span></span>

<span data-ttu-id="a65ef-102">Обновление свойств объекта tablerow.</span><span class="sxs-lookup"><span data-stu-id="a65ef-102">Update the properties of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a65ef-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a65ef-103">Permissions</span></span>
<span data-ttu-id="a65ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a65ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a65ef-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a65ef-106">Permission type</span></span>      | <span data-ttu-id="a65ef-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a65ef-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a65ef-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a65ef-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a65ef-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a65ef-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a65ef-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a65ef-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a65ef-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a65ef-111">Not supported.</span></span>    |
|<span data-ttu-id="a65ef-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a65ef-112">Application</span></span> | <span data-ttu-id="a65ef-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a65ef-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a65ef-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a65ef-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/rows(<index>)
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="a65ef-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a65ef-115">Optional request headers</span></span>
| <span data-ttu-id="a65ef-116">Имя</span><span class="sxs-lookup"><span data-stu-id="a65ef-116">Name</span></span>       | <span data-ttu-id="a65ef-117">Описание</span><span class="sxs-lookup"><span data-stu-id="a65ef-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a65ef-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a65ef-118">Authorization</span></span>  | <span data-ttu-id="a65ef-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a65ef-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a65ef-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a65ef-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="a65ef-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a65ef-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a65ef-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a65ef-124">Request body</span></span>
<span data-ttu-id="a65ef-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a65ef-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a65ef-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a65ef-128">Property</span></span>     | <span data-ttu-id="a65ef-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a65ef-129">Type</span></span>   |<span data-ttu-id="a65ef-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a65ef-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a65ef-131">values</span><span class="sxs-lookup"><span data-stu-id="a65ef-131">values</span></span>|<span data-ttu-id="a65ef-132">json</span><span class="sxs-lookup"><span data-stu-id="a65ef-132">json</span></span>|<span data-ttu-id="a65ef-p105">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="a65ef-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="a65ef-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a65ef-136">Response</span></span>

<span data-ttu-id="a65ef-137">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [tableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a65ef-137">If successful, this method returns a `200 OK` response code and updated [TableRow](../resources/tablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a65ef-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a65ef-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a65ef-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a65ef-139">Request</span></span>
<span data-ttu-id="a65ef-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a65ef-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablerow"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="a65ef-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a65ef-141">Response</span></span>
<span data-ttu-id="a65ef-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a65ef-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tablerow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->