---
title: 'Получение добавочных изменений для событий в представлении календаря '
description: 'Представление календаря — это коллекция событий в диапазоне дат и времени из календаря по умолчанию (../me/calendarview) '
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 2eeb1b403b772ea6693b9644e286fd0c60575731
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272249"
---
# <a name="get-incremental-changes-to-events-in-a-calendar-view"></a><span data-ttu-id="d300d-103">Получение добавочных изменений для событий в представлении календаря</span><span class="sxs-lookup"><span data-stu-id="d300d-103">Get incremental changes to events in a calendar view</span></span> 

<span data-ttu-id="d300d-p101">Представление календаря — это коллекция событий в диапазоне дат и времени из календаря по умолчанию (../me/calendarview) или другого календаря пользователя. С помощью запроса изменений вы можете получать новые, обновленные или удаленные события в представлении календаря. Возвращаемые события могут включать повторения и исключения из повторяющейся серии, а также отдельные экземпляры. Разностные данные позволяют поддерживать и синхронизировать локальное хранилище событий пользователя. При этом вам не требуется каждый раз получать весь набор событий пользователя с сервера.</span><span class="sxs-lookup"><span data-stu-id="d300d-p101">A calendar view is a collection of events in a date/time range from the default calendar (../me/calendarview) or some other calendar of the user's. By using delta query, you can get new, updated, or deleted events in a calendar view. The returned events may include occurrences and exceptions of a recurring series, and single instances. The delta data enables you to maintain and synchronize a local store of a user's events, without having to fetch the entire set of the user's events from the server every time.</span></span>

<span data-ttu-id="d300d-p102">Запрос изменений поддерживает как полную синхронизацию с получением всех событий в определенном представлении календаря, так и добавочную синхронизацию с получением тех событий, которые изменились в представлении календаря с момента последней синхронизации. Как правило, сначала выполняется полная синхронизация, а затем в представление календаря периодически добавляются изменения.</span><span class="sxs-lookup"><span data-stu-id="d300d-p102">Delta query supports both full synchronization that retrieves all the events in the specified calendar view, and incremental synchronization that retrieves those events that have changed in the calendar view since the last synchronization. Typically, you would do an initial full synchronization, and subsequently, get incremental changes to that calendar view periodically.</span></span> 

## <a name="track-event-changes-in-a-calendar-view"></a><span data-ttu-id="d300d-110">Отслеживание изменений событий в представлении календаря</span><span class="sxs-lookup"><span data-stu-id="d300d-110">Track event changes in a calendar view</span></span>

<span data-ttu-id="d300d-p103">Запрос изменений для событий относится к указанным календарю и диапазону дат и времени (т. е. представлению календаря). Чтобы отслеживать изменения в нескольких календарях, необходимо наблюдать за каждым календарем отдельно.</span><span class="sxs-lookup"><span data-stu-id="d300d-p103">Delta query for events is specific to a calendar and date/time range that you specify (i.e., a calendar view). To track the changes in multiple calendars, you need to track each calendar individually.</span></span> 

<span data-ttu-id="d300d-p104">Как правило, цикл отслеживания изменений событий в представлении календаря состоит из одного или нескольких запросов GET с функцией [delta](/graph/api/event-delta?view=graph-rest-1.0). Исходный запрос GET во многом аналогичен [получению списка calendarView](/graph/api/calendar-list-calendarview?view=graph-rest-1.0), но он также содержит функцию **delta**:</span><span class="sxs-lookup"><span data-stu-id="d300d-p104">Tracking event changes in a calendar view typically is a round of one or more GET requests with the [delta](/graph/api/event-delta?view=graph-rest-1.0) function. The initial GET request is very much like the way you [list a calendarView](/graph/api/calendar-list-calendarview?view=graph-rest-1.0), except that you include the **delta** function:</span></span>

