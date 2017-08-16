# <a name="list-messages"></a><span data-ttu-id="73167-101">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="73167-101">List messages</span></span>

<span data-ttu-id="73167-102">Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные").</span><span class="sxs-lookup"><span data-stu-id="73167-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="73167-103">В настоящее время эта операция возвращает текст сообщения только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="73167-103">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73167-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="73167-104">Prerequisites</span></span>
<span data-ttu-id="73167-105">Для применения этого API требуется одна из указанных **областей**: *Mail.Read; Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="73167-105">One of the following scopes is required to execute this API: Mail.Read; Mail.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="73167-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73167-106">HTTP request</span></span>

<span data-ttu-id="73167-107">Для получения всех сообщений в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="73167-107">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="73167-108">Для получения сообщений из определенной папки в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="73167-108">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73167-109">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="73167-109">Optional query parameters</span></span>
<span data-ttu-id="73167-110">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="73167-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="73167-111">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73167-111">Request headers</span></span>
| <span data-ttu-id="73167-112">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73167-112">Header</span></span>       | <span data-ttu-id="73167-113">Значение</span><span class="sxs-lookup"><span data-stu-id="73167-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="73167-114">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73167-114">Authorization</span></span>  | <span data-ttu-id="73167-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73167-p101">Bearer {token}. Required.</span></span>  |
 

## <a name="request-body"></a><span data-ttu-id="73167-117">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73167-117">Request body</span></span>
<span data-ttu-id="73167-118">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73167-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73167-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="73167-119">Response</span></span>

<span data-ttu-id="73167-120">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73167-120">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="73167-121">Размер страницы по умолчанию для этого запроса предусматривает отображение 10 сообщений.</span><span class="sxs-lookup"><span data-stu-id="73167-121">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="73167-122">Пример</span><span class="sxs-lookup"><span data-stu-id="73167-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73167-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="73167-123">Request</span></span>
<span data-ttu-id="73167-124">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73167-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="73167-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="73167-125">Response</span></span>
<span data-ttu-id="73167-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="73167-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
