# <a name="get-message"></a><span data-ttu-id="55510-101">Получение message</span><span class="sxs-lookup"><span data-stu-id="55510-101">Get message</span></span>

<span data-ttu-id="55510-102">Получение свойств и связей объекта [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="55510-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="55510-103">Так как ресурс **message** поддерживает [расширения](../../../concepts/extensibility_overview.md), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="55510-103">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>

<span data-ttu-id="55510-104">В настоящее время эта операция возвращает текст сообщения только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="55510-104">Currently, this operation returns message bodies in only HTML format.</span></span>


### <a name="get-messages-in-another-users-message-folder"></a><span data-ttu-id="55510-105">Получение сообщений из папки другого пользователя</span><span class="sxs-lookup"><span data-stu-id="55510-105">Get messages in another user's message folder</span></span>

<span data-ttu-id="55510-106">Если у вас есть разрешения приложения или соответствующие делегированные [разрешения](#permissions) от одного пользователя, то вы можете получить сообщения из папки другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="55510-106">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get messages from another user's message folder.</span></span> <span data-ttu-id="55510-107">В этом разделе основное внимание уделено сценариям, в которых используются делегированные разрешения.</span><span class="sxs-lookup"><span data-stu-id="55510-107">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="55510-108">Например, ваше приложение получило делегированные разрешения от пользователя с именем Никита.</span><span class="sxs-lookup"><span data-stu-id="55510-108">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="55510-109">Предположим, что другой пользователь (Garth) поделился своей папкой сообщений с Никитой.</span><span class="sxs-lookup"><span data-stu-id="55510-109">Suppose another user, Garth, has shared a message folder with John.</span></span> <span data-ttu-id="55510-110">Вы можете получить сообщение из этой общей папки, указав идентификатор пользователя (или имя участника-пользователя) Garth, пример соответствующего запроса показан ниже.</span><span class="sxs-lookup"><span data-stu-id="55510-110">You can get a message in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/messages/{id}
```

<span data-ttu-id="55510-111">Эта возможность распространяется на все поддерживаемые операции GET над сообщениями для отдельного пользователя, как показано в приведенном ниже разделе [HTTP-запрос](#http-request).</span><span class="sxs-lookup"><span data-stu-id="55510-111">This capability applies to all the supported GET messages operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="55510-112">Она также применяется, если пользователь Garth делегировал разрешения на доступ ко всему своему почтовому ящику пользователю с именем Никита.</span><span class="sxs-lookup"><span data-stu-id="55510-112">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="55510-113">Если пользователь Garth не поделился своей папкой сообщений с Никитой и не делегировал этому пользователю разрешения на доступ к своему почтовому ящику, указав идентификатор пользователя или имя участника-пользователя Garth в этих операциях GET, будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="55510-113">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="55510-114">В таких случаях, указав идентификатор пользователя или имя участника-пользователя, можно получить только сообщение из папки пользователя, выполнившего вход, а запрос будет эквивалентен использованию ярлыка /me:</span><span class="sxs-lookup"><span data-stu-id="55510-114">In such cases, specifying a user ID or user principal name only works for getting a message in the signed-in user’s own message folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
```

<span data-ttu-id="55510-115">Эта возможность доступна только в операциях GET для следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="55510-115">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="55510-116">общие папки контактов, календари и папки сообщений;</span><span class="sxs-lookup"><span data-stu-id="55510-116">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="55510-117">контакты, события и сообщения в общих папках;</span><span class="sxs-lookup"><span data-stu-id="55510-117">Contacts, events, and messages in shared folders</span></span>
- <span data-ttu-id="55510-118">указанные выше ресурсы в тех почтовых ящиках, разрешения на доступ к которым делегированы.</span><span class="sxs-lookup"><span data-stu-id="55510-118">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="55510-119">Эта возможность недоступна для других операций над контактами, событиями, сообщениями и их папками.</span><span class="sxs-lookup"><span data-stu-id="55510-119">This capability is not available in other operations for contacts, events, messages, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="55510-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55510-120">Permissions</span></span>
<span data-ttu-id="55510-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="55510-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="55510-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55510-123">Permission type</span></span>      | <span data-ttu-id="55510-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55510-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55510-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55510-125">Delegated (work or school account)</span></span> | <span data-ttu-id="55510-126">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="55510-126">Mail.Read</span></span>    |
|<span data-ttu-id="55510-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55510-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55510-128">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="55510-128">Mail.Read</span></span>    |
|<span data-ttu-id="55510-129">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55510-129">Application</span></span> | <span data-ttu-id="55510-130">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="55510-130">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="55510-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55510-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="55510-132">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="55510-132">Optional query parameters</span></span>
<span data-ttu-id="55510-133">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="55510-133">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="55510-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55510-134">Request headers</span></span>
| <span data-ttu-id="55510-135">Имя</span><span class="sxs-lookup"><span data-stu-id="55510-135">Name</span></span>       | <span data-ttu-id="55510-136">Тип</span><span class="sxs-lookup"><span data-stu-id="55510-136">Type</span></span> | <span data-ttu-id="55510-137">Описание</span><span class="sxs-lookup"><span data-stu-id="55510-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="55510-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55510-138">Authorization</span></span>  | <span data-ttu-id="55510-139">string (строка)</span><span class="sxs-lookup"><span data-stu-id="55510-139">string</span></span>  | <span data-ttu-id="55510-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55510-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="55510-142">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="55510-142">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="55510-143">string (строка)</span><span class="sxs-lookup"><span data-stu-id="55510-143">string</span></span> | <span data-ttu-id="55510-144">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="55510-144">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="55510-145">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="55510-145">Values can be "text" or "html".</span></span> <span data-ttu-id="55510-146">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="55510-146">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="55510-147">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="55510-147">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="55510-148">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="55510-148">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55510-149">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="55510-149">Request body</span></span>
<span data-ttu-id="55510-150">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55510-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55510-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="55510-151">Response</span></span>

<span data-ttu-id="55510-152">В случае успеха этот метод возвращает код отклика `200 OK` и объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55510-152">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="55510-153">Пример</span><span class="sxs-lookup"><span data-stu-id="55510-153">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="55510-154">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="55510-154">Request 1</span></span>
<span data-ttu-id="55510-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55510-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
##### <a name="response-1"></a><span data-ttu-id="55510-156">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="55510-156">Response 1</span></span>
<span data-ttu-id="55510-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55510-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="55510-160">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="55510-160">Request 2</span></span>
<span data-ttu-id="55510-161">В следующем примере используются параметр `$select` для получения заголовков интернет-сообщений.</span><span class="sxs-lookup"><span data-stu-id="55510-161">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
##### <a name="response-2"></a><span data-ttu-id="55510-162">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="55510-162">Response 2</span></span>
<span data-ttu-id="55510-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="55510-163">Here is an example of the response.</span></span> <span data-ttu-id="55510-164">Примечание. Представленные здесь заголовки ответов объекта могут быть усечены для краткости.</span><span class="sxs-lookup"><span data-stu-id="55510-164">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="55510-165">При фактическом вызове будут возвращены все заголовки.</span><span class="sxs-lookup"><span data-stu-id="55510-165">All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="55510-166">См. также</span><span class="sxs-lookup"><span data-stu-id="55510-166">See also</span></span>

- [<span data-ttu-id="55510-167">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="55510-167">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="55510-168">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="55510-168">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
