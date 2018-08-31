# <a name="message-move"></a><span data-ttu-id="11ef8-101">message: move</span><span class="sxs-lookup"><span data-stu-id="11ef8-101">message: move</span></span>

<span data-ttu-id="11ef8-102">Перемещение сообщения в папку.</span><span class="sxs-lookup"><span data-stu-id="11ef8-102">Move a DriveItem to a new folder</span></span> <span data-ttu-id="11ef8-103">Это создает новую копию сообщения в папке назначения и удаляет исходное сообщение.</span><span class="sxs-lookup"><span data-stu-id="11ef8-103">Move the message to a folder. This creates a new copy of the message in the destination folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="11ef8-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11ef8-104">Permissions</span></span>

<span data-ttu-id="11ef8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="11ef8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="11ef8-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11ef8-107">Permission type</span></span> | <span data-ttu-id="11ef8-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11ef8-108">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="11ef8-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11ef8-109">Delegated (work or school account)</span></span> | <span data-ttu-id="11ef8-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11ef8-110">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="11ef8-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11ef8-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11ef8-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11ef8-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="11ef8-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11ef8-113">Application</span></span> | <span data-ttu-id="11ef8-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11ef8-114">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="11ef8-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11ef8-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="11ef8-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11ef8-116">Request headers</span></span>

| <span data-ttu-id="11ef8-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11ef8-117">Header</span></span> | <span data-ttu-id="11ef8-118">Значение</span><span class="sxs-lookup"><span data-stu-id="11ef8-118">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="11ef8-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11ef8-119">Authorization</span></span> | <span data-ttu-id="11ef8-120">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="11ef8-120"></span></span> <span data-ttu-id="11ef8-121">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11ef8-121">Required.</span></span> |
| <span data-ttu-id="11ef8-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11ef8-122">Content-Type</span></span> | <span data-ttu-id="11ef8-123">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="11ef8-123"></span></span> <span data-ttu-id="11ef8-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11ef8-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11ef8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11ef8-125">Request body</span></span>

<span data-ttu-id="11ef8-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="11ef8-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="11ef8-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="11ef8-127">Parameter</span></span>   | <span data-ttu-id="11ef8-128">Тип</span><span class="sxs-lookup"><span data-stu-id="11ef8-128">Type</span></span> |<span data-ttu-id="11ef8-129">Описание</span><span class="sxs-lookup"><span data-stu-id="11ef8-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11ef8-130">destinationId</span><span class="sxs-lookup"><span data-stu-id="11ef8-130">destinationId</span></span>|<span data-ttu-id="11ef8-131">String (строка)</span><span class="sxs-lookup"><span data-stu-id="11ef8-131">String</span></span>|<span data-ttu-id="11ef8-132">Идентификатор целевой папки либо имя известной папки.</span><span class="sxs-lookup"><span data-stu-id="11ef8-132">The destination folder ID, or the , , , or  well-known folder name.</span></span> <span data-ttu-id="11ef8-133">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="11ef8-133">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="11ef8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="11ef8-134">Response</span></span>

<span data-ttu-id="11ef8-135">При успешном выполнении этот метод возвращает код отклика `201 Created` и ресурс [сообщения](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="11ef8-135">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11ef8-136">Пример</span><span class="sxs-lookup"><span data-stu-id="11ef8-136">Example</span></span>

<span data-ttu-id="11ef8-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="11ef8-137">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="11ef8-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="11ef8-138">Request</span></span>

<span data-ttu-id="11ef8-139">Следующий запрос перемещает указанное сообщение в папку «Удаленные», определенную известным именем папки `deleteditems`.</span><span class="sxs-lookup"><span data-stu-id="11ef8-139">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAATs28OAAA="],
  "name": "message_move"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAATs28OAAA=/move
Content-type: application/json

{
  "destinationId": "deleteditems"
}
```

##### <a name="response"></a><span data-ttu-id="11ef8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="11ef8-140">Response</span></span>

<span data-ttu-id="11ef8-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="11ef8-141">Here is an example of the response.</span></span>

> <span data-ttu-id="11ef8-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11ef8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#message",
    "@odata.type":"#microsoft.graph.message",
    "@odata.etag":"W/\"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB\"",
    "id":"AAMkADhAAAW-VPeAAA=",
    "createdDateTime":"2018-08-12T08:43:22Z",
    "lastModifiedDateTime":"2018-08-15T19:47:54Z",
    "changeKey":"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB",
    "categories":[

    ],
    "receivedDateTime":"2018-08-12T08:43:22Z",
    "sentDateTime":"2018-08-12T08:43:20Z",
    "hasAttachments":false,
    "internetMessageId":"<00535324-5988-4b6a-b9af-d44cf2d0b691@MWHPR2201MB1022.namprd22.prod.outlook.com>",
    "subject":"Undeliverable: Meet for lunch?",
    "bodyPreview":"Delivery has failed to these recipients or groups:\r\n\r\nfannyd@contoso.onmicrosoft.com (fannyd@contoso.onmicrosoft.com)\r\nYour message couldn't be delivered. Despite repeated attempts to deliver your message, querying the Domain Name System (DNS) for the rec",
    "importance":"normal",
    "parentFolderId":"AAMkADhAAAAAAEKAAA=",
    "conversationId":"AAQkADhJzfbkARFhe5kKhjihSA=",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADhAAAW%2FVPeAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html></html>"
    },
    "sender":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"fannyd@contoso.onmicrosoft.com",
                "address":"fannyd@contoso.onmicrosoft.com"
            }
        },
        {
            "emailAddress":{
                "name":"danas@contoso.onmicrosoft.com",
                "address":"danas@contoso.onmicrosoft.com"
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
