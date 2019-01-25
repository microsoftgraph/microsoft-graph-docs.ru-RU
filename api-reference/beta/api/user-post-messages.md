---
title: Создание объекта Message
description: С помощью этого API можно создать черновик нового сообщения. Черновики можно создавать в любой папке и при необходимости изменять перед отправкой. Для сохранения в папке "Черновики" используйте ярлык /messages.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4c15bfc0a29909b1e7a7ba27b5ac221c0d11f815
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509751"
---
# <a name="create-message"></a><span data-ttu-id="a13b9-105">Создание объекта Message</span><span class="sxs-lookup"><span data-stu-id="a13b9-105">Create Message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a13b9-p102">С помощью этого API можно создать черновик нового сообщения. Черновики можно создавать в любой папке и при необходимости изменять перед отправкой. Для сохранения в папке "Черновики" используйте ярлык /messages.</span><span class="sxs-lookup"><span data-stu-id="a13b9-p102">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="a13b9-109">При создании черновик в одном вызове **POST** , можно выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="a13b9-109">While creating the draft in the same **POST** call, you can:</span></span>

- <span data-ttu-id="a13b9-110">Включить [вложения](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="a13b9-110">Include an [attachment](../resources/attachment.md)</span></span> 
- <span data-ttu-id="a13b9-111">Используйте [упомянуть](../resources/mention.md) помечать другого пользователя в новое сообщение</span><span class="sxs-lookup"><span data-stu-id="a13b9-111">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="a13b9-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a13b9-112">Permissions</span></span>
<span data-ttu-id="a13b9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a13b9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a13b9-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a13b9-115">Permission type</span></span>      | <span data-ttu-id="a13b9-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a13b9-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a13b9-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a13b9-117">Delegated (work or school account)</span></span> | <span data-ttu-id="a13b9-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a13b9-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a13b9-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a13b9-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a13b9-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a13b9-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a13b9-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a13b9-121">Application</span></span> | <span data-ttu-id="a13b9-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a13b9-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a13b9-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a13b9-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="a13b9-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a13b9-124">Request headers</span></span>
| <span data-ttu-id="a13b9-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a13b9-125">Header</span></span>       | <span data-ttu-id="a13b9-126">Значение</span><span class="sxs-lookup"><span data-stu-id="a13b9-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a13b9-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a13b9-127">Authorization</span></span>  | <span data-ttu-id="a13b9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a13b9-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a13b9-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a13b9-130">Content-Type</span></span>  | <span data-ttu-id="a13b9-131">application/json</span><span class="sxs-lookup"><span data-stu-id="a13b9-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a13b9-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a13b9-132">Request body</span></span>
<span data-ttu-id="a13b9-133">В тексте запроса укажите представление объекта [message](../resources/message.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="a13b9-133">In the request body, supply a JSON representation of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="a13b9-134">Если вы хотите использовать **упомянуть** помечать другого пользователя в новое сообщение:</span><span class="sxs-lookup"><span data-stu-id="a13b9-134">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="a13b9-135">Включите свойства необходимые **toRecipients** , свойство **упоминания** и все свойства для записи сообщений в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="a13b9-135">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="a13b9-136">Для каждого упоминаются в свойстве **упоминания** необходимо указать свойство **упомянутые** .</span><span class="sxs-lookup"><span data-stu-id="a13b9-136">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="a13b9-137">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными в сообщение при его создании.</span><span class="sxs-lookup"><span data-stu-id="a13b9-137">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="a13b9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a13b9-138">Response</span></span>

<span data-ttu-id="a13b9-139">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [сообщения](../resources/message.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a13b9-139">If successful, this method returns a `201 Created` response code and a [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a13b9-140">Пример</span><span class="sxs-lookup"><span data-stu-id="a13b9-140">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="a13b9-141">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="a13b9-141">Request 1</span></span>
<span data-ttu-id="a13b9-142">Ниже приведен пример запроса на создание черновика нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="a13b9-142">Here is an example of the request to create a draft of a new message.</span></span>
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
<span data-ttu-id="a13b9-143">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a13b9-143">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="a13b9-144">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="a13b9-144">Response 1</span></span>
<span data-ttu-id="a13b9-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a13b9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="a13b9-148">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="a13b9-148">Request 2</span></span>
<span data-ttu-id="a13b9-149">В следующем примере показаны по электронной почте черновиков с Randi Welch для Samantha стенда.</span><span class="sxs-lookup"><span data-stu-id="a13b9-149">The next example shows a draft email by Randi Welch to Samantha Booth.</span></span> <span data-ttu-id="a13b9-150">Сообщение также включает в себя упоминание другому пользователю, Swope Дану.</span><span class="sxs-lookup"><span data-stu-id="a13b9-150">The message also includes a mention of another user, Dana Swope.</span></span>

<span data-ttu-id="a13b9-151">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a13b9-151">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
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


##### <a name="response-2"></a><span data-ttu-id="a13b9-152">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="a13b9-152">Response 2</span></span>
<span data-ttu-id="a13b9-p107">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a13b9-p107">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-3"></a><span data-ttu-id="a13b9-156">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="a13b9-156">Request 3</span></span>
<span data-ttu-id="a13b9-157">Следующий пример добавляет несколько заголовков сообщений Интернета клиента при создании черновика сообщения.</span><span class="sxs-lookup"><span data-stu-id="a13b9-157">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>
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
<span data-ttu-id="a13b9-158">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a13b9-158">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-3"></a><span data-ttu-id="a13b9-159">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="a13b9-159">Response 3</span></span>
<span data-ttu-id="a13b9-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a13b9-160">Here is an example of the response.</span></span> <span data-ttu-id="a13b9-161">Примечание: Заголовки сообщений Интернета не возвращаются в ответа POST по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a13b9-161">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="a13b9-162">Объект ответа, показанный здесь также может усекаться для краткости.</span><span class="sxs-lookup"><span data-stu-id="a13b9-162">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="a13b9-163">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a13b9-163">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="a13b9-164">См. также</span><span class="sxs-lookup"><span data-stu-id="a13b9-164">See also</span></span>

- [<span data-ttu-id="a13b9-165">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="a13b9-165">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a13b9-166">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="a13b9-166">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="a13b9-167">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="a13b9-167">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
