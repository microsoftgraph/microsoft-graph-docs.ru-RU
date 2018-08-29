# <a name="update-tablecolumn"></a><span data-ttu-id="9d6e7-101">Обновление объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="9d6e7-101">Update tablecolumn</span></span>

<span data-ttu-id="9d6e7-102">Обновление свойств объекта tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="9d6e7-102">Update the properties of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9d6e7-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d6e7-103">Permissions</span></span>
<span data-ttu-id="9d6e7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9d6e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9d6e7-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d6e7-106">Permission type</span></span>      | <span data-ttu-id="9d6e7-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d6e7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d6e7-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d6e7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9d6e7-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d6e7-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9d6e7-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d6e7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d6e7-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d6e7-111">Not supported.</span></span>    |
|<span data-ttu-id="9d6e7-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d6e7-112">Application</span></span> | <span data-ttu-id="9d6e7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d6e7-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d6e7-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d6e7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/columns/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="9d6e7-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d6e7-115">Optional request headers</span></span>
| <span data-ttu-id="9d6e7-116">Имя</span><span class="sxs-lookup"><span data-stu-id="9d6e7-116">Name</span></span>       | <span data-ttu-id="9d6e7-117">Описание</span><span class="sxs-lookup"><span data-stu-id="9d6e7-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9d6e7-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d6e7-118">Authorization</span></span>  | <span data-ttu-id="9d6e7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d6e7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9d6e7-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9d6e7-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="9d6e7-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9d6e7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d6e7-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d6e7-124">Request body</span></span>
<span data-ttu-id="9d6e7-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9d6e7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9d6e7-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d6e7-128">Property</span></span>     | <span data-ttu-id="9d6e7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9d6e7-129">Type</span></span>   |<span data-ttu-id="9d6e7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9d6e7-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d6e7-131">values</span><span class="sxs-lookup"><span data-stu-id="9d6e7-131">values</span></span>|<span data-ttu-id="9d6e7-132">Json</span><span class="sxs-lookup"><span data-stu-id="9d6e7-132">Json</span></span>|<span data-ttu-id="9d6e7-p105">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые (string) и числовые данные (number), а также логические значения (boolean). Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="9d6e7-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="9d6e7-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d6e7-136">Response</span></span>

<span data-ttu-id="9d6e7-137">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [WorkbookTableColumn](../resources/tablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d6e7-137">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/tablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9d6e7-138">Пример</span><span class="sxs-lookup"><span data-stu-id="9d6e7-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d6e7-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d6e7-139">Request</span></span>
<span data-ttu-id="9d6e7-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d6e7-140">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="9d6e7-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d6e7-141">Response</span></span>
<span data-ttu-id="9d6e7-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d6e7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
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