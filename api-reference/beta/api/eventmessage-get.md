---
title: Получение объекта eventMessage
description: Разверните узел "параметр на **события**
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ffa2524939e5866bc74d255606a7a28297d691d2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521770"
---
# <a name="get-eventmessage"></a><span data-ttu-id="23828-103">Получение объекта eventMessage</span><span class="sxs-lookup"><span data-stu-id="23828-103">Get eventMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23828-104">Получение свойств и связей объекта [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="23828-104">Get the properties and relationships of the [eventMessage](../resources/eventmessage.md) object.</span></span> <span data-ttu-id="23828-105">Применение `$expand` параметр на свойство навигации **события** для получения связанного [события](../resources/event.md) в календаре участника.</span><span class="sxs-lookup"><span data-stu-id="23828-105">Apply the `$expand` parameter on the **event** navigation property to get the associated [event](../resources/event.md) in an attendee's calendar.</span></span>

### <a name="get-the-event-message-body-in-html-or-text-format"></a><span data-ttu-id="23828-106">Получение событий текст сообщения в формате HTML или текст</span><span class="sxs-lookup"><span data-stu-id="23828-106">Get the event message body in HTML or text format</span></span>

<span data-ttu-id="23828-107">Текст сообщений событий может быть в формате HTML или текст.</span><span class="sxs-lookup"><span data-stu-id="23828-107">Event message bodies can be in HTML or text format.</span></span>

<span data-ttu-id="23828-108">Можно использовать `Prefer: outlook.body-content-type` укажите нужный формат, заголовок, возвращаемых в свойствах **uniqueBody** и **основной текст** в `GET` запроса:</span><span class="sxs-lookup"><span data-stu-id="23828-108">You can use the `Prefer: outlook.body-content-type` header to specify the desired format returned in the **body** and **uniqueBody** properties in a `GET` request:</span></span>

- <span data-ttu-id="23828-109">Укажите `Prefer: outlook.body-content-type="text"` для получения событий текст сообщения, возвращаемые в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="23828-109">Specify `Prefer: outlook.body-content-type="text"` to get a event message body returned in text format.</span></span>
- <span data-ttu-id="23828-110">Укажите `Prefer: outlook.body-content-type="html"`, или просто пропустить заголовка для возврата события текст сообщения в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="23828-110">Specify `Prefer: outlook.body-content-type="html"`, or just skip the header, to return the event message body in HTML format.</span></span>

<span data-ttu-id="23828-111">При указании любого из заголовка ответа будет включать соответствующий `Preference-Applied` заголовок подтверждения:</span><span class="sxs-lookup"><span data-stu-id="23828-111">If you specify either header, the response will include the corresponding `Preference-Applied` header as confirmation:</span></span>

- <span data-ttu-id="23828-112">Чтобы получить результат выполнения запроса в текстовом формате: `Preference-Applied: outlook.body-content-type="text"`</span><span class="sxs-lookup"><span data-stu-id="23828-112">For text format requests: `Preference-Applied: outlook.body-content-type="text"`</span></span>
- <span data-ttu-id="23828-113">Чтобы получить результат выполнения запроса в формате HTML: `Preference-Applied: outlook.body-content-type="html"`</span><span class="sxs-lookup"><span data-stu-id="23828-113">For HTML format requests: `Preference-Applied: outlook.body-content-type="html"`</span></span>

## <a name="permissions"></a><span data-ttu-id="23828-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23828-114">Permissions</span></span>
<span data-ttu-id="23828-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23828-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23828-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23828-117">Permission type</span></span>      | <span data-ttu-id="23828-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23828-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23828-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23828-119">Delegated (work or school account)</span></span> | <span data-ttu-id="23828-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="23828-120">Mail.Read</span></span>    |
|<span data-ttu-id="23828-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23828-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23828-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="23828-122">Mail.Read</span></span>    |
|<span data-ttu-id="23828-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23828-123">Application</span></span> | <span data-ttu-id="23828-124">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="23828-124">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="23828-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23828-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="23828-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="23828-126">Optional query parameters</span></span>
<span data-ttu-id="23828-127">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="23828-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="23828-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23828-128">Request headers</span></span>
| <span data-ttu-id="23828-129">Имя</span><span class="sxs-lookup"><span data-stu-id="23828-129">Name</span></span>       | <span data-ttu-id="23828-130">Тип</span><span class="sxs-lookup"><span data-stu-id="23828-130">Type</span></span> | <span data-ttu-id="23828-131">Описание</span><span class="sxs-lookup"><span data-stu-id="23828-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="23828-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="23828-132">Authorization</span></span>  | <span data-ttu-id="23828-133">string</span><span class="sxs-lookup"><span data-stu-id="23828-133">string</span></span>  | <span data-ttu-id="23828-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23828-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23828-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23828-136">Request body</span></span>
<span data-ttu-id="23828-137">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23828-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23828-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="23828-138">Response</span></span>

<span data-ttu-id="23828-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [eventMessage](../resources/eventmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23828-139">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23828-140">Пример</span><span class="sxs-lookup"><span data-stu-id="23828-140">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="23828-141">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="23828-141">Request 1</span></span>
<span data-ttu-id="23828-142">Первый пример показывает, как получить свойства сообщения о событии с учетом идентификатора этого сообщения.</span><span class="sxs-lookup"><span data-stu-id="23828-142">The first example shows how to get the properties of an event message based on the event message ID.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_eventmessage"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADYAAAImV_lAAA=')
```
##### <a name="response-1"></a><span data-ttu-id="23828-143">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="23828-143">Response 1</span></span>
<span data-ttu-id="23828-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="23828-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="23828-147">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="23828-147">Request 2</span></span>
<span data-ttu-id="23828-148">Второй пример показывает, как получить событие, связанное с сообщением о событии.</span><span class="sxs-lookup"><span data-stu-id="23828-148">The second example shows how to get the event associated with an event message.</span></span> <span data-ttu-id="23828-149">Этот пример кода по идентификатору сообщения о событии получает это сообщение, выполняет приведение этого сообщения для доступа к его свойству навигации **event** и применяет параметр $expand для получения свойств события.</span><span class="sxs-lookup"><span data-stu-id="23828-149">It uses the event message ID to get the event message, explicitly provides a cast on the event message to access its **event** navigation property, and apply an $expand parameter to get the properties of the event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_event_based_on_eventmessage"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADYAAAImV_jAAA=')?$expand=microsoft.graph.eventMessage/event
```
##### <a name="response-2"></a><span data-ttu-id="23828-150">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="23828-150">Response 2</span></span>
<span data-ttu-id="23828-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23828-151">Here is an example of the response.</span></span> <span data-ttu-id="23828-152">В отклике возвращаются свойства связанного события.</span><span class="sxs-lookup"><span data-stu-id="23828-152">The properties of the associated event are returned in the response.</span></span>
<span data-ttu-id="23828-153">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="23828-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="23828-154">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23828-154">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/eventmessage-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
