---
title: Создание объекта Message
description: С помощью этого API можно создать черновик нового сообщения. Черновики можно создавать в любой папке и при необходимости изменять перед отправкой. Для сохранения в папке "Черновики" используйте ярлык /messages.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 295397e4c85e2096d69e7ba14432cc866b4094a4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564045"
---
# <a name="create-message"></a><span data-ttu-id="ec910-105">Создание объекта Message</span><span class="sxs-lookup"><span data-stu-id="ec910-105">Create Message</span></span>

<span data-ttu-id="ec910-p102">С помощью этого API можно создать черновик нового сообщения. Черновики можно создавать в любой папке и при необходимости изменять перед отправкой. Для сохранения в папке "Черновики" используйте ярлык /messages.</span><span class="sxs-lookup"><span data-stu-id="ec910-p102">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="ec910-109">Создавая черновик, в тот же **POST**-запрос вы можете включить [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="ec910-109">While creating the draft in the same **POST** call, you can include an [attachment](../resources/attachment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ec910-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec910-110">Permissions</span></span>
<span data-ttu-id="ec910-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec910-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec910-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec910-113">Permission type</span></span>      | <span data-ttu-id="ec910-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec910-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec910-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec910-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ec910-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec910-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ec910-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec910-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec910-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec910-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ec910-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec910-119">Application</span></span> | <span data-ttu-id="ec910-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec910-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec910-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec910-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="ec910-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec910-122">Request headers</span></span>
| <span data-ttu-id="ec910-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ec910-123">Header</span></span>       | <span data-ttu-id="ec910-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ec910-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ec910-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec910-125">Authorization</span></span>  | <span data-ttu-id="ec910-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec910-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ec910-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ec910-128">Content-Type</span></span>  | <span data-ttu-id="ec910-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ec910-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ec910-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ec910-130">Request body</span></span>
<span data-ttu-id="ec910-131">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec910-131">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

<span data-ttu-id="ec910-132">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными в сообщение при его создании.</span><span class="sxs-lookup"><span data-stu-id="ec910-132">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="ec910-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec910-133">Response</span></span>

<span data-ttu-id="ec910-134">В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ec910-134">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec910-135">Пример</span><span class="sxs-lookup"><span data-stu-id="ec910-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="ec910-136">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="ec910-136">Request 1</span></span>
<span data-ttu-id="ec910-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec910-137">Here is an example of the request.</span></span>
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
<span data-ttu-id="ec910-138">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec910-138">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="ec910-139">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="ec910-139">Response 1</span></span>
<span data-ttu-id="ec910-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ec910-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="ec910-143">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="ec910-143">Request 2</span></span>
<span data-ttu-id="ec910-144">В следующем примере добавляется пара пользовательских заголовков сообщений Интернета при создании черновика сообщения.</span><span class="sxs-lookup"><span data-stu-id="ec910-144">The next example adds a couple of customer Internet message headers when creating the message draft.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_with_headers_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
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
<span data-ttu-id="ec910-145">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec910-145">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-2"></a><span data-ttu-id="ec910-146">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="ec910-146">Response 2</span></span>
<span data-ttu-id="ec910-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ec910-147">Here is an example of the response.</span></span> <span data-ttu-id="ec910-148">Примечание. Заголовки сообщений Интернета не возвращаются по умолчанию в ответе POST.</span><span class="sxs-lookup"><span data-stu-id="ec910-148">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="ec910-149">Примечание. Представленный здесь объект отклика также может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="ec910-149">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ec910-150">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec910-150">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
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

## <a name="see-also"></a><span data-ttu-id="ec910-151">См. также</span><span class="sxs-lookup"><span data-stu-id="ec910-151">See also</span></span>

- [<span data-ttu-id="ec910-152">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="ec910-152">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ec910-153">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="ec910-153">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
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
