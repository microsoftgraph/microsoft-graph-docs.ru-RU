---
title: Вывод сообщения
description: Получение свойств и связей объекта message.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ab57e15b88cef2ba1749c19a1b00d3521136f274
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865568"
---
# <a name="get-message"></a><span data-ttu-id="cae8b-103">Вывод сообщения</span><span class="sxs-lookup"><span data-stu-id="cae8b-103">Get message</span></span>

<span data-ttu-id="cae8b-104">Получение свойств и связей объекта [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="cae8b-104">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="cae8b-105">Вы можете использовать параметр `$value`, чтобы [получить MIME-содержимое сообщения](/graph/outlook-get-mime-message).</span><span class="sxs-lookup"><span data-stu-id="cae8b-105">You can use the `$value` parameter to [get the MIME content of a message](/graph/outlook-get-mime-message).</span></span>

<span data-ttu-id="cae8b-106">Существует два сценария, когда приложение может получить сообщение из папки почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="cae8b-106">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="cae8b-107">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="cae8b-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="cae8b-108">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="cae8b-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="cae8b-109">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="cae8b-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="cae8b-110">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="cae8b-110">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="cae8b-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cae8b-111">Permissions</span></span>
<span data-ttu-id="cae8b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cae8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cae8b-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cae8b-114">Permission type</span></span>      | <span data-ttu-id="cae8b-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cae8b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cae8b-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cae8b-116">Delegated (work or school account)</span></span> | <span data-ttu-id="cae8b-117">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cae8b-117">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="cae8b-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cae8b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cae8b-119">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cae8b-119">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="cae8b-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="cae8b-120">Application</span></span> | <span data-ttu-id="cae8b-121">Mail.ReadBasic.All, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cae8b-121">Mail.ReadBasic.All, Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="cae8b-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cae8b-122">HTTP request</span></span>

<span data-ttu-id="cae8b-123">Для получения указанного сообщения:</span><span class="sxs-lookup"><span data-stu-id="cae8b-123">To get the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="cae8b-124">Для получения MIME-содержимого указанного сообщения:</span><span class="sxs-lookup"><span data-stu-id="cae8b-124">To get the MIME content of the specified message:</span></span>
<!-- { "blockType": "ignored" } --> 
```http 
GET /me/messages/{id}/$value 
GET /users/{id | userPrincipalName}/messages/{id}/$value 
GET /me/mailFolders/{id}/messages/{id}/$value 
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/$value 
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cae8b-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cae8b-125">Optional query parameters</span></span>
<span data-ttu-id="cae8b-126">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cae8b-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="cae8b-127">Используйте параметр `$value`, чтобы получить MIME-содержимое сообщения.</span><span class="sxs-lookup"><span data-stu-id="cae8b-127">You can use the  parameter to get the MIME content of a message.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cae8b-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cae8b-128">Request headers</span></span>
| <span data-ttu-id="cae8b-129">Имя</span><span class="sxs-lookup"><span data-stu-id="cae8b-129">Name</span></span>       | <span data-ttu-id="cae8b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cae8b-130">Type</span></span> | <span data-ttu-id="cae8b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cae8b-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cae8b-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="cae8b-132">Authorization</span></span>  | <span data-ttu-id="cae8b-133">string</span><span class="sxs-lookup"><span data-stu-id="cae8b-133">string</span></span>  | <span data-ttu-id="cae8b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cae8b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cae8b-136">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="cae8b-136">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="cae8b-137">string</span><span class="sxs-lookup"><span data-stu-id="cae8b-137">string</span></span> | <span data-ttu-id="cae8b-138">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="cae8b-138">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="cae8b-139">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="cae8b-139">Values can be "text" or "html".</span></span> <span data-ttu-id="cae8b-140">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="cae8b-140">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="cae8b-141">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="cae8b-141">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="cae8b-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="cae8b-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cae8b-143">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cae8b-143">Request body</span></span>
<span data-ttu-id="cae8b-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cae8b-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cae8b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae8b-145">Response</span></span>

<span data-ttu-id="cae8b-146">В случае успеха этот метод возвращает код отклика `200 OK` и объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cae8b-146">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="cae8b-147">При указании параметра `$value` возвращается содержимое сообщения в формате MIME, а не ресурс **message**.</span><span class="sxs-lookup"><span data-stu-id="cae8b-147">Specifying the `$value` parameter returns the message content in MIME format, and not a **message** resource.</span></span>


## <a name="examples"></a><span data-ttu-id="cae8b-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="cae8b-148">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="cae8b-149">Пример 1</span><span class="sxs-lookup"><span data-stu-id="cae8b-149">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="cae8b-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="cae8b-150">Request</span></span>
<span data-ttu-id="cae8b-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cae8b-151">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cae8b-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="cae8b-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cae8b-153">C#</span><span class="sxs-lookup"><span data-stu-id="cae8b-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cae8b-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cae8b-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cae8b-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cae8b-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cae8b-156">Java</span><span class="sxs-lookup"><span data-stu-id="cae8b-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cae8b-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae8b-157">Response</span></span>
<span data-ttu-id="cae8b-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cae8b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2"></a><span data-ttu-id="cae8b-161">Пример 2</span><span class="sxs-lookup"><span data-stu-id="cae8b-161">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="cae8b-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="cae8b-162">Request</span></span>
<span data-ttu-id="cae8b-163">В следующем примере используется параметр запроса `$select` для получения заголовков сообщений Интернета для сообщения.</span><span class="sxs-lookup"><span data-stu-id="cae8b-163">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="cae8b-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="cae8b-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cae8b-165">C#</span><span class="sxs-lookup"><span data-stu-id="cae8b-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cae8b-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cae8b-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cae8b-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cae8b-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cae8b-168">Java</span><span class="sxs-lookup"><span data-stu-id="cae8b-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cae8b-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae8b-169">Response</span></span>
<span data-ttu-id="cae8b-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cae8b-170">Here is an example of the response.</span></span> <span data-ttu-id="cae8b-171">Примечание. Набор заголовков сообщений в объекте отклика усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="cae8b-171">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="cae8b-172">При фактическом вызове будут возвращены все заголовки.</span><span class="sxs-lookup"><span data-stu-id="cae8b-172">All of the headers will be returned from an actual call.</span></span>
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

### <a name="example-3"></a><span data-ttu-id="cae8b-173">Пример 3</span><span class="sxs-lookup"><span data-stu-id="cae8b-173">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="cae8b-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="cae8b-174">Request</span></span>

<span data-ttu-id="cae8b-175">В третьем примере показано, как использовать заголовок `Prefer: outlook.body-content-type="text"`, чтобы получить свойства **body** и **uniqueBody** указанного сообщения в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="cae8b-175">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cae8b-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="cae8b-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cae8b-177">C#</span><span class="sxs-lookup"><span data-stu-id="cae8b-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cae8b-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cae8b-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cae8b-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cae8b-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cae8b-180">Java</span><span class="sxs-lookup"><span data-stu-id="cae8b-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cae8b-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae8b-181">Response</span></span>

<span data-ttu-id="cae8b-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cae8b-182">Here is an example of the response.</span></span> <span data-ttu-id="cae8b-183">Примечание. Отклик включает заголовок `Preference-Applied: outlook.body-content-type`, подтверждающий заголовок запроса `Prefer: outlook.body-content-type`.</span><span class="sxs-lookup"><span data-stu-id="cae8b-183">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)/$entity",
    "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
    "id":"AAMkAGI1AAAoZCfHAAA=",
    "subject":"Welcome to our group!",
    "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nTh",
    "body":{
        "contentType":"text",
        "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nThanks!\r\n\r\n"
    },
    "uniqueBody":{
        "contentType":"text",
        "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\nThanks!\r\n"
    }
}
```

### <a name="example-4"></a><span data-ttu-id="cae8b-184">Пример 4</span><span class="sxs-lookup"><span data-stu-id="cae8b-184">Example 4</span></span>
#### <a name="request"></a><span data-ttu-id="cae8b-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="cae8b-185">Request</span></span>
<span data-ttu-id="cae8b-186">В четвертом примере показано, как получить MIME-содержимое сообщения в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="cae8b-186">The fourth example gets the MIME content of a message in the signed-in user's mailbox.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/4aade2547798441eab5188a7a2436bc1/$value
```

#### <a name="response"></a><span data-ttu-id="cae8b-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae8b-187">Response</span></span>
<span data-ttu-id="cae8b-188">Ниже приведен отклик.</span><span class="sxs-lookup"><span data-stu-id="cae8b-188">The following is the response.</span></span> <span data-ttu-id="cae8b-189">Содержимое MIME начинается с заголовка `MIME-Version`.</span><span class="sxs-lookup"><span data-stu-id="cae8b-189">The MIME content begins with the `MIME-Version` header.</span></span> 
<!-- {
  "blockType": "ignored"
} -->
```http
HTTP/1.1 200 OK

Received: from contoso.com (10.194.241.197) by 
contoso.com (10.194.241.197) with Microsoft 
SMTP Server (version=TLS1_2, 
cipher=TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384_P256) id 15.1.1374.0 via Mailbox 
Transport; Mon, 4 Sep 2017 03:00:08 -0700 
Received: from contoso.com (10.194.241.197) by 
contoso.com (10.194.241.197) with Microsoft 
SMTP Server (version=TLS1_2, 
cipher=TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384_P256) id 15.1.1374.0; Mon, 4 Sep 
2017 03:00:07 -0700 
Received: from contoso.com 
(fe80::5bf:5059:4ca0:5017) by contoso.com 
(fe80::5bf:5059:4ca0:5017%12) with mapi id 15.01.1374.000; Mon, 4 Sep 2017 
03:00:01 -0700 
From: Administrator <admin@contoso.com> 
To: Administrator <admin@contoso.com> 
Subject: This email has attachment. 
Thread-Topic: This email has attachment. 
Thread-Index: AQHTJWSHSywMzSz8o0OJud48nG50GQ== 
Date: Mon, 4 Sep 2017 10:00:00 +0000 
Message-ID: 
                <4aade2547798441eab5188a7a2436bc1@contoso.com> 
Accept-Language: en-US 
Content-Language: en-US 
X-MS-Exchange-Organization-AuthAs: Internal 
X-MS-Exchange-Organization-AuthMechanism: 04 
X-MS-Exchange-Organization-AuthSource: 
                contoso.com 
X-MS-Has-Attach: yes 
X-MS-Exchange-Organization-Network-Message-Id: 
                0ffdb402-ec03-42c8-5d32-08d4f37bb517 
X-MS-Exchange-Organization-SCL: -1 
X-MS-TNEF-Correlator: 
X-MS-Exchange-Organization-RecordReviewCfmType: 0 
x-ms-publictraffictype: Emai

```http
MIME-Version: 1.0 
Content-Type: multipart/mixed; 
                boundary="_004_4aade2547798441eab5188a7a2436bc1contoso_" 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: multipart/alternative; 
                boundary="_000_4aade2547798441eab5188a7a2436bc1contoso_" 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: text/plain; charset="iso-8859-1" 
Content-Transfer-Encoding: quoted-printable 
 
The attachment is an email. 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: text/html; charset="iso-8859-1" 
Content-Transfer-Encoding: quoted-printable 
 
<html> 
<head> 
<meta http-equiv=3D"Content-Type" content=3D"text/html; charset=3Diso-8859-= 
1"> 
<style type=3D"text/css" style=3D"display:none;"><!-- P {margin-top:0;margi= 
n-bottom:0;} --></style> 
</head> 
<body dir=3D"ltr"> 
<div id=3D"divtagdefaultwrapper" style=3D"font-size:12pt;color:#000000;font= 
-family:Calibri,Helvetica,sans-serif;" dir=3D"ltr"> 
<p>The attachment is an email.</p> 
</div> 
</body> 
</html> 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_-- 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: application/octet-stream; name="Attachment email.eml" 
Content-Description: Attachment email.eml 
Content-Disposition: attachment; filename="Attachment email.eml"; size=408; 
                creation-date="Mon, 04 Sep 2017 09:59:43 GMT"; 
                modification-date="Mon, 04 Sep 2017 09:59:43 GMT" 
Content-Transfer-Encoding: base64 
 
RnJvbToJQWRtaW5pc3RyYXRvciA8YWRtaW5AdGVuYW50LUVYSEItMTQ3MS5jb20+DQpTZW50OglN 
b25kYXksIFNlcHRlbWJlciA0LCAyMDE3IDM6MjYgUE0NClRvOglTcml2YXJkaGFuIEhlYmJhcg0K 
U3ViamVjdDoJQXR0YWNobWVudCBlbWFpbA0KDQpJIHdpbGwgYXR0YWNoIHRoaXMgZW1haWwgdG8g 
YW5vdGhlciBtYWlsLg0K 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_-- 
```


## <a name="see-also"></a><span data-ttu-id="cae8b-190">См. также</span><span class="sxs-lookup"><span data-stu-id="cae8b-190">See also</span></span>

- [<span data-ttu-id="cae8b-191">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="cae8b-191">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="cae8b-192">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="cae8b-192">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
