# <a name="get-eventmessage"></a><span data-ttu-id="fe912-101">Получение объекта eventMessage</span><span class="sxs-lookup"><span data-stu-id="fe912-101">Get eventMessage</span></span>

<span data-ttu-id="fe912-102">Получение свойств и связей объекта [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="fe912-102">Retrieve the properties and relationships of [eventMessage](../resources/eventmessage.md) object.</span></span>

<span data-ttu-id="fe912-103">В настоящее время эта операция возвращает текст сообщения о событии только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="fe912-103">Currently, this operation returns event message bodies in only HTML format.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe912-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fe912-104">Prerequisites</span></span>
<span data-ttu-id="fe912-105">Для применения этого API требуется одна из указанных **областей**: *Mail.Read*</span><span class="sxs-lookup"><span data-stu-id="fe912-105">One of the following **scopes** is required to execute this API: *Mail.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="fe912-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe912-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fe912-107">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fe912-107">Optional query parameters</span></span>
<span data-ttu-id="fe912-108">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fe912-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fe912-109">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe912-109">Request headers</span></span>
| <span data-ttu-id="fe912-110">Имя</span><span class="sxs-lookup"><span data-stu-id="fe912-110">Name</span></span>       | <span data-ttu-id="fe912-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fe912-111">Type</span></span> | <span data-ttu-id="fe912-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fe912-112">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fe912-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe912-113">Authorization</span></span>  | <span data-ttu-id="fe912-114">string</span><span class="sxs-lookup"><span data-stu-id="fe912-114">string</span></span>  | <span data-ttu-id="fe912-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe912-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe912-117">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe912-117">Request body</span></span>
<span data-ttu-id="fe912-118">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe912-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe912-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe912-119">Response</span></span>

<span data-ttu-id="fe912-120">В случае успеха этот метод возвращает код отклика `200 OK` и объект [eventMessage](../resources/eventmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe912-120">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe912-121">Пример</span><span class="sxs-lookup"><span data-stu-id="fe912-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe912-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe912-122">Request</span></span>
<span data-ttu-id="fe912-123">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe912-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_eventmessage"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="fe912-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe912-124">Response</span></span>
<span data-ttu-id="fe912-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fe912-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "html",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "meetingMessageType": "meetingMessageType-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
