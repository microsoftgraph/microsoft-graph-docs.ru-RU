# <a name="get-eventmessage"></a><span data-ttu-id="77e6c-101">Получение объекта eventMessage</span><span class="sxs-lookup"><span data-stu-id="77e6c-101">Get eventMessage</span></span>

<span data-ttu-id="77e6c-102">Получение свойств и связей объекта [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="77e6c-102">Retrieve the properties and relationships of [eventMessage](../resources/eventmessage.md) object.</span></span>

<span data-ttu-id="77e6c-103">В настоящее время эта операция возвращает текст сообщения о событии только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="77e6c-103">Currently, this operation returns event message bodies in only HTML format.</span></span>

## <a name="permissions"></a><span data-ttu-id="77e6c-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77e6c-104">Permissions</span></span>
<span data-ttu-id="77e6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="77e6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="77e6c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77e6c-107">Permission type</span></span>      | <span data-ttu-id="77e6c-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77e6c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77e6c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77e6c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="77e6c-110">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="77e6c-110">Mail.Read</span></span>    |
|<span data-ttu-id="77e6c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77e6c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77e6c-112">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="77e6c-112">Mail.Read</span></span>    |
|<span data-ttu-id="77e6c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77e6c-113">Application</span></span> | <span data-ttu-id="77e6c-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="77e6c-114">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="77e6c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77e6c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="77e6c-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="77e6c-116">Optional query parameters</span></span>
<span data-ttu-id="77e6c-117">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="77e6c-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="77e6c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77e6c-118">Request headers</span></span>
| <span data-ttu-id="77e6c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="77e6c-119">Name</span></span>       | <span data-ttu-id="77e6c-120">Тип</span><span class="sxs-lookup"><span data-stu-id="77e6c-120">Type</span></span> | <span data-ttu-id="77e6c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="77e6c-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="77e6c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="77e6c-122">Authorization</span></span>  | <span data-ttu-id="77e6c-123">string</span><span class="sxs-lookup"><span data-stu-id="77e6c-123">string</span></span>  | <span data-ttu-id="77e6c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77e6c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77e6c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77e6c-126">Request body</span></span>
<span data-ttu-id="77e6c-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="77e6c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77e6c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="77e6c-128">Response</span></span>

<span data-ttu-id="77e6c-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [eventMessage](../resources/eventmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77e6c-129">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="77e6c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="77e6c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77e6c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="77e6c-131">Request</span></span>
<span data-ttu-id="77e6c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77e6c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_eventmessage"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="77e6c-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="77e6c-133">Response</span></span>
<span data-ttu-id="77e6c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="77e6c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
