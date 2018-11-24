# <a name="list-worksheetcollection"></a><span data-ttu-id="59163-101">Список WorksheetCollection</span><span class="sxs-lookup"><span data-stu-id="59163-101">List WorksheetCollection</span></span>

<span data-ttu-id="59163-102">Получение списка объектов листов.</span><span class="sxs-lookup"><span data-stu-id="59163-102">Retrieve a list of worksheet objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="59163-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59163-103">Permissions</span></span>
<span data-ttu-id="59163-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="59163-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="59163-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59163-106">Permission type</span></span>      | <span data-ttu-id="59163-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59163-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59163-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59163-108">Delegated (work or school account)</span></span> | <span data-ttu-id="59163-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59163-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="59163-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59163-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59163-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59163-111">Not supported.</span></span>    |
|<span data-ttu-id="59163-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59163-112">Application</span></span> | <span data-ttu-id="59163-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59163-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59163-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59163-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59163-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="59163-115">Optional query parameters</span></span>
<span data-ttu-id="59163-116">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="59163-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59163-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59163-117">Request headers</span></span>
| <span data-ttu-id="59163-118">Имя</span><span class="sxs-lookup"><span data-stu-id="59163-118">Name</span></span>      |<span data-ttu-id="59163-119">Описание</span><span class="sxs-lookup"><span data-stu-id="59163-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="59163-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59163-120">Authorization</span></span>  | <span data-ttu-id="59163-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59163-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59163-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="59163-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="59163-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="59163-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59163-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59163-126">Request body</span></span>
<span data-ttu-id="59163-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="59163-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59163-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="59163-128">Response</span></span>

<span data-ttu-id="59163-129">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [WorkbookWorksheet](../resources/worksheet.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="59163-129">If successful, this method returns a `200 OK` response code and collection of [WorkbookWorksheet](../resources/worksheet.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59163-130">Пример</span><span class="sxs-lookup"><span data-stu-id="59163-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59163-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="59163-131">Request</span></span>
<span data-ttu-id="59163-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59163-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheetcollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets
```
##### <a name="response"></a><span data-ttu-id="59163-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="59163-133">Response</span></span>
<span data-ttu-id="59163-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="59163-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "id": "id-value",
      "position": 99,
      "name": "name-value",
      "visibility": "visibility-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List WorksheetCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->