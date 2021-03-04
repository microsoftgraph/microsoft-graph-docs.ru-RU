---
title: Перечисление событий
description: 'Получение списка объектов event из стандартного календаря пользователя или '
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 726fa26ce41571050c94c74165a2898ca767b8d3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433567"
---
# <a name="list-events"></a><span data-ttu-id="ffda4-103">Перечисление событий</span><span class="sxs-lookup"><span data-stu-id="ffda4-103">List events</span></span>

<span data-ttu-id="ffda4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffda4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffda4-105">Получение списка объектов [event](../resources/event.md) из стандартного календаря пользователя или указанного календаря.</span><span class="sxs-lookup"><span data-stu-id="ffda4-105">Get a list of [event](../resources/event.md) objects from the user's default calendar or from a specified calendar.</span></span> <span data-ttu-id="ffda4-106">В этом списке указаны единичные собрания и главные собрания в соответствующих рядах.</span><span class="sxs-lookup"><span data-stu-id="ffda4-106">The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="ffda4-107">Чтобы получить расширенные экземпляры события, вы можете [получить представление календаря](calendar-list-calendarview.md) или [экземпляры события](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="ffda4-107">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

<span data-ttu-id="ffda4-108">Существует два сценария, в которых приложение может получить события из календаря другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="ffda4-108">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="ffda4-109">если у приложения есть разрешения для приложений;</span><span class="sxs-lookup"><span data-stu-id="ffda4-109">If the app has application permissions, or,</span></span>
* <span data-ttu-id="ffda4-110">если у приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним календарем или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="ffda4-110">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="ffda4-111">См. [подробные сведения и пример](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="ffda4-111">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="ffda4-112">Поддержка разных часовых поясов</span><span class="sxs-lookup"><span data-stu-id="ffda4-112">Support various time zones</span></span>

<span data-ttu-id="ffda4-113">Для всех операций GET, которые возвращают события, можно использовать заголовок `Prefer: outlook.timezone`, чтобы задать часовой пояс для указанного в отклике времени начала и завершения события.</span><span class="sxs-lookup"><span data-stu-id="ffda4-113">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="ffda4-114">Например, заголовок `Prefer: outlook.timezone` задает в отклике время начала и завершения согласно североамериканскому восточному времени.</span><span class="sxs-lookup"><span data-stu-id="ffda4-114">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="ffda4-p103">Если событие создано с применением другого часового пояса, время начала и завершения будет изменено в соответствии с часовым поясом, указанным в заголовке `Prefer`. Поддерживаемые часовые пояса указаны в этом [списке](../resources/datetimetimezone.md). Если заголовок `Prefer: outlook.timezone` не указан, время начала и завершения возвращается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="ffda4-p103">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="ffda4-118">Узнать, какой именно часовой пояс использовался при создании события, позволят свойства **OriginalStartTimeZone** и **OriginalEndTimeZone** ресурса **event**.</span><span class="sxs-lookup"><span data-stu-id="ffda4-118">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="ffda4-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ffda4-119">Permissions</span></span>
<span data-ttu-id="ffda4-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffda4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffda4-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffda4-122">Permission type</span></span>      | <span data-ttu-id="ffda4-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffda4-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffda4-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffda4-124">Delegated (work or school account)</span></span> | <span data-ttu-id="ffda4-125">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ffda4-125">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ffda4-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffda4-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffda4-127">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ffda4-127">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ffda4-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffda4-128">Application</span></span> | <span data-ttu-id="ffda4-129">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ffda4-129">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ffda4-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffda4-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events
GET /users/{id | userPrincipalName}/events

GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events

GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendargroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ffda4-131">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ffda4-131">Optional query parameters</span></span>
<span data-ttu-id="ffda4-132">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ffda4-132">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ffda4-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffda4-133">Request headers</span></span>
| <span data-ttu-id="ffda4-134">Имя</span><span class="sxs-lookup"><span data-stu-id="ffda4-134">Name</span></span>       | <span data-ttu-id="ffda4-135">Тип</span><span class="sxs-lookup"><span data-stu-id="ffda4-135">Type</span></span> | <span data-ttu-id="ffda4-136">Описание</span><span class="sxs-lookup"><span data-stu-id="ffda4-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ffda4-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffda4-137">Authorization</span></span>  | <span data-ttu-id="ffda4-138">string</span><span class="sxs-lookup"><span data-stu-id="ffda4-138">string</span></span>  | <span data-ttu-id="ffda4-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffda4-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ffda4-141">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="ffda4-141">Prefer: outlook.timezone</span></span> | <span data-ttu-id="ffda4-142">string</span><span class="sxs-lookup"><span data-stu-id="ffda4-142">string</span></span> | <span data-ttu-id="ffda4-143">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="ffda4-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="ffda4-144">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="ffda4-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="ffda4-145">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="ffda4-145">Optional.</span></span> |
| <span data-ttu-id="ffda4-146">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="ffda4-146">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="ffda4-147">string</span><span class="sxs-lookup"><span data-stu-id="ffda4-147">string</span></span> | <span data-ttu-id="ffda4-148">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="ffda4-148">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="ffda4-149">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="ffda4-149">Values can be "text" or "html".</span></span> <span data-ttu-id="ffda4-150">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="ffda4-150">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="ffda4-151">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="ffda4-151">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="ffda4-152">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="ffda4-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffda4-153">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ffda4-153">Request body</span></span>
<span data-ttu-id="ffda4-154">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ffda4-154">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffda4-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffda4-155">Response</span></span>

<span data-ttu-id="ffda4-156">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ffda4-156">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ffda4-157">Пример</span><span class="sxs-lookup"><span data-stu-id="ffda4-157">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="ffda4-158">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="ffda4-158">Request 1</span></span>
<span data-ttu-id="ffda4-159">В первом примере возвращаются все события пользователя.</span><span class="sxs-lookup"><span data-stu-id="ffda4-159">The first example gets all the user's events.</span></span> <span data-ttu-id="ffda4-160">В нем указывается:</span><span class="sxs-lookup"><span data-stu-id="ffda4-160">It specifies the following:</span></span>

- <span data-ttu-id="ffda4-161">Заголовок `Prefer: outlook.timezone` для получения значений даты и времени, которые возвращаются для стандартного тихоокеанского времени.</span><span class="sxs-lookup"><span data-stu-id="ffda4-161">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="ffda4-p109">Параметр запроса `$select`, который возвращает конкретные свойства. Без параметра `$select` будут возвращены все свойства событий.</span><span class="sxs-lookup"><span data-stu-id="ffda4-p109">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="ffda4-164">В запросе не определен никакой заголовок `Prefer: outlook.body-content-type`, чтобы указать конкретный формат для текста возвращаемого события.</span><span class="sxs-lookup"><span data-stu-id="ffda4-164">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 


# <a name="http"></a>[<span data-ttu-id="ffda4-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="ffda4-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[<span data-ttu-id="ffda4-166">C#</span><span class="sxs-lookup"><span data-stu-id="ffda4-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ffda4-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ffda4-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ffda4-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ffda4-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ffda4-169">Java</span><span class="sxs-lookup"><span data-stu-id="ffda4-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="ffda4-170">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="ffda4-170">Response 1</span></span>
<span data-ttu-id="ffda4-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ffda4-171">Here is an example of the response.</span></span> <span data-ttu-id="ffda4-172">Так как заголовок `Prefer: outlook.body-content-type` не указан, свойство **body** возвращается в формате HTML по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ffda4-172">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_events",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-length: 1932

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)",
    "value":[
        {
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
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
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
    ]
}
```

##### <a name="request-2"></a><span data-ttu-id="ffda4-173">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="ffda4-173">Request 2</span></span>
<span data-ttu-id="ffda4-174">Во втором примере показано, как использовать заголовок `Prefer: outlook.body-content-type="text"`, чтобы получить свойство **body** указанного сообщения в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="ffda4-174">The second example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified message in text format.</span></span>

<span data-ttu-id="ffda4-175">В запросе также используется параметр `$select` для возврата отдельных свойств.</span><span class="sxs-lookup"><span data-stu-id="ffda4-175">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="ffda4-176">Без параметра `$select` будут возвращены все свойства событий.</span><span class="sxs-lookup"><span data-stu-id="ffda4-176">Without a `$select` parameter, all of the event properties will be returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="ffda4-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="ffda4-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_events_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text" 
```
# <a name="c"></a>[<span data-ttu-id="ffda4-178">C#</span><span class="sxs-lookup"><span data-stu-id="ffda4-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-events-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ffda4-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ffda4-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-events-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ffda4-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ffda4-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-events-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ffda4-181">Java</span><span class="sxs-lookup"><span data-stu-id="ffda4-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-events-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="ffda4-182">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="ffda4-182">Response 2</span></span>
<span data-ttu-id="ffda4-183">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ffda4-183">Here is an example of the response.</span></span> <span data-ttu-id="ffda4-184">Свойство **body** возвращается в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="ffda4-184">The **body** property is returned in text format.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"
Content-length: 640

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview)",
    "value":[
        {
            "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
            "id":"AAMkAGIAAAoZDOFAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            }
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
