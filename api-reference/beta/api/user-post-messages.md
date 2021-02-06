---
title: Создание объекта Message
description: С помощью этого API можно создать черновик нового сообщения. Черновики можно создавать в любой папке и при необходимости изменять перед отправкой. Для сохранения в папке "Черновики" используйте ярлык /messages.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fcf8ad8a4b8016f972ee8844a959d0a3359a2db9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135165"
---
# <a name="create-message"></a><span data-ttu-id="e1b11-105">Создание объекта Message</span><span class="sxs-lookup"><span data-stu-id="e1b11-105">Create Message</span></span>

<span data-ttu-id="e1b11-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1b11-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1b11-p102">С помощью этого API можно создать черновик нового сообщения. Черновики можно создавать в любой папке и при необходимости изменять перед отправкой. Для сохранения в папке "Черновики" используйте ярлык /messages.</span><span class="sxs-lookup"><span data-stu-id="e1b11-p102">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="e1b11-110">Создавая черновик в одном вызове **POST,** вы можете:</span><span class="sxs-lookup"><span data-stu-id="e1b11-110">While creating the draft in the same **POST** call, you can:</span></span>

- <span data-ttu-id="e1b11-111">Включить [вложение](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="e1b11-111">Include an [attachment](../resources/attachment.md)</span></span> 
- <span data-ttu-id="e1b11-112">Использование упоминания [для](../resources/mention.md) вызова другого пользователя в новом сообщении</span><span class="sxs-lookup"><span data-stu-id="e1b11-112">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="e1b11-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1b11-113">Permissions</span></span>
<span data-ttu-id="e1b11-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1b11-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1b11-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1b11-116">Permission type</span></span>      | <span data-ttu-id="e1b11-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1b11-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1b11-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1b11-118">Delegated (work or school account)</span></span> | <span data-ttu-id="e1b11-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1b11-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e1b11-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1b11-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1b11-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1b11-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e1b11-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1b11-122">Application</span></span> | <span data-ttu-id="e1b11-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1b11-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1b11-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1b11-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="e1b11-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1b11-125">Request headers</span></span>
| <span data-ttu-id="e1b11-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1b11-126">Header</span></span>       | <span data-ttu-id="e1b11-127">Значение</span><span class="sxs-lookup"><span data-stu-id="e1b11-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e1b11-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1b11-128">Authorization</span></span>  | <span data-ttu-id="e1b11-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1b11-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e1b11-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1b11-131">Content-Type</span></span>  | <span data-ttu-id="e1b11-132">application/json</span><span class="sxs-lookup"><span data-stu-id="e1b11-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e1b11-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1b11-133">Request body</span></span>
<span data-ttu-id="e1b11-134">В тексте запроса укажу представление объекта [сообщения](../resources/message.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="e1b11-134">In the request body, supply a JSON representation of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="e1b11-135">Если вы хотите использовать **упоминание** для вызова другого пользователя в новом сообщении:</span><span class="sxs-lookup"><span data-stu-id="e1b11-135">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="e1b11-136">Включит в текст запроса обязательное свойство **toRecipients,** свойство **упоминаний** и любые свойства сообщений, которые можно писать.</span><span class="sxs-lookup"><span data-stu-id="e1b11-136">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="e1b11-137">Для каждого упоминания в **свойстве упоминаний** необходимо указать **упомянутое** свойство.</span><span class="sxs-lookup"><span data-stu-id="e1b11-137">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="e1b11-138">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными в сообщение при его создании.</span><span class="sxs-lookup"><span data-stu-id="e1b11-138">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="e1b11-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1b11-139">Response</span></span>

<span data-ttu-id="e1b11-140">В случае успеха этот метод возвращает код отклика и `201 Created` [объект сообщения](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1b11-140">If successful, this method returns a `201 Created` response code and a [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1b11-141">Пример</span><span class="sxs-lookup"><span data-stu-id="e1b11-141">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e1b11-142">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="e1b11-142">Request 1</span></span>
<span data-ttu-id="e1b11-143">Вот пример запроса на создание черновика нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="e1b11-143">Here is an example of the request to create a draft of a new message.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1b11-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1b11-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
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
# <a name="c"></a>[<span data-ttu-id="e1b11-145">C#</span><span class="sxs-lookup"><span data-stu-id="e1b11-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1b11-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1b11-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1b11-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1b11-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1b11-148">Java</span><span class="sxs-lookup"><span data-stu-id="e1b11-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e1b11-149">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1b11-149">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="e1b11-150">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="e1b11-150">Response 1</span></span>
<span data-ttu-id="e1b11-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e1b11-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('ad787b4f-1fda-4523-8e48-ffedb7f4635f')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAAmXr9SsE/UR4PcnTZcg7qWAAAFS12t\"",
    "id":"AAMkAGRWAAAFSmKXAAA=",
    "createdDateTime":"2017-12-23T07:29:57Z",
    "lastModifiedDateTime":"2017-12-23T07:29:58Z",
    "changeKey":"CQAAABYAAAAmXr9SsE/UR4PcnTZcg7qWAAAFS12t",
    "categories":[

    ],
    "receivedDateTime":"2017-12-23T07:29:58Z",
    "sentDateTime":"2017-12-23T07:29:58Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR130@MWHPR130.namprd13.prod.outlook.com>",
    "subject":"Did you see last night's game?",
    "bodyPreview":"They were awesome!",
    "importance":"low",
    "parentFolderId":"AAMkAGRWAAAAAAEPAAA=",
    "conversationId":"AAQkAGRVYAsRJrRdc_mWNaxU=",
    "conversationIndex":"AQHTe7/VAniOJVgCxEmtF1z6ZY1rFQ==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkAGRWAAAFSmKXAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "mentionsPreview":null,
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThey were <b>awesome</b>!\r\n</body>\r\n</html>\r\n"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"AdeleV@contoso.onmicrosoft.com",
                "address":"AdeleV@contoso.onmicrosoft.com"
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

##### <a name="request-2"></a><span data-ttu-id="e1b11-154">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="e1b11-154">Request 2</span></span>
<span data-ttu-id="e1b11-155">В следующем примере показан черновик сообщения от Randi Welch к Samantha Чтобы отправить сообщение.</span><span class="sxs-lookup"><span data-stu-id="e1b11-155">The next example shows a draft email by Randi Welch to Samantha Booth.</span></span> <span data-ttu-id="e1b11-156">Сообщение также содержит упоминание другого пользователя, Dana Swope.</span><span class="sxs-lookup"><span data-stu-id="e1b11-156">The message also includes a mention of another user, Dana Swope.</span></span>

<span data-ttu-id="e1b11-157">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1b11-157">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1b11-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1b11-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_with_mentions_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
Content-type: application/json

{
    "subject": "Party planning",
    "toRecipients":[
      {
          "emailAddress":{
              "name":"Samantha Booth",
              "address":"samanthab@contoso.onmicrosoft.com"
          }
      }
    ],
    "mentions":[
      {    
        "mentioned":{
          "name":"Dana Swope",
          "address":"danas@contoso.onmicrosoft.com"
         }
      }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="e1b11-159">C#</span><span class="sxs-lookup"><span data-stu-id="e1b11-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-with-mentions-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1b11-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1b11-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-with-mentions-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1b11-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1b11-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-with-mentions-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1b11-162">Java</span><span class="sxs-lookup"><span data-stu-id="e1b11-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-with-mentions-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response-2"></a><span data-ttu-id="e1b11-163">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="e1b11-163">Response 2</span></span>
<span data-ttu-id="e1b11-p107">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1b11-p107">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/Messages/$entity",
  "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAW1fsAAAAA==')",
  "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAbYj7\"",
  "id":"AQMkADJmMTUAAAW1fsAAAAA==",
  "body":{
    "contentType":"Text",
    "content":""
  },
  "bodyPreview":"",
  "sender":null,
  "from":null,
  "subject": "Party planning",
  "toRecipients":[
    {
      "emailAddress":{
        "name":"Samantha Booth",
        "address":"samanthab@contoso.onmicrosoft.com"
      }
    }
  ],
  "mentionsPreview":{
    "isMentioned":false
  },
  "mentions@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages('AQMkADJmMTUAAAW1fsAAAAA%3D%3D')/mentions",
  "mentions":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAW1fsAAAAA==')/mentions('4577bba4-b063-4cea-9073-6f7ca815fcec')",
      "id":"4577bba4-b063-4cea-9073-6f7ca815fcec",
      "mentioned":{
        "name":"Dana Swope",
        "address":"danas@contoso.onmicrosoft.com"
      },
      "mentionText":null,
      "clientReference":null,
      "createdBy":{
        "name":"Randi Welch",
        "address":"randiw@contoso.onmicrosoft.com"
      },
      "createdDateTime":"2016-07-22T02:22:44Z",
      "serverCreatedDateTime":"2016-07-22T02:22:44.201Z",
      "deepLink":null,
      "application":null
    }
  ]
}

```

##### <a name="request-3"></a><span data-ttu-id="e1b11-167">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="e1b11-167">Request 3</span></span>
<span data-ttu-id="e1b11-168">В следующем примере добавляется пара пользовательских заголовков сообщений Интернета при создании черновика сообщения.</span><span class="sxs-lookup"><span data-stu-id="e1b11-168">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1b11-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1b11-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_with_headers_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
Content-type: application/json

{
    "subject":"9/8/2018: concert",
    "body":{
        "contentType":"HTML",
        "content":"The group represents Washington."
    },
    "toRecipients":[
        {
            "emailAddress":{
                "address":"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "internetMessageHeaders":[
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
# <a name="c"></a>[<span data-ttu-id="e1b11-170">C#</span><span class="sxs-lookup"><span data-stu-id="e1b11-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-with-headers-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1b11-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1b11-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-with-headers-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1b11-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1b11-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-with-headers-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1b11-173">Java</span><span class="sxs-lookup"><span data-stu-id="e1b11-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-with-headers-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e1b11-174">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1b11-174">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-3"></a><span data-ttu-id="e1b11-175">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="e1b11-175">Response 3</span></span>
<span data-ttu-id="e1b11-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e1b11-176">Here is an example of the response.</span></span> <span data-ttu-id="e1b11-177">Примечание. Заголовки сообщений Интернета не возвращаются по умолчанию в ответе POST.</span><span class="sxs-lookup"><span data-stu-id="e1b11-177">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="e1b11-178">Примечание. Представленный здесь объект отклика также может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="e1b11-178">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="e1b11-179">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1b11-179">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_message_with_headers_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuE\"",
    "id":"AAMkADhNmAAA=",
    "createdDateTime":"2018-09-09T02:54:56Z",
    "lastModifiedDateTime":"2018-09-09T02:54:56Z",
    "changeKey":"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuE",
    "categories":[

    ],
    "receivedDateTime":"2018-09-09T02:54:56Z",
    "sentDateTime":"2018-09-09T02:54:56Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR220MB1120.namprd22.prod.outlook.com>",
    "subject":"9/8/2018: concert",
    "bodyPreview":"The group represents Washington.",
    "importance":"normal",
    "parentFolderId":"AAMkADhAAAAAAEPAAA=",
    "conversationId":"AAQkADhNCuP8OKSm-0NE=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADhNmAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "mentionsPreview":null,
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThe group represents Washington.\r\n</body>\r\n</html>\r\n"
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

## <a name="see-also"></a><span data-ttu-id="e1b11-180">См. также</span><span class="sxs-lookup"><span data-stu-id="e1b11-180">See also</span></span>

- [<span data-ttu-id="e1b11-181">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="e1b11-181">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e1b11-182">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e1b11-182">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="e1b11-183">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e1b11-183">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


