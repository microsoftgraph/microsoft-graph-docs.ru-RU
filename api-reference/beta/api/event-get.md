---
title: Вывод события
description: Получение свойств и отношений указанного объекта event.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 22f72f23d0521b6e78e4d776b0e5e0288ebba46a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43365513"
---
# <a name="get-event"></a><span data-ttu-id="c4a65-103">Вывод события</span><span class="sxs-lookup"><span data-stu-id="c4a65-103">Get event</span></span>

<span data-ttu-id="c4a65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4a65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4a65-105">Получение свойств и отношений указанного объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="c4a65-105">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="c4a65-106">Существует два сценария, в которых приложение может получить событие из календаря другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="c4a65-106">There are two scenarios where an app can get an event in another user's calendar:</span></span>

* <span data-ttu-id="c4a65-107">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="c4a65-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="c4a65-108">если у приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним календарем или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="c4a65-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="c4a65-109">См. [подробные сведения и пример](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="c4a65-109">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

<span data-ttu-id="c4a65-110">Так как ресурс **event** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` вы можете получить настраиваемые свойства и данные расширения в экземпляре **события**.</span><span class="sxs-lookup"><span data-stu-id="c4a65-110">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="c4a65-111">Поддержка разных часовых поясов</span><span class="sxs-lookup"><span data-stu-id="c4a65-111">Support various time zones</span></span>

<span data-ttu-id="c4a65-112">Для всех операций GET, которые возвращают события, можно использовать заголовок `Prefer: outlook.timezone`, чтобы задать часовой пояс для указанного в отклике времени начала и завершения события.</span><span class="sxs-lookup"><span data-stu-id="c4a65-112">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="c4a65-113">Например, заголовок `Prefer: outlook.timezone` задает в отклике время начала и завершения согласно североамериканскому восточному времени.</span><span class="sxs-lookup"><span data-stu-id="c4a65-113">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="c4a65-p102">Если событие создано с применением другого часового пояса, время начала и завершения будет изменено в соответствии с часовым поясом, указанным в заголовке `Prefer`. Поддерживаемые часовые пояса указаны в этом [списке](../resources/datetimetimezone.md). Если заголовок `Prefer: outlook.timezone` не указан, время начала и завершения возвращается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c4a65-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="c4a65-117">Узнать, какой именно часовой пояс использовался при создании события, позволят свойства **OriginalStartTimeZone** и **OriginalEndTimeZone** ресурса **event**.</span><span class="sxs-lookup"><span data-stu-id="c4a65-117">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4a65-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4a65-118">Permissions</span></span>
<span data-ttu-id="c4a65-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4a65-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4a65-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4a65-121">Permission type</span></span>      | <span data-ttu-id="c4a65-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4a65-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4a65-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4a65-123">Delegated (work or school account)</span></span> | <span data-ttu-id="c4a65-124">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c4a65-124">Calendars.Read</span></span>    |
|<span data-ttu-id="c4a65-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4a65-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4a65-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c4a65-126">Calendars.Read</span></span>    |
|<span data-ttu-id="c4a65-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4a65-127">Application</span></span> | <span data-ttu-id="c4a65-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c4a65-128">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4a65-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4a65-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}
GET /users/{id | userPrincipalName}/events/{id}
GET /groups/{id}/events/{id}

GET /me/calendar/events/{id}
GET /users/{id | userPrincipalName}/calendar/events/{id}
GET /groups/{id}/calendar/events/{id}

GET /me/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}

GET /me/calendargroup/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c4a65-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c4a65-130">Optional query parameters</span></span>
<span data-ttu-id="c4a65-131">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c4a65-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c4a65-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4a65-132">Request headers</span></span>
| <span data-ttu-id="c4a65-133">Имя</span><span class="sxs-lookup"><span data-stu-id="c4a65-133">Name</span></span>       | <span data-ttu-id="c4a65-134">Тип</span><span class="sxs-lookup"><span data-stu-id="c4a65-134">Type</span></span> | <span data-ttu-id="c4a65-135">Описание</span><span class="sxs-lookup"><span data-stu-id="c4a65-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c4a65-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4a65-136">Authorization</span></span>  | <span data-ttu-id="c4a65-137">string</span><span class="sxs-lookup"><span data-stu-id="c4a65-137">string</span></span>  | <span data-ttu-id="c4a65-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4a65-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c4a65-140">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="c4a65-140">Prefer: outlook.timezone</span></span> | <span data-ttu-id="c4a65-141">string</span><span class="sxs-lookup"><span data-stu-id="c4a65-141">string</span></span> | <span data-ttu-id="c4a65-142">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="c4a65-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="c4a65-143">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c4a65-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="c4a65-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c4a65-144">Optional.</span></span> |
| <span data-ttu-id="c4a65-145">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="c4a65-145">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="c4a65-146">string</span><span class="sxs-lookup"><span data-stu-id="c4a65-146">string</span></span> | <span data-ttu-id="c4a65-147">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="c4a65-147">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="c4a65-148">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="c4a65-148">Values can be "text" or "html".</span></span> <span data-ttu-id="c4a65-149">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="c4a65-149">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="c4a65-150">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="c4a65-150">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="c4a65-151">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c4a65-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4a65-152">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c4a65-152">Request body</span></span>
<span data-ttu-id="c4a65-153">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4a65-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4a65-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4a65-154">Response</span></span>

<span data-ttu-id="c4a65-155">В случае успеха этот метод возвратит код отклика `200 OK` и объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c4a65-155">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c4a65-156">Пример</span><span class="sxs-lookup"><span data-stu-id="c4a65-156">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="c4a65-157">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="c4a65-157">Request 1</span></span>
<span data-ttu-id="c4a65-p107">Первый пример возвращает указанное событие. Он указывает следующее:</span><span class="sxs-lookup"><span data-stu-id="c4a65-p107">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="c4a65-160">Заголовок `Prefer: outlook.timezone` для получения значений даты и времени, которые возвращаются для стандартного тихоокеанского времени.</span><span class="sxs-lookup"><span data-stu-id="c4a65-160">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="c4a65-p108">Параметр запроса `$select`, который возвращает конкретные свойства. Без параметра `$select` будут возвращены все свойства событий.</span><span class="sxs-lookup"><span data-stu-id="c4a65-p108">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="c4a65-163">В запросе не определен никакой заголовок `Prefer: outlook.body-content-type`, чтобы указать конкретный формат для текста возвращаемого события.</span><span class="sxs-lookup"><span data-stu-id="c4a65-163">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 


# <a name="http"></a>[<span data-ttu-id="c4a65-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4a65-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGIAAAoZDOFAAA=/?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[<span data-ttu-id="c4a65-165">C#</span><span class="sxs-lookup"><span data-stu-id="c4a65-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4a65-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4a65-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4a65-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4a65-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="c4a65-168">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="c4a65-168">Response 1</span></span>
<span data-ttu-id="c4a65-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c4a65-169">Here is an example of the response.</span></span> <span data-ttu-id="c4a65-170">Так как заголовок `Prefer: outlook.body-content-type` не указан, свойство **body** возвращается в формате HTML по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c4a65-170">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-length: 1928

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
    "id":"AAMkAGIAAAoZDOFAAA=",
    "subject":"Orientation ",
    "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
    "body":{
        "contentType":"html",
        "content":"<html><head></head><body><p>Dana, this is the time you selected for our orientation. Please bring the notes I sent you.</p></body></html>"
    },
    "start":{
        "dateTime":"2017-04-21T10:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-04-21T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location": {
        "displayName": "Assembly Hall",
        "locationType": "default",
        "uniqueId": "Assembly Hall",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Assembly Hall",
            "locationType": "default",
            "uniqueIdType": "unknown"
        }
    ],
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Samantha Booth",
                "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
            }
        },
        {
            "type":"required",
            "status":{
                "response":"tentativelyAccepted",
                "time":"0001-01-01T00:00:00Z"
            },
            "proposedNewTime": {
                "start": {
                    "dateTime": "2019-08-16T12:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-08-16T14:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            },
            "emailAddress":{
                "name":"Dana Swope",
                "address":"danas@a830edad905084922E17020313.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Samantha Booth",
            "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
        }
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="c4a65-171">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="c4a65-171">Request 2</span></span>
<span data-ttu-id="c4a65-172">Во втором примере показано, как использовать `Prefer: outlook.body-content-type="text"` заголовок для получения свойства **Body** указанного события в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="c4a65-172">The second example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified event in text format.</span></span>

<span data-ttu-id="c4a65-173">В запросе также используется параметр `$select` для возврата отдельных свойств.</span><span class="sxs-lookup"><span data-stu-id="c4a65-173">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="c4a65-174">Без параметра `$select` будут возвращены все свойства событий.</span><span class="sxs-lookup"><span data-stu-id="c4a65-174">Without a `$select` parameter, all of the event properties will be returned.</span></span>


# <a name="http"></a>[<span data-ttu-id="c4a65-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4a65-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGI1AAAoZDOFAAA=/?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="c4a65-176">C#</span><span class="sxs-lookup"><span data-stu-id="c4a65-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4a65-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4a65-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4a65-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4a65-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="c4a65-179">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="c4a65-179">Response 2</span></span>
<span data-ttu-id="c4a65-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c4a65-180">Here is an example of the response.</span></span> <span data-ttu-id="c4a65-181">Свойство **body** возвращается в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="c4a65-181">The **body** property is returned in text format.</span></span> 

<!-- {
  "blockType": "response",
  "name": "get_event_in_text",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"
Content-length: 636

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview)/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
    "id":"AAMkAGI1AAAoZDOFAAA=",
    "subject":"Orientation ",
    "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
    "body":{
        "contentType":"text",
        "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
    }
}
```


##### <a name="request-3"></a><span data-ttu-id="c4a65-182">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="c4a65-182">Request 3</span></span>

<span data-ttu-id="c4a65-183">В третьем примере показано, как получается событие, задающее несколько расположений.</span><span class="sxs-lookup"><span data-stu-id="c4a65-183">The third example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="c4a65-184">В запросе указан параметр `$select` для возврата отдельных свойств.</span><span class="sxs-lookup"><span data-stu-id="c4a65-184">The request specifies a `$select` query parameter to return specific properties.</span></span> 


# <a name="http"></a>[<span data-ttu-id="c4a65-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4a65-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_multiple_locations"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkADAGAADDdm4NAAA=/?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
# <a name="c"></a>[<span data-ttu-id="c4a65-186">C#</span><span class="sxs-lookup"><span data-stu-id="c4a65-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-multiple-locations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4a65-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4a65-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-multiple-locations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4a65-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4a65-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-multiple-locations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-3"></a><span data-ttu-id="c4a65-189">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="c4a65-189">Response 3</span></span>
<span data-ttu-id="c4a65-190">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c4a65-190">Here is an example of the response.</span></span> <span data-ttu-id="c4a65-191">Свойство **locations** включает информацию о трех местах, для которых организовано событие.</span><span class="sxs-lookup"><span data-stu-id="c4a65-191">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="c4a65-192">Так как в запросе не указано ни `Prefer: outlook.timezone` одного `Prefer: outlook.body-content-type` заголовка или заголовка, свойства **Start** и **End** отображаются в ЧАСОВОМ поясе по умолчанию в формате UTC, а текст по умолчанию — в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="c4a65-192">Because the request does not specify any `Prefer: outlook.timezone` or `Prefer: outlook.body-content-type` header, the **start** and **end** properties are displayed in the default UTC time zone, and the body is in the default HTML format.</span></span>  

<!-- {
  "blockType": "response",
  "name": "get_event_multiple_locations",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1992

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,locations)/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "subject":"Plan summer company picnic",
  "bodyPreview":"Let's kick-start this event planning!",
  "body":{
    "contentType":"html",
    "content":"<html>\r\n<head>\r\n</head>\r\n<body>\r\nLet's kick-start this event planning!\r\n</body>\r\n</html>\r\n"
  },
  "start":{
    "dateTime":"2017-08-30T11:00:00.0000000",
    "timeZone":"UTC"
  },
  "end":{
    "dateTime":"2017-08-30T12:00:00.0000000",
    "timeZone":"UTC"
  },
  "location":{
    "displayName":"Conf Room 3; Fourth Coffee; Home Office",
    "locationType":"default",
    "uniqueId":"Conf Room 3; Fourth Coffee; Home Office",
    "uniqueIdType":"private"
  },
  "locations":[
    {
      "displayName":"Conf Room 3",
      "locationType":"default",
      "uniqueIdType":"unknown"
    },
    {
      "displayName":"Fourth Coffee",
      "locationType":"default",
      "uniqueId":"Fourth Coffee",
      "uniqueIdType":"private",
      "address":{
        "type":"unknown",
        "street":"4567 Main St",
        "city":"Redmond",
        "state":"WA",
        "countryOrRegion":"US",
        "postalCode":"32008"
      },
      "coordinates":{
        "latitude":47.672,
        "longitude":-102.103
      }
    },
    {
      "displayName":"Home Office",
      "locationType":"default",
      "uniqueIdType":"unknown"
    }
  ],
  "attendees":[
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Dana Swope",
        "address":"DanaS@contoso.onmicrosoft.com"
      }
    },
    {
      "type":"required",
      "status":{
        "response":"none",
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
      "name":"Adele Vance",
      "address":"AdeleV@contoso.onmicrosoft.com"
    }
  }
}
```

## <a name="see-also"></a><span data-ttu-id="c4a65-193">См. также</span><span class="sxs-lookup"><span data-stu-id="c4a65-193">See also</span></span>

- [<span data-ttu-id="c4a65-194">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="c4a65-194">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c4a65-195">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="c4a65-195">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="c4a65-196">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="c4a65-196">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
