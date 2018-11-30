---
title: Создание объекта Message
description: С помощью этого API можно создать черновик нового сообщения. Черновики можно создавать в любой папке и при необходимости изменять перед отправкой. Для сохранения в папке "Черновики" используйте ярлык /messages.
ms.openlocfilehash: 21a5f9dc54afdbfd6298841f1f441a78103ab28c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077075"
---
# <a name="create-message"></a><span data-ttu-id="4886e-105">Создание объекта Message</span><span class="sxs-lookup"><span data-stu-id="4886e-105">Create Message</span></span>

> <span data-ttu-id="4886e-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4886e-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4886e-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4886e-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4886e-p103">С помощью этого API можно создать черновик нового сообщения. Черновики можно создавать в любой папке и при необходимости изменять перед отправкой. Для сохранения в папке "Черновики" используйте ярлык /messages.</span><span class="sxs-lookup"><span data-stu-id="4886e-p103">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="4886e-111">При создании черновик в одном вызове **POST** , можно выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="4886e-111">While creating the draft in the same **POST** call, you can:</span></span>

- <span data-ttu-id="4886e-112">Включить [вложения](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="4886e-112">Include an [attachment](../resources/attachment.md)</span></span> 
- <span data-ttu-id="4886e-113">Используйте [упомянуть](../resources/mention.md) помечать другого пользователя в новое сообщение</span><span class="sxs-lookup"><span data-stu-id="4886e-113">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="4886e-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4886e-114">Permissions</span></span>
<span data-ttu-id="4886e-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4886e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4886e-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4886e-117">Permission type</span></span>      | <span data-ttu-id="4886e-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4886e-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4886e-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4886e-119">Delegated (work or school account)</span></span> | <span data-ttu-id="4886e-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4886e-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4886e-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4886e-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4886e-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4886e-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4886e-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4886e-123">Application</span></span> | <span data-ttu-id="4886e-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4886e-124">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4886e-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4886e-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="4886e-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4886e-126">Request headers</span></span>
| <span data-ttu-id="4886e-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4886e-127">Header</span></span>       | <span data-ttu-id="4886e-128">Значение</span><span class="sxs-lookup"><span data-stu-id="4886e-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4886e-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4886e-129">Authorization</span></span>  | <span data-ttu-id="4886e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4886e-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4886e-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4886e-132">Content-Type</span></span>  | <span data-ttu-id="4886e-133">application/json</span><span class="sxs-lookup"><span data-stu-id="4886e-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4886e-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4886e-134">Request body</span></span>
<span data-ttu-id="4886e-135">В тексте запроса укажите представление объекта [message](../resources/message.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="4886e-135">In the request body, supply a JSON representation of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="4886e-136">Если вы хотите использовать **упомянуть** помечать другого пользователя в новое сообщение:</span><span class="sxs-lookup"><span data-stu-id="4886e-136">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="4886e-137">Включите свойства необходимые **toRecipients** , свойство **упоминания** и все свойства для записи сообщений в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="4886e-137">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="4886e-138">Для каждого упоминаются в свойстве **упоминания** необходимо указать свойство **упомянутые** .</span><span class="sxs-lookup"><span data-stu-id="4886e-138">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="4886e-139">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными в сообщение при его создании.</span><span class="sxs-lookup"><span data-stu-id="4886e-139">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="4886e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4886e-140">Response</span></span>

<span data-ttu-id="4886e-141">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [сообщения](../resources/message.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4886e-141">If successful, this method returns a `201 Created` response code and a [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4886e-142">Пример</span><span class="sxs-lookup"><span data-stu-id="4886e-142">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="4886e-143">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="4886e-143">Request 1</span></span>
<span data-ttu-id="4886e-144">Ниже приведен пример запроса на создание черновика нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="4886e-144">Here is an example of the request to create a draft of a new message.</span></span>
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
<span data-ttu-id="4886e-145">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4886e-145">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="4886e-146">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="4886e-146">Response 1</span></span>
<span data-ttu-id="4886e-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4886e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="4886e-150">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="4886e-150">Request 2</span></span>
<span data-ttu-id="4886e-151">В следующем примере показаны по электронной почте черновиков с Randi Welch для Samantha стенда.</span><span class="sxs-lookup"><span data-stu-id="4886e-151">The next example shows a draft email by Randi Welch to Samantha Booth.</span></span> <span data-ttu-id="4886e-152">Сообщение также включает в себя упоминание другому пользователю, Swope Дану.</span><span class="sxs-lookup"><span data-stu-id="4886e-152">The message also includes a mention of another user, Dana Swope.</span></span>

<span data-ttu-id="4886e-153">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4886e-153">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
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


##### <a name="response-2"></a><span data-ttu-id="4886e-154">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="4886e-154">Response 2</span></span>
<span data-ttu-id="4886e-p108">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4886e-p108">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-3"></a><span data-ttu-id="4886e-158">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="4886e-158">Request 3</span></span>
<span data-ttu-id="4886e-159">Следующий пример добавляет несколько заголовков сообщений Интернета клиента при создании черновика сообщения.</span><span class="sxs-lookup"><span data-stu-id="4886e-159">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>
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
<span data-ttu-id="4886e-160">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4886e-160">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-3"></a><span data-ttu-id="4886e-161">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="4886e-161">Response 3</span></span>
<span data-ttu-id="4886e-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4886e-162">Here is an example of the response.</span></span> <span data-ttu-id="4886e-163">Примечание: Заголовки сообщений Интернета не возвращаются в ответа POST по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4886e-163">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="4886e-164">Объект ответа, показанный здесь также может усекаться для краткости.</span><span class="sxs-lookup"><span data-stu-id="4886e-164">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="4886e-165">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4886e-165">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="4886e-166">См. также</span><span class="sxs-lookup"><span data-stu-id="4886e-166">See also</span></span>

- [<span data-ttu-id="4886e-167">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="4886e-167">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4886e-168">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="4886e-168">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="4886e-169">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="4886e-169">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
