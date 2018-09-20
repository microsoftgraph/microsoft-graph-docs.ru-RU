# <a name="get-message"></a><span data-ttu-id="aa425-101">Получение message</span><span class="sxs-lookup"><span data-stu-id="aa425-101">Get message</span></span>

<span data-ttu-id="aa425-102">Получение свойств и связей объекта [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="aa425-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="aa425-103">В настоящее время эта операция возвращает текст сообщения только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="aa425-103">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="aa425-104">Существует два сценария, в которых приложения может получать сообщение в почтовую папку другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="aa425-104">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="aa425-105">Если программа имеет разрешения для приложения, или,</span><span class="sxs-lookup"><span data-stu-id="aa425-105">If the app has application permissions, or,</span></span>
* <span data-ttu-id="aa425-106">Если приложение имеет соответствующие делегированные [разрешения](#permissions) от одного пользователя и другой пользователь поделился календарем с этим пользователем или предоставил делегированный доступ к этому пользователю.</span><span class="sxs-lookup"><span data-stu-id="aa425-106">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="aa425-107">См. [сведения и примеры](../../../concepts/outlook-share-messages-folders.md).</span><span class="sxs-lookup"><span data-stu-id="aa425-107">See [details and an example](../../../concepts/outlook-share-messages-folders.md).</span></span>

<span data-ttu-id="aa425-108">Так как ресурс **message** поддерживает [расширения](../../../concepts/extensibility_overview.md), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="aa425-108">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="aa425-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa425-109">Permissions</span></span>
<span data-ttu-id="aa425-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aa425-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aa425-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa425-112">Permission type</span></span>      | <span data-ttu-id="aa425-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa425-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa425-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa425-114">Delegated (work or school account)</span></span> | <span data-ttu-id="aa425-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="aa425-115">Mail.Read</span></span>    |
|<span data-ttu-id="aa425-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa425-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa425-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="aa425-117">Mail.Read</span></span>    |
|<span data-ttu-id="aa425-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa425-118">Application</span></span> | <span data-ttu-id="aa425-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="aa425-119">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa425-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa425-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aa425-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aa425-121">Optional query parameters</span></span>
<span data-ttu-id="aa425-122">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aa425-122">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="aa425-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa425-123">Request headers</span></span>
| <span data-ttu-id="aa425-124">Имя</span><span class="sxs-lookup"><span data-stu-id="aa425-124">Name</span></span>       | <span data-ttu-id="aa425-125">Тип</span><span class="sxs-lookup"><span data-stu-id="aa425-125">Type</span></span> | <span data-ttu-id="aa425-126">Описание</span><span class="sxs-lookup"><span data-stu-id="aa425-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aa425-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa425-127">Authorization</span></span>  | <span data-ttu-id="aa425-128">строка</span><span class="sxs-lookup"><span data-stu-id="aa425-128">string</span></span>  | <span data-ttu-id="aa425-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa425-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aa425-131">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="aa425-131">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="aa425-132">строка</span><span class="sxs-lookup"><span data-stu-id="aa425-132">string</span></span> | <span data-ttu-id="aa425-133">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="aa425-133">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="aa425-134">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="aa425-134">Values can be "text" or "html".</span></span> <span data-ttu-id="aa425-135">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="aa425-135">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="aa425-136">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="aa425-136">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="aa425-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="aa425-137">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa425-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aa425-138">Request body</span></span>
<span data-ttu-id="aa425-139">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa425-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa425-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa425-140">Response</span></span>

<span data-ttu-id="aa425-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aa425-141">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aa425-142">Пример</span><span class="sxs-lookup"><span data-stu-id="aa425-142">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="aa425-143">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="aa425-143">Request 1</span></span>
<span data-ttu-id="aa425-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa425-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
##### <a name="response-1"></a><span data-ttu-id="aa425-145">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="aa425-145">Response 1</span></span>
<span data-ttu-id="aa425-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa425-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuZ\"",
    "id":"AAMkADhMGAAA=",
    "createdDateTime":"2018-09-09T03:15:05Z",
    "lastModifiedDateTime":"2018-09-09T03:15:08Z",
    "changeKey":"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuZ",
    "categories":[

    ],
    "receivedDateTime":"2018-09-09T03:15:08Z",
    "sentDateTime":"2018-09-09T03:15:06Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR6E1BE060@MWHPR1120.namprd22.prod.outlook.com>",
    "subject":"9/9/2018: concert",
    "bodyPreview":"The group represents Nevada.",
    "importance":"normal",
    "parentFolderId":"AAMkADcbAAAAAAEJAAA=",
    "conversationId":"AAQkADOUpag6yWs=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADMGAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThe group represents Nevada.\r\n</body>\r\n</html>\r\n"
    },
    "sender":{
        "emailAddress":{
            "name":"Adele Vance",
            "address":"adelev@contoso.OnMicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Adele Vance",
            "address":"adelev@contoso.OnMicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="aa425-149">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="aa425-149">Request 2</span></span>
<span data-ttu-id="aa425-150">В следующем примере используются параметр `$select` для получения заголовков интернет-сообщений.</span><span class="sxs-lookup"><span data-stu-id="aa425-150">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
##### <a name="response-2"></a><span data-ttu-id="aa425-151">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="aa425-151">Response 2</span></span>
<span data-ttu-id="aa425-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aa425-152">Here is an example of the response.</span></span> <span data-ttu-id="aa425-153">Примечание. Представленные здесь заголовки ответов объекта могут быть усечены для краткости.</span><span class="sxs-lookup"><span data-stu-id="aa425-153">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="aa425-154">При фактическом вызове будут возвращены все заголовки.</span><span class="sxs-lookup"><span data-stu-id="aa425-154">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages(internetMessageHeaders)/$entity",
    "@odata.etag":"W/\"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB\"",
    "id":"AAMkADhAAAW-VPeAAA=",
    "internetMessageHeaders":[
        {
            "name":"MIME-Version",
            "value":"1.0"
        },
        {
            "name":"Content-Type",
            "value":"multipart/report"
        },
        {
            "name":"x-custom-header-group-name",
            "value":"Washington"
        },
        {
            "name":"x-custom-header-group-id",
            "value":"WA001"
        }
    ]
}
```


## <a name="see-also"></a><span data-ttu-id="aa425-155">См. также</span><span class="sxs-lookup"><span data-stu-id="aa425-155">See also</span></span>

- [<span data-ttu-id="aa425-156">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="aa425-156">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="aa425-157">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="aa425-157">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
