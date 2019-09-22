---
title: Вывод сообщения
description: Получение свойств и связей объекта message.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fbaf9d07e031369c004ce795b060a303fc8d2575
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041966"
---
# <a name="get-message"></a><span data-ttu-id="6a021-103">Вывод сообщения</span><span class="sxs-lookup"><span data-stu-id="6a021-103">Get message</span></span>

<span data-ttu-id="6a021-104">Получение свойств и связей объекта [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="6a021-104">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="6a021-105">Вы можете использовать параметр `$value`, чтобы [получить MIME-содержимое сообщения](/graph/outlook-get-mime-message).</span><span class="sxs-lookup"><span data-stu-id="6a021-105">You can now use a  segment to get the MIME content of an Outlook message.</span></span>

<span data-ttu-id="6a021-106">Существует два сценария, когда приложение может получить сообщение из папки почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="6a021-106">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="6a021-107">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="6a021-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="6a021-108">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="6a021-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="6a021-109">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="6a021-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="6a021-110">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="6a021-110">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="6a021-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a021-111">Permissions</span></span>
<span data-ttu-id="6a021-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a021-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a021-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a021-114">Permission type</span></span>      | <span data-ttu-id="6a021-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a021-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a021-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a021-116">Delegated (work or school account)</span></span> | <span data-ttu-id="6a021-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6a021-117">Mail.Read</span></span>    |
|<span data-ttu-id="6a021-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a021-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a021-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6a021-119">Mail.Read</span></span>    |
|<span data-ttu-id="6a021-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a021-120">Application</span></span> | <span data-ttu-id="6a021-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6a021-121">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a021-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a021-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6a021-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6a021-123">Optional query parameters</span></span>
<span data-ttu-id="6a021-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6a021-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6a021-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a021-125">Request headers</span></span>
| <span data-ttu-id="6a021-126">Имя</span><span class="sxs-lookup"><span data-stu-id="6a021-126">Name</span></span>       | <span data-ttu-id="6a021-127">Тип</span><span class="sxs-lookup"><span data-stu-id="6a021-127">Type</span></span> | <span data-ttu-id="6a021-128">Описание</span><span class="sxs-lookup"><span data-stu-id="6a021-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6a021-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a021-129">Authorization</span></span>  | <span data-ttu-id="6a021-130">string</span><span class="sxs-lookup"><span data-stu-id="6a021-130">string</span></span>  | <span data-ttu-id="6a021-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a021-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6a021-133">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="6a021-133">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="6a021-134">string</span><span class="sxs-lookup"><span data-stu-id="6a021-134">string</span></span> | <span data-ttu-id="6a021-135">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="6a021-135">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="6a021-136">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="6a021-136">Values can be "text" or "html".</span></span> <span data-ttu-id="6a021-137">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="6a021-137">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="6a021-138">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="6a021-138">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="6a021-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="6a021-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a021-140">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6a021-140">Request body</span></span>
<span data-ttu-id="6a021-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6a021-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a021-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a021-142">Response</span></span>

<span data-ttu-id="6a021-143">В случае успеха этот метод возвращает код отклика `200 OK` и объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a021-143">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="6a021-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="6a021-144">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="6a021-145">Пример 1</span><span class="sxs-lookup"><span data-stu-id="6a021-145">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="6a021-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a021-146">Request</span></span>
<span data-ttu-id="6a021-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a021-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6a021-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a021-148">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6a021-149">C#</span><span class="sxs-lookup"><span data-stu-id="6a021-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a021-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a021-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6a021-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a021-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6a021-152">Java</span><span class="sxs-lookup"><span data-stu-id="6a021-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6a021-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a021-153">Response</span></span>
<span data-ttu-id="6a021-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a021-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2"></a><span data-ttu-id="6a021-157">Пример 2</span><span class="sxs-lookup"><span data-stu-id="6a021-157">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="6a021-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a021-158">Request</span></span>
<span data-ttu-id="6a021-159">В следующем примере используется параметр запроса `$select` для получения заголовков сообщений Интернета для сообщения.</span><span class="sxs-lookup"><span data-stu-id="6a021-159">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="6a021-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a021-160">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6a021-161">C#</span><span class="sxs-lookup"><span data-stu-id="6a021-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a021-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a021-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6a021-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a021-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6a021-164">Java</span><span class="sxs-lookup"><span data-stu-id="6a021-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6a021-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a021-165">Response</span></span>
<span data-ttu-id="6a021-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6a021-166">Here is an example of the response.</span></span> <span data-ttu-id="6a021-167">Примечание. Набор заголовков сообщений в объекте отклика усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="6a021-167">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="6a021-168">При фактическом вызове будут возвращены все заголовки.</span><span class="sxs-lookup"><span data-stu-id="6a021-168">All of the headers will be returned from an actual call.</span></span>
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

### <a name="example-3"></a><span data-ttu-id="6a021-169">Пример 3</span><span class="sxs-lookup"><span data-stu-id="6a021-169">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="6a021-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a021-170">Request</span></span>

<span data-ttu-id="6a021-171">В третьем примере показано, как использовать заголовок `Prefer: outlook.body-content-type="text"`, чтобы получить свойства **body** и **uniqueBody** указанного сообщения в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="6a021-171">The second example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified message in text format.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6a021-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a021-172">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6a021-173">C#</span><span class="sxs-lookup"><span data-stu-id="6a021-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a021-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a021-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6a021-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a021-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6a021-176">Java</span><span class="sxs-lookup"><span data-stu-id="6a021-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6a021-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a021-177">Response</span></span>

<span data-ttu-id="6a021-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6a021-178">Here is an example of the response.</span></span> <span data-ttu-id="6a021-179">Примечание. Отклик включает заголовок `Preference-Applied: outlook.body-content-type`, подтверждающий заголовок запроса `Prefer: outlook.body-content-type`.</span><span class="sxs-lookup"><span data-stu-id="6a021-179">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="6a021-180">См. также</span><span class="sxs-lookup"><span data-stu-id="6a021-180">See also</span></span>

- [<span data-ttu-id="6a021-181">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="6a021-181">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6a021-182">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="6a021-182">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
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
