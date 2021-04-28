---
title: Вывод сообщения
description: Получение свойств и связей объекта message.
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: faef3fd45e331012b642624361c9fc03e35d9a97
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035381"
---
# <a name="get-message"></a><span data-ttu-id="9623a-103">Вывод сообщения</span><span class="sxs-lookup"><span data-stu-id="9623a-103">Get message</span></span>

<span data-ttu-id="9623a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9623a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9623a-105">Получение свойств и связей объекта [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="9623a-105">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="9623a-106">Вы можете использовать параметр `$value`, чтобы [получить MIME-содержимое сообщения](/graph/outlook-get-mime-message).</span><span class="sxs-lookup"><span data-stu-id="9623a-106">You can use the `$value` parameter to [get the MIME content of a message](/graph/outlook-get-mime-message).</span></span> <span data-ttu-id="9623a-107">Также см. [пример](#example-4-get-mime-content) ниже.</span><span class="sxs-lookup"><span data-stu-id="9623a-107">See also an [example](#example-4-get-mime-content) below.</span></span>

<span data-ttu-id="9623a-108">Существует два сценария, когда приложение может получить сообщение из папки почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="9623a-108">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="9623a-109">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="9623a-109">If the app has application permissions, or,</span></span>
* <span data-ttu-id="9623a-110">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="9623a-110">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="9623a-111">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="9623a-111">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="9623a-112">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="9623a-112">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="9623a-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9623a-113">Permissions</span></span>
<span data-ttu-id="9623a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9623a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9623a-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9623a-116">Permission type</span></span>      | <span data-ttu-id="9623a-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9623a-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9623a-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9623a-118">Delegated (work or school account)</span></span> | <span data-ttu-id="9623a-119">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9623a-119">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="9623a-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9623a-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9623a-121">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9623a-121">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="9623a-122">Для приложения</span><span class="sxs-lookup"><span data-stu-id="9623a-122">Application</span></span> | <span data-ttu-id="9623a-123">Mail.ReadBasic.All, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9623a-123">Mail.ReadBasic.All, Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="9623a-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9623a-124">HTTP request</span></span>

<span data-ttu-id="9623a-125">Для получения указанного сообщения:</span><span class="sxs-lookup"><span data-stu-id="9623a-125">To get the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="9623a-126">Для получения MIME-содержимого указанного сообщения:</span><span class="sxs-lookup"><span data-stu-id="9623a-126">To get the MIME content of the specified message:</span></span>
<!-- { "blockType": "ignored" } --> 
```http 
GET /me/messages/{id}/$value 
GET /users/{id | userPrincipalName}/messages/{id}/$value 
GET /me/mailFolders/{id}/messages/{id}/$value 
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/$value 
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9623a-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9623a-127">Optional query parameters</span></span>
<span data-ttu-id="9623a-128">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9623a-128">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="9623a-129">Используйте параметр `$value`, чтобы получить MIME-содержимое сообщения.</span><span class="sxs-lookup"><span data-stu-id="9623a-129">Use the `$value` parameter to get the MIME content of a message.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9623a-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9623a-130">Request headers</span></span>
| <span data-ttu-id="9623a-131">Имя</span><span class="sxs-lookup"><span data-stu-id="9623a-131">Name</span></span>       | <span data-ttu-id="9623a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="9623a-132">Type</span></span> | <span data-ttu-id="9623a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="9623a-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9623a-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="9623a-134">Authorization</span></span>  | <span data-ttu-id="9623a-135">string</span><span class="sxs-lookup"><span data-stu-id="9623a-135">string</span></span>  | <span data-ttu-id="9623a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9623a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9623a-138">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="9623a-138">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="9623a-139">string</span><span class="sxs-lookup"><span data-stu-id="9623a-139">string</span></span> | <span data-ttu-id="9623a-140">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="9623a-140">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="9623a-141">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="9623a-141">Values can be "text" or "html".</span></span> <span data-ttu-id="9623a-142">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="9623a-142">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="9623a-143">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="9623a-143">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="9623a-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9623a-144">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9623a-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9623a-145">Request body</span></span>
<span data-ttu-id="9623a-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9623a-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9623a-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="9623a-147">Response</span></span>

<span data-ttu-id="9623a-148">В случае успеха этот метод возвращает код отклика `200 OK` и объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9623a-148">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="9623a-149">При указании параметра `$value` возвращается содержимое сообщения в формате MIME, а не ресурс **message**.</span><span class="sxs-lookup"><span data-stu-id="9623a-149">Specifying the `$value` parameter returns the message content in MIME format, and not a **message** resource.</span></span>


## <a name="examples"></a><span data-ttu-id="9623a-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="9623a-150">Examples</span></span>
### <a name="example-1-get-a-specific-message"></a><span data-ttu-id="9623a-151">Пример 1. Получение определенного сообщения</span><span class="sxs-lookup"><span data-stu-id="9623a-151">Example 1: Get a specific message</span></span>
#### <a name="request"></a><span data-ttu-id="9623a-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="9623a-152">Request</span></span>
<span data-ttu-id="9623a-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9623a-153">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9623a-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="9623a-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
# <a name="c"></a>[<span data-ttu-id="9623a-155">C#</span><span class="sxs-lookup"><span data-stu-id="9623a-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9623a-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9623a-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9623a-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9623a-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9623a-158">Java</span><span class="sxs-lookup"><span data-stu-id="9623a-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9623a-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="9623a-159">Response</span></span>
<span data-ttu-id="9623a-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9623a-160">Here is an example of the response.</span></span> <span data-ttu-id="9623a-161">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9623a-161">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_message",
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

### <a name="example-2-get-internet-message-headers"></a><span data-ttu-id="9623a-162">Пример 2. Получение заголовков сообщений Интернета</span><span class="sxs-lookup"><span data-stu-id="9623a-162">Example 2: Get Internet message headers</span></span>
#### <a name="request"></a><span data-ttu-id="9623a-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="9623a-163">Request</span></span>
<span data-ttu-id="9623a-164">В следующем примере используется параметр запроса `$select` для получения заголовков сообщений Интернета для сообщения.</span><span class="sxs-lookup"><span data-stu-id="9623a-164">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 

# <a name="http"></a>[<span data-ttu-id="9623a-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="9623a-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
# <a name="c"></a>[<span data-ttu-id="9623a-166">C#</span><span class="sxs-lookup"><span data-stu-id="9623a-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9623a-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9623a-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9623a-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9623a-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9623a-169">Java</span><span class="sxs-lookup"><span data-stu-id="9623a-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9623a-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="9623a-170">Response</span></span>
<span data-ttu-id="9623a-p107">Ниже приведен пример отклика. Примечание. Набор заголовков сообщений в объекте отклика усечен для краткости. При фактическом вызове будут возвращены все заголовки.</span><span class="sxs-lookup"><span data-stu-id="9623a-p107">Here is an example of the response. Note: The set of message headers in the response object is truncated for brevity. All of the headers will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_message_headers",
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

### <a name="example-3-get-message-body-in-text-format"></a><span data-ttu-id="9623a-174">Пример 3. Получение текста сообщения в текстовом формате</span><span class="sxs-lookup"><span data-stu-id="9623a-174">Example 3: Get message body in text format</span></span>
#### <a name="request"></a><span data-ttu-id="9623a-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="9623a-175">Request</span></span>

<span data-ttu-id="9623a-176">В третьем примере показано, как использовать заголовок `Prefer: outlook.body-content-type="text"`, чтобы получить свойства **body** и **uniqueBody** указанного сообщения в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="9623a-176">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>


# <a name="http"></a>[<span data-ttu-id="9623a-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="9623a-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="9623a-178">C#</span><span class="sxs-lookup"><span data-stu-id="9623a-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9623a-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9623a-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9623a-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9623a-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9623a-181">Java</span><span class="sxs-lookup"><span data-stu-id="9623a-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9623a-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="9623a-182">Response</span></span>

<span data-ttu-id="9623a-183">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9623a-183">Here is an example of the response.</span></span> <span data-ttu-id="9623a-184">Примечание. Отклик включает заголовок `Preference-Applied: outlook.body-content-type`, подтверждающий заголовок запроса `Prefer: outlook.body-content-type`.</span><span class="sxs-lookup"><span data-stu-id="9623a-184">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_message_in_text",
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

### <a name="example-4-get-mime-content"></a><span data-ttu-id="9623a-185">Пример 4. Получение содержимого MIME</span><span class="sxs-lookup"><span data-stu-id="9623a-185">Example 4: Get MIME content</span></span>
#### <a name="request"></a><span data-ttu-id="9623a-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="9623a-186">Request</span></span>
<span data-ttu-id="9623a-187">В четвертом примере показано, как получить MIME-содержимое сообщения в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="9623a-187">The fourth example gets the MIME content of a message in the signed-in user's mailbox.</span></span>


# <a name="http"></a>[<span data-ttu-id="9623a-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="9623a-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_message_in_mime",
  "sampleKeys": ["4aade2547798441eab5188a7a2436bc1"]
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/4aade2547798441eab5188a7a2436bc1/$value
```
# <a name="c"></a>[<span data-ttu-id="9623a-189">C#</span><span class="sxs-lookup"><span data-stu-id="9623a-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-mime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9623a-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9623a-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-mime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9623a-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9623a-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-mime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9623a-192">Java</span><span class="sxs-lookup"><span data-stu-id="9623a-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-mime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9623a-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="9623a-193">Response</span></span>
<span data-ttu-id="9623a-194">Ниже приведен отклик.</span><span class="sxs-lookup"><span data-stu-id="9623a-194">The following is the response.</span></span> <span data-ttu-id="9623a-195">Содержимое MIME начинается с заголовка `MIME-Version`.</span><span class="sxs-lookup"><span data-stu-id="9623a-195">The MIME content begins with the `MIME-Version` header.</span></span> 

<!-- {
  "blockType": "response",
  "name": "get_message_in_mime",
  "truncated": true,
  "@odata.type": "string"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

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


## <a name="see-also"></a><span data-ttu-id="9623a-196">См. также</span><span class="sxs-lookup"><span data-stu-id="9623a-196">See also</span></span>

- [<span data-ttu-id="9623a-197">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="9623a-197">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9623a-198">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="9623a-198">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
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
