---
title: Вывод сообщения
description: Получение свойств и связей объекта message.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 905eaad15afcf25734886e1786991c65b737cc51
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612611"
---
# <a name="get-message"></a><span data-ttu-id="946f1-103">Вывод сообщения</span><span class="sxs-lookup"><span data-stu-id="946f1-103">Get message</span></span>

<span data-ttu-id="946f1-104">Получение свойств и связей объекта [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="946f1-104">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="946f1-105">В настоящее время эта операция возвращает текст сообщения только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="946f1-105">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="946f1-106">Существует два сценария, когда приложение может получить сообщение из папки почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="946f1-106">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="946f1-107">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="946f1-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="946f1-108">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="946f1-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="946f1-109">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="946f1-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="946f1-110">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="946f1-110">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="946f1-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="946f1-111">Permissions</span></span>
<span data-ttu-id="946f1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="946f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="946f1-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="946f1-114">Permission type</span></span>      | <span data-ttu-id="946f1-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="946f1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="946f1-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="946f1-116">Delegated (work or school account)</span></span> | <span data-ttu-id="946f1-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="946f1-117">Mail.Read</span></span>    |
|<span data-ttu-id="946f1-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="946f1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="946f1-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="946f1-119">Mail.Read</span></span>    |
|<span data-ttu-id="946f1-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="946f1-120">Application</span></span> | <span data-ttu-id="946f1-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="946f1-121">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="946f1-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="946f1-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="946f1-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="946f1-123">Optional query parameters</span></span>
<span data-ttu-id="946f1-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="946f1-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="946f1-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="946f1-125">Request headers</span></span>
| <span data-ttu-id="946f1-126">Имя</span><span class="sxs-lookup"><span data-stu-id="946f1-126">Name</span></span>       | <span data-ttu-id="946f1-127">Тип</span><span class="sxs-lookup"><span data-stu-id="946f1-127">Type</span></span> | <span data-ttu-id="946f1-128">Описание</span><span class="sxs-lookup"><span data-stu-id="946f1-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="946f1-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="946f1-129">Authorization</span></span>  | <span data-ttu-id="946f1-130">string</span><span class="sxs-lookup"><span data-stu-id="946f1-130">string</span></span>  | <span data-ttu-id="946f1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="946f1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="946f1-133">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="946f1-133">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="946f1-134">string</span><span class="sxs-lookup"><span data-stu-id="946f1-134">string</span></span> | <span data-ttu-id="946f1-135">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="946f1-135">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="946f1-136">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="946f1-136">Values can be "text" or "html".</span></span> <span data-ttu-id="946f1-137">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="946f1-137">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="946f1-138">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="946f1-138">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="946f1-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="946f1-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="946f1-140">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="946f1-140">Request body</span></span>
<span data-ttu-id="946f1-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="946f1-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="946f1-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="946f1-142">Response</span></span>

<span data-ttu-id="946f1-143">В случае успеха этот метод возвращает код отклика `200 OK` и объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="946f1-143">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="946f1-144">Пример</span><span class="sxs-lookup"><span data-stu-id="946f1-144">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="946f1-145">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="946f1-145">Request 1</span></span>
<span data-ttu-id="946f1-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="946f1-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
##### <a name="response-1"></a><span data-ttu-id="946f1-147">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="946f1-147">Response 1</span></span>
<span data-ttu-id="946f1-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="946f1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="946f1-151">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="946f1-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="946f1-152">C#</span><span class="sxs-lookup"><span data-stu-id="946f1-152">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="946f1-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="946f1-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_message-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="946f1-154">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="946f1-154">Request 2</span></span>
<span data-ttu-id="946f1-155">В следующем примере используется параметр запроса `$select` для получения заголовков сообщений Интернета для сообщения.</span><span class="sxs-lookup"><span data-stu-id="946f1-155">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
##### <a name="response-2"></a><span data-ttu-id="946f1-156">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="946f1-156">Response 2</span></span>
<span data-ttu-id="946f1-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="946f1-157">Here is an example of the response.</span></span> <span data-ttu-id="946f1-158">Примечание. Набор заголовков сообщений в объекте отклика усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="946f1-158">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="946f1-159">При фактическом вызове будут возвращены все заголовки.</span><span class="sxs-lookup"><span data-stu-id="946f1-159">All of the headers will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="946f1-160">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="946f1-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="946f1-161">C#</span><span class="sxs-lookup"><span data-stu-id="946f1-161">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_message_headers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="946f1-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="946f1-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_message_headers-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="see-also"></a><span data-ttu-id="946f1-163">Дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="946f1-163">See also</span></span>

- [<span data-ttu-id="946f1-164">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="946f1-164">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="946f1-165">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="946f1-165">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
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
    "Error: /api-reference/v1.0/api/message-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/message-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
