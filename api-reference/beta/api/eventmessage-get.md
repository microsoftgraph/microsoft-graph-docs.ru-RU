---
title: Получение объекта eventMessage
description: развернуть "параметр для **события**
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9463bd7b9198dc31311a8e4bacd07c5b10fbc965
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965768"
---
# <a name="get-eventmessage"></a><span data-ttu-id="2c69a-103">Получение объекта eventMessage</span><span class="sxs-lookup"><span data-stu-id="2c69a-103">Get eventMessage</span></span>

<span data-ttu-id="2c69a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c69a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c69a-105">Получение свойств и связей объекта [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="2c69a-105">Get the properties and relationships of the [eventMessage](../resources/eventmessage.md) object.</span></span> <span data-ttu-id="2c69a-106">Примените `$expand` параметр в свойстве навигации **события** , чтобы получить связанное [событие](../resources/event.md) в календаре участника.</span><span class="sxs-lookup"><span data-stu-id="2c69a-106">Apply the `$expand` parameter on the **event** navigation property to get the associated [event](../resources/event.md) in an attendee's calendar.</span></span>

### <a name="get-the-event-message-body-in-html-or-text-format"></a><span data-ttu-id="2c69a-107">Получение текста сообщения о событии в формате HTML или текстовом формате</span><span class="sxs-lookup"><span data-stu-id="2c69a-107">Get the event message body in HTML or text format</span></span>

<span data-ttu-id="2c69a-108">Тексты сообщений о событиях могут быть в формате HTML или текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="2c69a-108">Event message bodies can be in HTML or text format.</span></span>

<span data-ttu-id="2c69a-109">Вы можете использовать `Prefer: outlook.body-content-type` заголовок, чтобы указать нужный формат, возвращаемый в свойствах **Body** и **uniqueBody** в `GET` запросе:</span><span class="sxs-lookup"><span data-stu-id="2c69a-109">You can use the `Prefer: outlook.body-content-type` header to specify the desired format returned in the **body** and **uniqueBody** properties in a `GET` request:</span></span>

- <span data-ttu-id="2c69a-110">Укажите `Prefer: outlook.body-content-type="text"` , чтобы получить текст сообщения о событии, возвращенный в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="2c69a-110">Specify `Prefer: outlook.body-content-type="text"` to get a event message body returned in text format.</span></span>
- <span data-ttu-id="2c69a-111">Укажите `Prefer: outlook.body-content-type="html"` или просто пропустите заголовок, чтобы вернуть текст сообщения события в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="2c69a-111">Specify `Prefer: outlook.body-content-type="html"`, or just skip the header, to return the event message body in HTML format.</span></span>

<span data-ttu-id="2c69a-112">Если указан любой из этих заголовков, в ответ будет включен соответствующий `Preference-Applied` заголовок в качестве подтверждения:</span><span class="sxs-lookup"><span data-stu-id="2c69a-112">If you specify either header, the response will include the corresponding `Preference-Applied` header as confirmation:</span></span>

- <span data-ttu-id="2c69a-113">Чтобы получить результат выполнения запроса в текстовом формате: `Preference-Applied: outlook.body-content-type="text"`</span><span class="sxs-lookup"><span data-stu-id="2c69a-113">For text format requests: `Preference-Applied: outlook.body-content-type="text"`</span></span>
- <span data-ttu-id="2c69a-114">Чтобы получить результат выполнения запроса в формате HTML: `Preference-Applied: outlook.body-content-type="html"`</span><span class="sxs-lookup"><span data-stu-id="2c69a-114">For HTML format requests: `Preference-Applied: outlook.body-content-type="html"`</span></span>

## <a name="permissions"></a><span data-ttu-id="2c69a-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c69a-115">Permissions</span></span>
<span data-ttu-id="2c69a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c69a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c69a-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c69a-118">Permission type</span></span>      | <span data-ttu-id="2c69a-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c69a-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c69a-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c69a-120">Delegated (work or school account)</span></span> | <span data-ttu-id="2c69a-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2c69a-121">Mail.Read</span></span>    |
|<span data-ttu-id="2c69a-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c69a-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c69a-123">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2c69a-123">Mail.Read</span></span>    |
|<span data-ttu-id="2c69a-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c69a-124">Application</span></span> | <span data-ttu-id="2c69a-125">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2c69a-125">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c69a-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c69a-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2c69a-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2c69a-127">Optional query parameters</span></span>
<span data-ttu-id="2c69a-128">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2c69a-128">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2c69a-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c69a-129">Request headers</span></span>
| <span data-ttu-id="2c69a-130">Имя</span><span class="sxs-lookup"><span data-stu-id="2c69a-130">Name</span></span>       | <span data-ttu-id="2c69a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2c69a-131">Type</span></span> | <span data-ttu-id="2c69a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2c69a-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2c69a-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c69a-133">Authorization</span></span>  | <span data-ttu-id="2c69a-134">string</span><span class="sxs-lookup"><span data-stu-id="2c69a-134">string</span></span>  | <span data-ttu-id="2c69a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c69a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c69a-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2c69a-137">Request body</span></span>
<span data-ttu-id="2c69a-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2c69a-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c69a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c69a-139">Response</span></span>

<span data-ttu-id="2c69a-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [eventMessage](../resources/eventmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2c69a-140">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="2c69a-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="2c69a-141">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="2c69a-142">Пример 1</span><span class="sxs-lookup"><span data-stu-id="2c69a-142">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="2c69a-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c69a-143">Request</span></span>
<span data-ttu-id="2c69a-144">Первый пример показывает, как получить свойства сообщения о событии с учетом идентификатора этого сообщения.</span><span class="sxs-lookup"><span data-stu-id="2c69a-144">The first example shows how to get the properties of an event message based on the event message ID.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c69a-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c69a-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_eventmessage"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkADYAAAImV_lAAA=
```
# <a name="c"></a>[<span data-ttu-id="2c69a-146">C#</span><span class="sxs-lookup"><span data-stu-id="2c69a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c69a-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c69a-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c69a-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c69a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c69a-149">Java</span><span class="sxs-lookup"><span data-stu-id="2c69a-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="2c69a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c69a-150">Response</span></span>
<span data-ttu-id="2c69a-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c69a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_eventmessage",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessageRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages/$entity",
    "@odata.type":"#microsoft.graph.eventMessageRequest",
    "@odata.etag":"W/\"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVD\"",
    "id":"AAMkADYAAAImV_lAAA=",
    "createdDateTime":"2017-12-27T21:58:36Z",
    "lastModifiedDateTime":"2017-12-27T23:26:38Z",
    "changeKey":"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVD",
    "categories":[

    ],
    "receivedDateTime":"2017-12-27T21:58:36Z",
    "sentDateTime":"2017-12-27T21:58:36Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR1301MB2110DCFC@MWHPR1301MB2110.namprd13.prod.outlook.com>",
    "subject":"Debrief from meetup",
    "bodyPreview":"Let's debrief after community meetup.",
    "importance":"normal",
    "parentFolderId":"AQMkADYAAAIBDAAAAA==",
    "conversationId":"AAQkADYCipTiRjXQORU=",
    "conversationIndex":"AdN/Xdgnql4N9FlrT0KKlOJGNdA5FQ==",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADYAAAImV%2BlAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "meetingMessageType":"meetingRequest",
    "type":"singleInstance",
    "isOutOfDate":false,
    "isAllDay":false,
    "isDelegated":false,
    "responseRequested":true,
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n<style type=\"text/css\" style=\"display:none\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" dir=\"ltr\" style=\"font-size:12pt; color:#000000; font-family:Calibri,Helvetica,sans-serif\">\r\n<p style=\"margin-top:0; margin-bottom:0\">Let's debrief after community meetup.<br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "sender":{
        "emailAddress":{
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "mentionsPreview":null,
    "flag":{
        "flagStatus":"notFlagged"
    },
    "startDateTime":{
        "dateTime":"2018-02-19T19:00:00.0000000",
        "timeZone":"UTC"
    },
    "endDateTime":{
        "dateTime":"2018-02-19T19:30:00.0000000",
        "timeZone":"UTC"
    },
    "location":{
        "displayName":"Mt. Hood",
        "locationType":"default",
        "uniqueIdType":"unknown"
    },
    "recurrence":null,
    "previousLocation":null,
    "previousStartDateTime":null,
    "previousEndDateTime":null
}
```

### <a name="example-2"></a><span data-ttu-id="2c69a-154">Пример 2</span><span class="sxs-lookup"><span data-stu-id="2c69a-154">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="2c69a-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c69a-155">Request</span></span>
<span data-ttu-id="2c69a-156">Второй пример показывает, как получить событие, связанное с сообщением о событии.</span><span class="sxs-lookup"><span data-stu-id="2c69a-156">The second example shows how to get the event associated with an event message.</span></span> <span data-ttu-id="2c69a-157">Этот пример кода по идентификатору сообщения о событии получает это сообщение, выполняет приведение этого сообщения для доступа к его свойству навигации **event** и применяет параметр $expand для получения свойств события.</span><span class="sxs-lookup"><span data-stu-id="2c69a-157">It uses the event message ID to get the event message, explicitly provides a cast on the event message to access its **event** navigation property, and apply an $expand parameter to get the properties of the event.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c69a-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c69a-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_based_on_eventmessage"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkADYAAAImV_jAAA=/?$expand=microsoft.graph.eventMessage/event
```
# <a name="c"></a>[<span data-ttu-id="2c69a-159">C#</span><span class="sxs-lookup"><span data-stu-id="2c69a-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-based-on-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c69a-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c69a-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-based-on-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c69a-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c69a-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-based-on-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c69a-162">Java</span><span class="sxs-lookup"><span data-stu-id="2c69a-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-based-on-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="2c69a-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c69a-163">Response</span></span>
<span data-ttu-id="2c69a-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2c69a-164">Here is an example of the response.</span></span> <span data-ttu-id="2c69a-165">В отклике возвращаются свойства связанного события.</span><span class="sxs-lookup"><span data-stu-id="2c69a-165">The properties of the associated event are returned in the response.</span></span>
<span data-ttu-id="2c69a-166">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="2c69a-166">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2c69a-167">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c69a-167">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_event_based_on_eventmessage",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessageRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages/$entity",
    "@odata.type":"#microsoft.graph.eventMessageRequest",
    "@odata.etag":"W/\"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVF\"",
    "id":"AAMkADYAAAImV_jAAA=",
    "createdDateTime":"2017-12-27T21:54:55Z",
    "lastModifiedDateTime":"2017-12-27T23:26:38Z",
    "changeKey":"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVF",
    "categories":[

    ],
    "receivedDateTime":"2017-12-27T21:54:55Z",
    "sentDateTime":"2017-12-27T21:54:54Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR1301MB211042CFBF@MWHPR1301MB2110.namprd13.prod.outlook.com>",
    "subject":"Kick off planning",
    "bodyPreview":"Let's collect opinions from our teams and organize action items.",
    "importance":"normal",
    "parentFolderId":"AQMkADYAS4AAAIBDAAAAA==",
    "conversationId":"AAQkADYRuffB3wDlPn-ReFZarI60=",
    "conversationIndex":"AdN/XVP4JG598HfAOU+f9F4VlqsjrQ==",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADYAAAImV%2BjAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "meetingMessageType":"meetingRequest",
    "type":"singleInstance",
    "isOutOfDate":false,
    "isAllDay":false,
    "isDelegated":false,
    "responseRequested":true,
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n<style type=\"text/css\" style=\"display:none\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" dir=\"ltr\" style=\"font-size:12pt; color:#000000; font-family:Calibri,Helvetica,sans-serif\">\r\n<p style=\"margin-top:0; margin-bottom:0\">Let's collect opinions from our teams and organize action items.<br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "sender":{
        "emailAddress":{
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "mentionsPreview":null,
    "flag":{
        "flagStatus":"notFlagged"
    },
    "startDateTime":{
        "dateTime":"2018-02-02T22:00:00.0000000",
        "timeZone":"UTC"
    },
    "endDateTime":{
        "dateTime":"2018-02-02T23:00:00.0000000",
        "timeZone":"UTC"
    },
    "location":{
        "displayName":"Mt. Hood",
        "locationType":"default",
        "uniqueIdType":"unknown"
    },
    "recurrence":null,
    "previousLocation":null,
    "previousStartDateTime":null,
    "previousEndDateTime":null,
    "event@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages('AAMkADYAAAImV_jAAA%3D')/microsoft.graph.eventMessage/event/$entity",
    "event":{
        "@odata.etag":"W/\"V5Qf0i9DeEOoOqPo0mABLgAACJpBWg==\"",
        "id":"AAMkADYAAAImVu6AAA=",
        "createdDateTime":"2017-12-27T21:54:55.2624551Z",
        "lastModifiedDateTime":"2017-12-27T22:19:16.6667889Z",
        "changeKey":"V5Qf0i9DeEOoOqPo0mABLgAACJpBWg==",
        "categories":[

        ],
        "originalStartTimeZone":"Pacific Standard Time",
        "originalEndTimeZone":"Pacific Standard Time",
        "uid":"040000008200E00074C5B7101A82E00800000000A2A6F3535D7FD3010000000000000000100000003D770E2E8974F44B9471BDB348097FE3",
        "reminderMinutesBeforeStart":15,
        "isReminderOn":true,
        "hasAttachments":false,
        "subject":"Kick off planning",
        "bodyPreview":"Let's collect opinions from our teams and organize action items.",
        "importance":"normal",
        "sensitivity":"normal",
        "isAllDay":false,
        "isCancelled":false,
        "isOrganizer":false,
        "responseRequested":true,
        "seriesMasterId":null,
        "showAs":"tentative",
        "type":"singleInstance",
        "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADYAAAImVu6AAA%3D&exvsurl=1&path=/calendar/item",
        "onlineMeetingUrl":null,
        "responseStatus":{
            "response":"tentativelyAccepted",
            "time":"2017-12-27T22:19:12.6197462Z"
        },
        "body":{
            "contentType":"html",
            "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n<style type=\"text/css\" style=\"display:none\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" dir=\"ltr\" style=\"font-size:12pt; color:#000000; font-family:Calibri,Helvetica,sans-serif\">\r\n<p style=\"margin-top:0; margin-bottom:0\">Let's collect opinions from our teams and organize action items.<br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
        },
        "start":{
            "dateTime":"2018-02-02T22:00:00.0000000",
            "timeZone":"UTC"
        },
        "end":{
            "dateTime":"2018-02-02T23:00:00.0000000",
            "timeZone":"UTC"
        },
        "location":{
            "displayName":"Mt. Hood",
            "locationType":"default",
            "uniqueId":"Mt. Hood",
            "uniqueIdType":"private"
        },
        "locations":[
            {
                "displayName":"Mt. Hood",
                "locationType":"default",
                "uniqueId":"Mt. Hood",
                "uniqueIdType":"private"
            }
        ],
        "recurrence":null,
        "attendees":[
            {
                "type":"required",
                "status":{
                    "response":"none",
                    "time":"0001-01-01T00:00:00Z"
                },
                "emailAddress":{
                    "name":"Administrator",
                    "address":"admin@contoso.onmicrosoft.com"
                }
            },
            {
                "type":"required",
                "status":{
                    "response":"tentativelyAccepted",
                    "time":"0001-01-01T00:00:00Z"
                },
                "emailAddress":{
                    "name":"Alex Wilber",
                    "address":"AlexW@contoso.onmicrosoft.com"
                }
            }
        ],
        "organizer":{
            "emailAddress":{
                "name":"Administrator",
                "address":"admin@contoso.onmicrosoft.com"
            }
        },
        "OnlineMeeting":null
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
