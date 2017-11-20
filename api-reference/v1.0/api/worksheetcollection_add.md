# <a name="worksheetcollection-add"></a><span data-ttu-id="e611a-101">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="e611a-101">WorksheetCollection: add</span></span>

<span data-ttu-id="e611a-p101">Добавляет новый лист в книгу. Лист будет добавлен в конец набора имеющихся листов. Если вы хотите активировать только что добавленный лист, вызовите команду .activate().</span><span class="sxs-lookup"><span data-stu-id="e611a-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="e611a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e611a-105">Permissions</span></span>
<span data-ttu-id="e611a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e611a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e611a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e611a-108">Permission type</span></span>      | <span data-ttu-id="e611a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e611a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e611a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e611a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e611a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e611a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e611a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e611a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e611a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e611a-113">Not supported.</span></span>    |
|<span data-ttu-id="e611a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e611a-114">Application</span></span> | <span data-ttu-id="e611a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e611a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e611a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e611a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="e611a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e611a-117">Request headers</span></span>
| <span data-ttu-id="e611a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e611a-118">Name</span></span>       | <span data-ttu-id="e611a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e611a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e611a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e611a-120">Authorization</span></span>  | <span data-ttu-id="e611a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e611a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e611a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e611a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e611a-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e611a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e611a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e611a-126">Request body</span></span>
<span data-ttu-id="e611a-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e611a-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e611a-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="e611a-128">Parameter</span></span>    | <span data-ttu-id="e611a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e611a-129">Type</span></span>   |<span data-ttu-id="e611a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e611a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e611a-131">name</span><span class="sxs-lookup"><span data-stu-id="e611a-131">name</span></span>|<span data-ttu-id="e611a-132">string</span><span class="sxs-lookup"><span data-stu-id="e611a-132">string</span></span>|<span data-ttu-id="e611a-p105">Необязательный параметр. Имя добавляемого листа. Если параметр используется, имя должно быть уникальным. В противном случае Excel определяет имя нового листа.</span><span class="sxs-lookup"><span data-stu-id="e611a-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="e611a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e611a-137">Response</span></span>

<span data-ttu-id="e611a-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Worksheet](../resources/worksheet.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e611a-138">If successful, this method returns `200 OK` response code and [Worksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e611a-139">Пример</span><span class="sxs-lookup"><span data-stu-id="e611a-139">Example</span></span>
<span data-ttu-id="e611a-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e611a-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e611a-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="e611a-141">Request</span></span>
<span data-ttu-id="e611a-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e611a-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="e611a-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e611a-143">Response</span></span>
<span data-ttu-id="e611a-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e611a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->