```
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="d300d-115">Запрос GET с функцией **delta** возвращает одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="d300d-115">A GET request with the **delta** function returns either:</span></span>

- <span data-ttu-id="d300d-116">ссылку `nextLink` (содержащую URL-адрес с вызовом функции **delta** и маркером _skipToken_);</span><span class="sxs-lookup"><span data-stu-id="d300d-116">A `nextLink` (that contains a URL with a **delta** function call and a _skipToken_), or</span></span> 
- <span data-ttu-id="d300d-117">ссылку `deltaLink` (содержащую URL-адрес с вызовом функции **delta** и маркером _deltaToken_).</span><span class="sxs-lookup"><span data-stu-id="d300d-117">A `deltaLink` (that contains a URL with a **delta** function call and _deltaToken_).</span></span>

<span data-ttu-id="d300d-118">Эти маркеры являются [маркерами состояния](delta-query-overview.md#state-tokens), кодирующими параметры _startDateTime_ и _endDateTime_ конечной точки refs/remotes/microsoftgraph/master, а также любой другой параметр в исходном запросе изменений GET.</span><span class="sxs-lookup"><span data-stu-id="d300d-118">These tokens are [state tokens](delta-query-overview.md#state-tokens) which encode the refs/remotes/microsoftgraph/master _startDateTime_ and _endDateTime_ parameters, and any other query parameter in your initial delta query GET request.</span></span> 

<span data-ttu-id="d300d-p105">Маркеры состояния полностью непрозрачны для клиента. Чтобы продолжить цикл отслеживания изменений, просто скопируйте и примените URL-адрес `nextLink` или `deltaLink`, возвращенный последним запросом GET, при следующем вызове функции **delta** для этого представления календаря. Ссылка `deltaLink` в ответе означает, что текущий цикл отслеживания изменений завершен. Вы можете сохранить и использовать URL-адрес `deltaLink` в начале следующего цикла.</span><span class="sxs-lookup"><span data-stu-id="d300d-p105">State tokens are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next **delta** function call for that same calendar view. A `deltaLink` returned in a response signifies that the current round of change tracking is complete. You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="d300d-123">В приведенном ниже [примере](#example-to-synchronize-events-in-a-calendar-view) показано, как использовать URL-адреса `nextLink` и `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="d300d-123">See the [example](#example-to-synchronize-events-in-a-calendar-view) below to learn how to use these `nextLink` and `deltaLink` URLs.</span></span>

### <a name="use-query-parameters-in-a-delta-query-for-calendar-view"></a><span data-ttu-id="d300d-124">Использование параметров запроса изменений для представления календаря</span><span class="sxs-lookup"><span data-stu-id="d300d-124">Use query parameters in a delta query for calendar view</span></span>

- <span data-ttu-id="d300d-125">Укажите параметры _startDateTime_ и _endDateTime_, чтобы определить диапазон дат и времени для представления календаря.</span><span class="sxs-lookup"><span data-stu-id="d300d-125">Include the _startDateTime_ and _endDateTime_ parameters to define a date/time range for your calendar view.</span></span>
- <span data-ttu-id="d300d-126">Параметр `$select` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d300d-126">`$select` is not supported.</span></span>


### <a name="optional-request-header"></a><span data-ttu-id="d300d-127">Необязательный заголовок запроса</span><span class="sxs-lookup"><span data-stu-id="d300d-127">Optional request header</span></span>

<span data-ttu-id="d300d-128">Каждый разностный запрос GET возвращает коллекцию из одного или нескольких событий в отклике.</span><span class="sxs-lookup"><span data-stu-id="d300d-128">Each delta query GET request returns a collection of one or more events in the response.</span></span> <span data-ttu-id="d300d-129">При необходимости вы можете указать заголовок запроса `Prefer: odata.maxpagesize={x}`, чтобы задать максимальное количество событий в отклике.</span><span class="sxs-lookup"><span data-stu-id="d300d-129">You can optionally specify the request header, `Prefer: odata.maxpagesize={x}`, to set the maximum number of events in a response.</span></span>


## <a name="example-to-synchronize-events-in-a-calendar-view"></a><span data-ttu-id="d300d-130">Пример синхронизации событий в представлении календаря</span><span class="sxs-lookup"><span data-stu-id="d300d-130">Example to synchronize events in a calendar view</span></span>

<span data-ttu-id="d300d-p107">В приведенном ниже примере показана серия из 3 запросов, синхронизирующих календарь пользователя по умолчанию в определенном диапазоне времени. Это представление календаря содержит 5 событий.</span><span class="sxs-lookup"><span data-stu-id="d300d-p107">The following example shows a series of 3 requests to synchronize the user's default calendar in a specific time range. There are 5 events in that calendar view.</span></span>

- <span data-ttu-id="d300d-133">[Шаг 1. Пример исходного запроса](#step-1-sample-initial-request) и [ответ](#sample-initial-response)</span><span class="sxs-lookup"><span data-stu-id="d300d-133">[Step 1: sample initial request](#step-1-sample-initial-request) and [response](#sample-initial-response)</span></span>
- <span data-ttu-id="d300d-134">[Шаг 2. Пример второго запроса](#step-2-sample-second-request) и [ответ](#sample-second-response)</span><span class="sxs-lookup"><span data-stu-id="d300d-134">[Step 2: sample second request](#step-2-sample-second-request) and [response](#sample-second-response)</span></span>
- <span data-ttu-id="d300d-135">[Шаг 3. Пример третьего запроса](#step-3-sample-third-request) и [последний ответ](#sample-third-and-final-response)</span><span class="sxs-lookup"><span data-stu-id="d300d-135">[Step 3: sample third request](#step-3-sample-third-request) and [final response](#sample-third-and-final-response)</span></span>

<span data-ttu-id="d300d-p108">В примерах показаны только некоторые свойства события. При фактическом вызове возвращается большинство свойств события.</span><span class="sxs-lookup"><span data-stu-id="d300d-p108">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span> 

<span data-ttu-id="d300d-138">См. также, что можно сделать в [следующем цикле](#the-next-round-sample-first-response).</span><span class="sxs-lookup"><span data-stu-id="d300d-138">See also what you'll do in the [next round](#the-next-round-sample-first-response).</span></span>


### <a name="step-1-sample-initial-request"></a><span data-ttu-id="d300d-139">Шаг 1. Пример исходного запроса</span><span class="sxs-lookup"><span data-stu-id="d300d-139">Step 1: sample initial request</span></span>

<span data-ttu-id="d300d-p109">В этом примере указанное представление календаря синхронизируется впервые, поэтому исходный запрос на синхронизацию не содержит маркер состояния. В этом цикле возвращаются все события в представлении календаря.</span><span class="sxs-lookup"><span data-stu-id="d300d-p109">In this example, the specified calendar view is being synchronized for the first time, so the initial sync request does not include any state token. This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="d300d-142">Первый запрос задает следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="d300d-142">The first request specifies the following:</span></span>

- <span data-ttu-id="d300d-143">значения даты и времени для параметров _startDateTime_ и _endDateTime_;</span><span class="sxs-lookup"><span data-stu-id="d300d-143">Date/time values for the _startDateTime_ and _endDateTime_ parameters.</span></span>
- <span data-ttu-id="d300d-144">[необязательный заголовок запроса](#optional-request-header) _odata.maxpagesize_, возвращающий 2 события одновременно.</span><span class="sxs-lookup"><span data-stu-id="d300d-144">The [optional request header](#optional-request-header), _odata.maxpagesize_, returning 2 events at a time.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime=2016-12-01T00:00:00Z&enddatetime=2016-12-30T00:00:00Z HTTP/1.1
Prefer: odata.maxpagesize=2
```


### <a name="sample-initial-response"></a><span data-ttu-id="d300d-145">Пример исходного ответа</span><span class="sxs-lookup"><span data-stu-id="d300d-145">Sample initial response</span></span>

<span data-ttu-id="d300d-p110">Ответ включает два события и заголовок ответа `@odata.nextLink` с маркером `skipToken`. URL-адрес `nextLink` указывает, что получены не все события в представлении календаря.</span><span class="sxs-lookup"><span data-stu-id="d300d-p110">The response includes two events and a `@odata.nextLink` response header with a `skipToken`. The `nextLink` URL indicates there are more events in the calendar view to get.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIQ==\"",
            "subject":"Plan shopping list",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-09T20:30:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-09T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },      
            "id":"AAMkADNVxRAAA="
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIg==\"",
            "subject":"Pick up car",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T01:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-10T02:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxSAAA="
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d300d-148">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d300d-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d300d-149">C#</span><span class="sxs-lookup"><span data-stu-id="d300d-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_calendarview_delta_1-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d300d-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d300d-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_calendarview_delta_1-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d300d-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d300d-151">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_calendarview_delta_1-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="step-2-sample-second-request"></a><span data-ttu-id="d300d-152">Шаг 2. Пример второго запроса</span><span class="sxs-lookup"><span data-stu-id="d300d-152">Step 2: sample second request</span></span>

<span data-ttu-id="d300d-p111">Второй запрос указывает URL-адрес `nextLink`, полученный из предыдущего ответа. Обратите внимание, что в нем больше не требуется указывать те же параметры _startDateTime_ и _endDateTime_, что и в исходном запросе, так как маркер `skipToken` в URL-адресе `nextLink` кодирует и включает их.</span><span class="sxs-lookup"><span data-stu-id="d300d-p111">The second request specifies the `nextLink` URL returned from the previous response. Notice that it no longer has to specify the same _startDateTime_ and _endDateTime_ parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-second-response"></a><span data-ttu-id="d300d-155">Пример второго ответа</span><span class="sxs-lookup"><span data-stu-id="d300d-155">Sample second response</span></span> 

<span data-ttu-id="d300d-156">Второй ответ содержит следующие 2 события в представлении календаря и еще одну ссылку `nextLink`, указывающую, что получены не все события в представлении календаря.</span><span class="sxs-lookup"><span data-stu-id="d300d-156">The second response returns the next 2 events in the calendar view and another `nextLink`, indicating there are more events to get from the calendar view.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIw==\"",
            "subject":"Get food",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T19:30:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-10T21:30:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxTAAA="
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvJA==\"",
            "subject":"Prepare food",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-11T00:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxUAAA="
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d300d-157">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d300d-157">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d300d-158">C#</span><span class="sxs-lookup"><span data-stu-id="d300d-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_calendarview_delta_2-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d300d-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d300d-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_calendarview_delta_2-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d300d-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d300d-160">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_calendarview_delta_2-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


### <a name="step-3-sample-third-request"></a><span data-ttu-id="d300d-161">Шаг 3. Пример третьего запроса</span><span class="sxs-lookup"><span data-stu-id="d300d-161">Step 3: sample third request</span></span>

<span data-ttu-id="d300d-162">Третий запрос продолжает использовать маркер `nextLink`, полученный из последнего запроса на синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="d300d-162">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span> 
 

<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4 HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-third-and-final-response"></a><span data-ttu-id="d300d-163">Пример третьего и последнего ответа</span><span class="sxs-lookup"><span data-stu-id="d300d-163">Sample third and final response</span></span>

<span data-ttu-id="d300d-p112">Третий ответ содержат последнее оставшееся событие из представления календаря и URL-адрес `deltaLink`, указывающий, что синхронизация для этого представления календаря завершена. Сохраните URL-адрес `deltaLink` и используйте его в [следующем цикле синхронизации этого представления календаря](#the-next-round-sample-first-request).</span><span class="sxs-lookup"><span data-stu-id="d300d-p112">The third response returns the only remaining event in the calendar view, and a `deltaLink` URL which indicates synchronization is complete for this calendar view. Save and use the `deltaLink` URL to [synchronize that calendar view in the next round](#the-next-round-sample-first-request).</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAALZu97g==\"",
            "subject":"Rest!",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-12T02:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-12T07:30:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"Home"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADj1HuAAA="
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d300d-166">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d300d-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d300d-167">C#</span><span class="sxs-lookup"><span data-stu-id="d300d-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_calendarview_delta_3-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d300d-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d300d-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_calendarview_delta_3-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d300d-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d300d-169">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_calendarview_delta_3-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


### <a name="the-next-round-sample-first-request"></a><span data-ttu-id="d300d-170">Следующий цикл: пример первого запроса</span><span class="sxs-lookup"><span data-stu-id="d300d-170">The next round: sample first request</span></span>

<span data-ttu-id="d300d-p113">С помощью ссылки `deltaLink` из последнего цикла [прошлого запроса](#step-3-sample-third-request) вы сможете получить только те события, которые изменились (путем добавления, удаления или обновления) в этом представлении календаря с момента последней синхронизации. При условии, что вы не хотите менять максимальный размер страницы ответа, первый запрос следующего цикла будет выглядеть следующим образом:</span><span class="sxs-lookup"><span data-stu-id="d300d-p113">Using the `deltaLink` from the [last request](#step-3-sample-third-request) in the last round, you will be able to get only those events that have changed (by being added, deleted, or updated) in that calendar view since then. Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_next"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="the-next-round-sample-first-response"></a><span data-ttu-id="d300d-173">Следующий цикл: пример первого ответа</span><span class="sxs-lookup"><span data-stu-id="d300d-173">The next round: sample first response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcFuQtZdtpk4",
    "value":[
        {
            "@odata.type": "#microsoft.graph.event",
            "id": "AAMkADk0MGFkODE3LWE4MmYtNDRhOS04OGQLkRkXbBznTvAADb6ytyAAA=",
            "@removed": {
                "reason": "deleted"
            }
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAALZu97w==\"",
            "subject":"Attend service",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-25T06:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-25T07:30:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"Chapel of Saint Ignatius",
                "address":{
                    "street":"900 Broadway",
                    "city":"Seattle",
                    "state":"WA",
                    "countryOrRegion":"United States",
                    "postalCode":""
                },
                "coordinates":{
                    "latitude":47.6105,
                    "longitude":-122.321
                }
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADj1HvAAA="
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d300d-174">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d300d-174">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d300d-175">C#</span><span class="sxs-lookup"><span data-stu-id="d300d-175">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_calendarview_delta_next-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d300d-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d300d-176">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_calendarview_delta_next-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d300d-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d300d-177">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_calendarview_delta_next-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="d300d-178">См. также</span><span class="sxs-lookup"><span data-stu-id="d300d-178">See also</span></span>

- [<span data-ttu-id="d300d-179">Запрос изменений Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d300d-179">Microsoft Graph delta query</span></span>](delta-query-overview.md)
- [<span data-ttu-id="d300d-180">Получение добавочных изменений для сообщений</span><span class="sxs-lookup"><span data-stu-id="d300d-180">Get incremental changes to messages</span></span>](delta-query-messages.md)
- [<span data-ttu-id="d300d-181">Получение добавочных изменений для групп</span><span class="sxs-lookup"><span data-stu-id="d300d-181">Get incremental changes to groups</span></span>](delta-query-groups.md)
- [<span data-ttu-id="d300d-182">Получение добавочных изменений пользователей</span><span class="sxs-lookup"><span data-stu-id="d300d-182">Get incremental changes to users</span></span>](delta-query-users.md)
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example to synchronize events in a calendar view",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /concepts/delta-query-events.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /concepts/delta-query-events.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/delta-query-events.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /concepts/delta-query-events.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/delta-query-events.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /concepts/delta-query-events.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/delta-query-events.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /concepts/delta-query-events.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/delta-query-events.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
