# <a name="list-messages"></a><span data-ttu-id="43c2f-101">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="43c2f-101">List messages</span></span>

<span data-ttu-id="43c2f-102">Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные").</span><span class="sxs-lookup"><span data-stu-id="43c2f-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="43c2f-103">В настоящее время эта операция возвращает текст сообщения только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="43c2f-103">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="43c2f-104">Существует два сценария, в которых приложение может получать сообщения в почтовой папке другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="43c2f-104">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="43c2f-105">Если программа имеет разрешения для приложения, или,</span><span class="sxs-lookup"><span data-stu-id="43c2f-105">If the app has application permissions, or,</span></span>
* <span data-ttu-id="43c2f-106">Если приложение имеет соответствующие делегированные [разрешения](#permissions) от одного пользователя и другой пользователь поделился календарем с этим пользователем или предоставил делегированный доступ к этому пользователю.</span><span class="sxs-lookup"><span data-stu-id="43c2f-106">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="43c2f-107">См. [сведения и примеры](../../../concepts/outlook-share-messages-folders.md).</span><span class="sxs-lookup"><span data-stu-id="43c2f-107">See [details and an example](../../../concepts/outlook-share-messages-folders.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="43c2f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="43c2f-108">Permissions</span></span>
<span data-ttu-id="43c2f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="43c2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="43c2f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43c2f-111">Permission type</span></span>      | <span data-ttu-id="43c2f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43c2f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43c2f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43c2f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="43c2f-114">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43c2f-114">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="43c2f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43c2f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43c2f-116">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43c2f-116">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="43c2f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43c2f-117">Application</span></span> | <span data-ttu-id="43c2f-118">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43c2f-118">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="43c2f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43c2f-119">HTTP request</span></span>

<span data-ttu-id="43c2f-120">Для получения всех сообщений в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="43c2f-120">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="43c2f-121">Для получения сообщений из определенной папки в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="43c2f-121">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43c2f-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="43c2f-122">Optional query parameters</span></span>
<span data-ttu-id="43c2f-123">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="43c2f-123">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="43c2f-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43c2f-124">Request headers</span></span>
| <span data-ttu-id="43c2f-125">Имя</span><span class="sxs-lookup"><span data-stu-id="43c2f-125">Name</span></span>       | <span data-ttu-id="43c2f-126">Тип</span><span class="sxs-lookup"><span data-stu-id="43c2f-126">Type</span></span> | <span data-ttu-id="43c2f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="43c2f-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="43c2f-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43c2f-128">Authorization</span></span>  | <span data-ttu-id="43c2f-129">строка</span><span class="sxs-lookup"><span data-stu-id="43c2f-129">string</span></span>  | <span data-ttu-id="43c2f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43c2f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="43c2f-132">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="43c2f-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="43c2f-133">string</span><span class="sxs-lookup"><span data-stu-id="43c2f-133">string</span></span> | <span data-ttu-id="43c2f-134">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="43c2f-134">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="43c2f-135">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="43c2f-135">Values can be "text" or "html".</span></span> <span data-ttu-id="43c2f-136">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="43c2f-136">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="43c2f-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="43c2f-137">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="43c2f-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="43c2f-138">Request body</span></span>
<span data-ttu-id="43c2f-139">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43c2f-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43c2f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="43c2f-140">Response</span></span>

<span data-ttu-id="43c2f-141">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="43c2f-141">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="43c2f-142">Размер страницы по умолчанию для этого запроса предусматривает отображение 10 сообщений.</span><span class="sxs-lookup"><span data-stu-id="43c2f-142">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="43c2f-143">Пример</span><span class="sxs-lookup"><span data-stu-id="43c2f-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="43c2f-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="43c2f-144">Request</span></span>
<span data-ttu-id="43c2f-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43c2f-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="43c2f-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="43c2f-146">Response</span></span>
<span data-ttu-id="43c2f-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43c2f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
