# <a name="get-message"></a><span data-ttu-id="15570-101">Получение message</span><span class="sxs-lookup"><span data-stu-id="15570-101">Get message</span></span>

<span data-ttu-id="15570-102">Получение свойств и связей объекта [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="15570-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="15570-103">Так как ресурс **message** поддерживает [расширения](../../../concepts/extensibility_overview.md), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="15570-103">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>

<span data-ttu-id="15570-104">В настоящее время эта операция возвращает текст сообщения только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="15570-104">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15570-105">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="15570-105">Prerequisites</span></span>
<span data-ttu-id="15570-106">Для применения этого API требуется одна из указанных **областей**: *Mail.Read*</span><span class="sxs-lookup"><span data-stu-id="15570-106">One of the following **scopes** is required to execute this API: *Mail.Read*</span></span>  
## <a name="http-request"></a><span data-ttu-id="15570-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15570-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="15570-108">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="15570-108">Optional query parameters</span></span>
<span data-ttu-id="15570-109">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="15570-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="15570-110">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15570-110">Request headers</span></span>
| <span data-ttu-id="15570-111">Имя</span><span class="sxs-lookup"><span data-stu-id="15570-111">Name</span></span>       | <span data-ttu-id="15570-112">Тип</span><span class="sxs-lookup"><span data-stu-id="15570-112">Type</span></span> | <span data-ttu-id="15570-113">Описание</span><span class="sxs-lookup"><span data-stu-id="15570-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="15570-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="15570-114">Authorization</span></span>  | <span data-ttu-id="15570-115">string</span><span class="sxs-lookup"><span data-stu-id="15570-115">string</span></span>  | <span data-ttu-id="15570-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15570-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15570-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15570-118">Request body</span></span>
<span data-ttu-id="15570-119">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="15570-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15570-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="15570-120">Response</span></span>

<span data-ttu-id="15570-121">В случае успеха этот метод возвращает код отклика `200 OK` и объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15570-121">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="15570-122">Пример</span><span class="sxs-lookup"><span data-stu-id="15570-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15570-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="15570-123">Request</span></span>
<span data-ttu-id="15570-124">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15570-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="15570-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="15570-125">Response</span></span>
<span data-ttu-id="15570-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="15570-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
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
  "bodyPreview": "bodyPreview-value"
}
```

## <a name="see-also"></a><span data-ttu-id="15570-129">См. также</span><span class="sxs-lookup"><span data-stu-id="15570-129">See also</span></span>

- [<span data-ttu-id="15570-130">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="15570-130">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="15570-131">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="15570-131">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
