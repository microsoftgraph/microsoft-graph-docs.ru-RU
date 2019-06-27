---
title: Создание объекта Message
description: С помощью этого API можно создать черновик нового сообщения. Черновики можно создавать в любой папке и при необходимости изменять перед отправкой. Для сохранения в папке "Черновики" используйте ярлык /messages.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1f3157977ee66aab36eef55dec50c7ea387936ce
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269974"
---
# <a name="create-message"></a><span data-ttu-id="2f5b2-105">Создание объекта Message</span><span class="sxs-lookup"><span data-stu-id="2f5b2-105">Create Message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f5b2-p102">С помощью этого API можно создать черновик нового сообщения. Черновики можно создавать в любой папке и при необходимости изменять перед отправкой. Для сохранения в папке "Черновики" используйте ярлык /messages.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-p102">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="2f5b2-109">При создании черновика в одном вызове **POST** можно выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="2f5b2-109">While creating the draft in the same **POST** call, you can:</span></span>

- <span data-ttu-id="2f5b2-110">Включение [вложения](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="2f5b2-110">Include an [attachment](../resources/attachment.md)</span></span> 
- <span data-ttu-id="2f5b2-111">Используйте [упоминание](../resources/mention.md) , чтобы вызвонить другому пользователю в новом сообщении.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-111">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="2f5b2-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f5b2-112">Permissions</span></span>
<span data-ttu-id="2f5b2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f5b2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f5b2-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f5b2-115">Permission type</span></span>      | <span data-ttu-id="2f5b2-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f5b2-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f5b2-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f5b2-117">Delegated (work or school account)</span></span> | <span data-ttu-id="2f5b2-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f5b2-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2f5b2-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f5b2-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f5b2-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f5b2-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2f5b2-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f5b2-121">Application</span></span> | <span data-ttu-id="2f5b2-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f5b2-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f5b2-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f5b2-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="2f5b2-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f5b2-124">Request headers</span></span>
| <span data-ttu-id="2f5b2-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f5b2-125">Header</span></span>       | <span data-ttu-id="2f5b2-126">Значение</span><span class="sxs-lookup"><span data-stu-id="2f5b2-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2f5b2-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f5b2-127">Authorization</span></span>  | <span data-ttu-id="2f5b2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2f5b2-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f5b2-130">Content-Type</span></span>  | <span data-ttu-id="2f5b2-131">application/json</span><span class="sxs-lookup"><span data-stu-id="2f5b2-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f5b2-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2f5b2-132">Request body</span></span>
<span data-ttu-id="2f5b2-133">В тексте запроса добавьте представление объекта [Message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-133">In the request body, supply a JSON representation of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="2f5b2-134">Если вы хотите использовать **упоминание** , чтобы вызвонить другому пользователю в новом сообщении:</span><span class="sxs-lookup"><span data-stu-id="2f5b2-134">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="2f5b2-135">Включите в текст запроса обязательное свойство **toRecipients** , свойства **упоминаютх** и все доступные для записи свойства сообщения.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-135">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="2f5b2-136">Для каждого упоминания в свойстве **упоминания** необходимо указать указанное свойство. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="2f5b2-136">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="2f5b2-137">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными в сообщение при его создании.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-137">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="2f5b2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f5b2-138">Response</span></span>

<span data-ttu-id="2f5b2-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-139">If successful, this method returns a `201 Created` response code and a [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f5b2-140">Пример</span><span class="sxs-lookup"><span data-stu-id="2f5b2-140">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="2f5b2-141">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="2f5b2-141">Request 1</span></span>
<span data-ttu-id="2f5b2-142">Ниже приведен пример запроса на создание черновика нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-142">Here is an example of the request to create a draft of a new message.</span></span>
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
<span data-ttu-id="2f5b2-143">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-143">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="2f5b2-144">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="2f5b2-144">Response 1</span></span>
<span data-ttu-id="2f5b2-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2f5b2-148">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="2f5b2-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2f5b2-149">C#</span><span class="sxs-lookup"><span data-stu-id="2f5b2-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_message_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2f5b2-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="2f5b2-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_message_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2f5b2-151">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2f5b2-151">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_message_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="2f5b2-152">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="2f5b2-152">Request 2</span></span>
<span data-ttu-id="2f5b2-153">В следующем примере показан черновик электронного письма с помощью Ранди Велч на стенд Samantha.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-153">The next example shows a draft email by Randi Welch to Samantha Booth.</span></span> <span data-ttu-id="2f5b2-154">Сообщение также содержит упоминание другого пользователя, дана свопе.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-154">The message also includes a mention of another user, Dana Swope.</span></span>

<span data-ttu-id="2f5b2-155">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-155">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
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


##### <a name="response-2"></a><span data-ttu-id="2f5b2-156">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="2f5b2-156">Response 2</span></span>
<span data-ttu-id="2f5b2-p107">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-p107">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2f5b2-160">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="2f5b2-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2f5b2-161">C#</span><span class="sxs-lookup"><span data-stu-id="2f5b2-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_message_with_mentions_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2f5b2-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="2f5b2-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_message_with_mentions_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2f5b2-163">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2f5b2-163">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_message_with_mentions_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-3"></a><span data-ttu-id="2f5b2-164">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="2f5b2-164">Request 3</span></span>
<span data-ttu-id="2f5b2-165">В следующем примере добавляется пара пользовательских заголовков сообщений Интернета при создании черновика сообщения.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-165">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>
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
<span data-ttu-id="2f5b2-166">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-166">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-3"></a><span data-ttu-id="2f5b2-167">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="2f5b2-167">Response 3</span></span>
<span data-ttu-id="2f5b2-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-168">Here is an example of the response.</span></span> <span data-ttu-id="2f5b2-169">Примечание. Заголовки сообщений Интернета не возвращаются по умолчанию в ответе POST.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-169">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="2f5b2-170">Примечание. Представленный здесь объект отклика также может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-170">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="2f5b2-171">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f5b2-171">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2f5b2-172">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="2f5b2-172">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2f5b2-173">C#</span><span class="sxs-lookup"><span data-stu-id="2f5b2-173">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_message_with_headers_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2f5b2-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="2f5b2-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_message_with_headers_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2f5b2-175">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2f5b2-175">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_message_with_headers_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="2f5b2-176">См. также</span><span class="sxs-lookup"><span data-stu-id="2f5b2-176">See also</span></span>

- [<span data-ttu-id="2f5b2-177">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="2f5b2-177">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2f5b2-178">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2f5b2-178">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="2f5b2-179">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2f5b2-179">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
