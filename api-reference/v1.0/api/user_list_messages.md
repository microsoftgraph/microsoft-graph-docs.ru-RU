# <a name="list-messages"></a><span data-ttu-id="8609d-101">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="8609d-101">List messages</span></span>

<span data-ttu-id="8609d-102">Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные").</span><span class="sxs-lookup"><span data-stu-id="8609d-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="8609d-103">В настоящее время эта операция возвращает текст сообщения только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="8609d-103">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="permissions"></a><span data-ttu-id="8609d-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8609d-104">Permissions</span></span>
<span data-ttu-id="8609d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8609d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8609d-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8609d-107">Permission type</span></span>      | <span data-ttu-id="8609d-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8609d-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8609d-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8609d-109">Delegated (work or school account)</span></span> | <span data-ttu-id="8609d-110">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8609d-110">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8609d-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8609d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8609d-112">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8609d-112">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8609d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8609d-113">Application</span></span> | <span data-ttu-id="8609d-114">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8609d-114">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8609d-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8609d-115">HTTP request</span></span>

<span data-ttu-id="8609d-116">Для получения всех сообщений в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="8609d-116">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="8609d-117">Для получения сообщений из определенной папки в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="8609d-117">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8609d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8609d-118">Optional query parameters</span></span>
<span data-ttu-id="8609d-119">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8609d-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8609d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8609d-120">Request headers</span></span>
| <span data-ttu-id="8609d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8609d-121">Header</span></span>       | <span data-ttu-id="8609d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8609d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8609d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8609d-123">Authorization</span></span>  | <span data-ttu-id="8609d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8609d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8609d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8609d-126">Request body</span></span>
<span data-ttu-id="8609d-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8609d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8609d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8609d-128">Response</span></span>

<span data-ttu-id="8609d-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8609d-129">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="8609d-130">Размер страницы по умолчанию для этого запроса предусматривает отображение 10 сообщений.</span><span class="sxs-lookup"><span data-stu-id="8609d-130">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="8609d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8609d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8609d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8609d-132">Request</span></span>
<span data-ttu-id="8609d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8609d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="8609d-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="8609d-134">Response</span></span>
<span data-ttu-id="8609d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8609d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
