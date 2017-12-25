# <a name="create-message"></a><span data-ttu-id="c32dd-101">Создание объекта Message</span><span class="sxs-lookup"><span data-stu-id="c32dd-101">Create Message</span></span>

<span data-ttu-id="c32dd-p101">С помощью этого API можно создать черновик нового сообщения. Черновики можно создавать в любой папке и при необходимости изменять перед отправкой. Для сохранения в папке "Черновики" используйте ярлык /messages.</span><span class="sxs-lookup"><span data-stu-id="c32dd-p101">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="c32dd-105">Создавая черновик, в тот же **POST**-запрос вы можете включить [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="c32dd-105">While creating the draft in the same **POST** call, you can include an [attachment](../resources/attachment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c32dd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c32dd-106">Permissions</span></span>
<span data-ttu-id="c32dd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c32dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c32dd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c32dd-109">Permission type</span></span>      | <span data-ttu-id="c32dd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c32dd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c32dd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c32dd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c32dd-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c32dd-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c32dd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c32dd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c32dd-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c32dd-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c32dd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c32dd-115">Application</span></span> | <span data-ttu-id="c32dd-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c32dd-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c32dd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c32dd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="c32dd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c32dd-118">Request headers</span></span>
| <span data-ttu-id="c32dd-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c32dd-119">Header</span></span>       | <span data-ttu-id="c32dd-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c32dd-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c32dd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c32dd-121">Authorization</span></span>  | <span data-ttu-id="c32dd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c32dd-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c32dd-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c32dd-124">Content-Type</span></span>  | <span data-ttu-id="c32dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c32dd-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c32dd-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c32dd-126">Request body</span></span>
<span data-ttu-id="c32dd-127">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c32dd-127">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

<span data-ttu-id="c32dd-128">Так как ресурс **message** поддерживает [расширения](../../../concepts/extensibility_overview.md), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными в сообщение при его создании.</span><span class="sxs-lookup"><span data-stu-id="c32dd-128">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="c32dd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c32dd-129">Response</span></span>

<span data-ttu-id="c32dd-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c32dd-130">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c32dd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c32dd-131">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="c32dd-132">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="c32dd-132">Request 1</span></span>
<span data-ttu-id="c32dd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c32dd-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
Content-type: application/json

{
    "subject":"Did you see last night's game?",
    "importance":"Low",
    "body":{
        "contentType":"HTML",
        "content":"They were <b>awesome</b>!"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ]
}
```
<span data-ttu-id="c32dd-134">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c32dd-134">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="c32dd-135">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="c32dd-135">Response 1</span></span>
<span data-ttu-id="c32dd-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c32dd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_message_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAABK4UfANE/UR5clSilZtIuWAAC1vdti\"",
    "id":"AAMkADNlNYjSAAA=",
    "createdDateTime":"2017-07-22T01:53:56Z",
    "lastModifiedDateTime":"2017-07-22T01:53:57Z",
    "changeKey":"CQAAABYAAABK4UfANE/UR5clSilZtIuWAAC1vdti",
    "categories":[

    ],
    "receivedDateTime":"2017-07-22T01:53:57Z",
    "sentDateTime":"2017-07-22T01:53:57Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR1301MB@MWHPR1301MB.namprd13.prod.outlook.com>",
    "subject":"Did you see last night's game?",
    "bodyPreview":"They were awesome!",
    "importance":"low",
    "parentFolderId":"AAMkADNlNWAAAAAAEPAAA=",
    "conversationId":"AAQkADNlNFdXGBnqtY=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADNlNYjSAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThey were <b>awesome</b>!\r\n</body>\r\n</html>\r\n"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Adele Vance",
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ]
}
```

## <a name="see-also"></a><span data-ttu-id="c32dd-139">См. также</span><span class="sxs-lookup"><span data-stu-id="c32dd-139">See also</span></span>

- [<span data-ttu-id="c32dd-140">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="c32dd-140">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="c32dd-141">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="c32dd-141">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
