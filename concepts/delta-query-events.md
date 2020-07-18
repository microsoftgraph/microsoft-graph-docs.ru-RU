---
title: 'Получение добавочных изменений для событий в представлении календаря '
description: 'Представление календаря — это коллекция событий в диапазоне дат и времени из календаря по умолчанию (../me/calendarview) '
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 5b5e41a689a62157bb686ca6bb97ef63af9ac02a
ms.sourcegitcommit: b469176f49aacbd02cd06838cc7c8d36cf5bc768
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2020
ms.locfileid: "45165046"
---
# <a name="get-incremental-changes-to-events-in-a-calendar-view"></a><span data-ttu-id="b13e3-103">Получение добавочных изменений для событий в представлении календаря</span><span class="sxs-lookup"><span data-stu-id="b13e3-103">Get incremental changes to events in a calendar view</span></span> 

<span data-ttu-id="b13e3-104">С помощью разностного запроса можно получить новые, обновленные или удаленные события в указанном календаре(-ях) или в заданном наборе событий (например, в виде представления календаря) в календаре.</span><span class="sxs-lookup"><span data-stu-id="b13e3-104">By using delta query, you can get new, updated, or deleted events in a specified calendar(s), or within a defined collection of events (as a calendar view) in the calendar.</span></span> <span data-ttu-id="b13e3-105">В этой статье описывается последний случай: получение добавочных изменений для событий в представлении календаря.</span><span class="sxs-lookup"><span data-stu-id="b13e3-105">This article describes the latter - getting such incremental changes to events in a calendar view.</span></span> 

> <span data-ttu-id="b13e3-106">**Примечание** Возможность получения добавочных изменений для событий календаря, не привязанного к диапазону с фиксированными начальными и конечными датами, относящаяся к первому случаю, в настоящий момент доступна только в бета-версии.</span><span class="sxs-lookup"><span data-stu-id="b13e3-106">**Note** The capability for the former - getting incremental changes to events in a calendar not bound to a fixed start and end date range - is currently available only in the beta version.</span></span> <span data-ttu-id="b13e3-107">Дополнительные сведения см. в статье функция [delta](/graph/api/event-delta?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="b13e3-107">For more information, see [delta](/graph/api/event-delta?view=graph-rest-beta) function.</span></span>

<span data-ttu-id="b13e3-108">Представление календаря — это коллекция событий в диапазоне дат и времени (../me/calendarview) из календаря по умолчанию или другого указанного календаря пользователя, или календаря группы.</span><span class="sxs-lookup"><span data-stu-id="b13e3-108">A calendar view is a collection of events in a date/time range (../me/calendarview) from the default calendar or some other specified calendar of a user, or from a group calendar.</span></span> <span data-ttu-id="b13e3-109">Возвращаемые события могут включать отдельные экземпляры, а также повторения и исключения из повторяющейся серии.</span><span class="sxs-lookup"><span data-stu-id="b13e3-109">The returned events may include single instances, or occurrences and exceptions of a recurring series.</span></span> <span data-ttu-id="b13e3-110">Разностные данные позволяют поддерживать и синхронизировать локальное хранилище событий пользователя. При этом вам не требуется каждый раз получать весь набор событий пользователя с сервера.</span><span class="sxs-lookup"><span data-stu-id="b13e3-110">The delta data enables you to maintain and synchronize a local store of a user's events, without having to fetch the entire set of the user's events from the server every time.</span></span>

<span data-ttu-id="b13e3-p104">Запрос изменений поддерживает как полную синхронизацию с получением всех событий в определенном представлении календаря, так и добавочную синхронизацию с получением тех событий, которые изменились в представлении календаря с момента последней синхронизации. Как правило, сначала выполняется полная синхронизация, а затем в представление календаря периодически добавляются изменения.</span><span class="sxs-lookup"><span data-stu-id="b13e3-p104">Delta query supports both full synchronization that retrieves all the events in the specified calendar view, and incremental synchronization that retrieves those events that have changed in the calendar view since the last synchronization. Typically, you would do an initial full synchronization, and subsequently, get incremental changes to that calendar view periodically.</span></span> 

## <a name="track-event-changes-in-a-calendar-view"></a><span data-ttu-id="b13e3-113">Отслеживание изменений событий в представлении календаря</span><span class="sxs-lookup"><span data-stu-id="b13e3-113">Track event changes in a calendar view</span></span>

<span data-ttu-id="b13e3-114">Запрос изменений в представлении календаря для событий относится к указанным календарю и диапазону дат и времени.</span><span class="sxs-lookup"><span data-stu-id="b13e3-114">Delta query for events in a calendar view is specific to a calendar and date/time range that you specify.</span></span> <span data-ttu-id="b13e3-115">Чтобы отслеживать изменения в нескольких календарях, необходимо наблюдать за каждым календарем отдельно.</span><span class="sxs-lookup"><span data-stu-id="b13e3-115">To track the changes in multiple calendars, you need to track each calendar individually.</span></span> 

<span data-ttu-id="b13e3-116">Как правило, цикл отслеживания изменений событий в представлении календаря состоит из одного или нескольких запросов GET с функцией [delta](/graph/api/event-delta?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="b13e3-116">Tracking event changes in a calendar view typically is a round of one or more GET requests with the [delta](/graph/api/event-delta?view=graph-rest-1.0) function.</span></span> <span data-ttu-id="b13e3-117">Исходный запрос GET во многом аналогичен [получению списка calendarView](/graph/api/calendar-list-calendarview?view=graph-rest-1.0), но он также содержит функцию **delta**.</span><span class="sxs-lookup"><span data-stu-id="b13e3-117">The initial GET request is very much like the way you [list a calendarView](/graph/api/calendar-list-calendarview?view=graph-rest-1.0), except that you include the **delta** function.</span></span> <span data-ttu-id="b13e3-118">Ниже приведен исходный запрос GET delta для представления календаря в календаре, используемом по умолчанию пользователем, который вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="b13e3-118">The following is the initial GET delta request of a calendar view in the signed-in user's default calendar:</span></span>

```
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="b13e3-119">Запрос GET с функцией **delta** возвращает одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="b13e3-119">A GET request with the **delta** function returns either:</span></span>

- <span data-ttu-id="b13e3-120">ссылку `nextLink` (содержащую URL-адрес с вызовом функции **delta** и маркером _skipToken_);</span><span class="sxs-lookup"><span data-stu-id="b13e3-120">A `nextLink` (that contains a URL with a **delta** function call and a _skipToken_), or</span></span> 
- <span data-ttu-id="b13e3-121">ссылку `deltaLink` (содержащую URL-адрес с вызовом функции **delta** и маркером _deltaToken_).</span><span class="sxs-lookup"><span data-stu-id="b13e3-121">A `deltaLink` (that contains a URL with a **delta** function call and _deltaToken_).</span></span>

<span data-ttu-id="b13e3-122">Эти маркеры являются [маркерами состояния](delta-query-overview.md#state-tokens), кодирующими параметры _startDateTime_ и _endDateTime_, а также любой другой параметр в исходном разностном запросе GET.</span><span class="sxs-lookup"><span data-stu-id="b13e3-122">These tokens are [state tokens](delta-query-overview.md#state-tokens) which encode the _startDateTime_ and _endDateTime_ parameters, and any other query parameter in your initial delta query GET request.</span></span> <span data-ttu-id="b13e3-123">Эти параметры не нужно включать в последующих запросах, поскольку они закодированы в маркерах.</span><span class="sxs-lookup"><span data-stu-id="b13e3-123">You do not need to include these parameters in subsequent requests as they are encoded in the tokens.</span></span>

<span data-ttu-id="b13e3-p108">Маркеры состояния полностью непрозрачны для клиента. Чтобы продолжить цикл отслеживания изменений, просто скопируйте и примените URL-адрес `nextLink` или `deltaLink`, возвращенный последним запросом GET, при следующем вызове функции **delta** для этого представления календаря. Ссылка `deltaLink` в ответе означает, что текущий цикл отслеживания изменений завершен. Вы можете сохранить и использовать URL-адрес `deltaLink` в начале следующего цикла.</span><span class="sxs-lookup"><span data-stu-id="b13e3-p108">State tokens are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next **delta** function call for that same calendar view. A `deltaLink` returned in a response signifies that the current round of change tracking is complete. You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="b13e3-128">В приведенном ниже [примере](#example-to-synchronize-events-in-a-calendar-view) показано, как использовать URL-адреса `nextLink` и `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="b13e3-128">See the [example](#example-to-synchronize-events-in-a-calendar-view) below to learn how to use these `nextLink` and `deltaLink` URLs.</span></span>

### <a name="use-query-parameters-in-a-delta-query-for-calendar-view"></a><span data-ttu-id="b13e3-129">Использование параметров запроса изменений для представления календаря</span><span class="sxs-lookup"><span data-stu-id="b13e3-129">Use query parameters in a delta query for calendar view</span></span>

- <span data-ttu-id="b13e3-130">Укажите параметры _startDateTime_ и _endDateTime_, чтобы определить диапазон дат и времени для представления календаря.</span><span class="sxs-lookup"><span data-stu-id="b13e3-130">Include the _startDateTime_ and _endDateTime_ parameters to define a date/time range for your calendar view.</span></span>
- <span data-ttu-id="b13e3-131">Параметр `$select` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b13e3-131">`$select` is not supported.</span></span>


### <a name="optional-request-header"></a><span data-ttu-id="b13e3-132">Необязательный заголовок запроса</span><span class="sxs-lookup"><span data-stu-id="b13e3-132">Optional request header</span></span>

<span data-ttu-id="b13e3-133">Каждый разностный запрос GET возвращает коллекцию из одного или нескольких событий в отклике.</span><span class="sxs-lookup"><span data-stu-id="b13e3-133">Each delta query GET request returns a collection of one or more events in the response.</span></span> <span data-ttu-id="b13e3-134">При необходимости вы можете указать заголовок запроса `Prefer: odata.maxpagesize={x}`, чтобы задать максимальное количество событий в отклике.</span><span class="sxs-lookup"><span data-stu-id="b13e3-134">You can optionally specify the request header, `Prefer: odata.maxpagesize={x}`, to set the maximum number of events in a response.</span></span>


## <a name="example-to-synchronize-events-in-a-calendar-view"></a><span data-ttu-id="b13e3-135">Пример синхронизации событий в представлении календаря</span><span class="sxs-lookup"><span data-stu-id="b13e3-135">Example to synchronize events in a calendar view</span></span>

<span data-ttu-id="b13e3-p110">В приведенном ниже примере показана серия из 3 запросов, синхронизирующих календарь пользователя по умолчанию в определенном диапазоне времени. Это представление календаря содержит 5 событий.</span><span class="sxs-lookup"><span data-stu-id="b13e3-p110">The following example shows a series of 3 requests to synchronize the user's default calendar in a specific time range. There are 5 events in that calendar view.</span></span>

- <span data-ttu-id="b13e3-138">[Шаг 1. Пример исходного запроса](#step-1-sample-initial-request) и [ответ](#sample-initial-response)</span><span class="sxs-lookup"><span data-stu-id="b13e3-138">[Step 1: sample initial request](#step-1-sample-initial-request) and [response](#sample-initial-response)</span></span>
- <span data-ttu-id="b13e3-139">[Шаг 2. Пример второго запроса](#step-2-sample-second-request) и [ответ](#sample-second-response)</span><span class="sxs-lookup"><span data-stu-id="b13e3-139">[Step 2: sample second request](#step-2-sample-second-request) and [response](#sample-second-response)</span></span>
- <span data-ttu-id="b13e3-140">[Шаг 3. Пример третьего запроса](#step-3-sample-third-request) и [последний ответ](#sample-third-and-final-response)</span><span class="sxs-lookup"><span data-stu-id="b13e3-140">[Step 3: sample third request](#step-3-sample-third-request) and [final response](#sample-third-and-final-response)</span></span>

<span data-ttu-id="b13e3-p111">В примерах показаны только некоторые свойства события. При фактическом вызове возвращается большинство свойств события.</span><span class="sxs-lookup"><span data-stu-id="b13e3-p111">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span> 

<span data-ttu-id="b13e3-143">См. также, что можно сделать в [следующем цикле](#the-next-round-sample-first-response).</span><span class="sxs-lookup"><span data-stu-id="b13e3-143">See also what you'll do in the [next round](#the-next-round-sample-first-response).</span></span>


### <a name="step-1-sample-initial-request"></a><span data-ttu-id="b13e3-144">Шаг 1. Пример исходного запроса</span><span class="sxs-lookup"><span data-stu-id="b13e3-144">Step 1: sample initial request</span></span>

<span data-ttu-id="b13e3-145">В этом примере указанное представление календаря для календаря, используемого по умолчанию пользователем, который вошел в систему, синхронизируется впервые, поэтому исходный запрос на синхронизацию не содержит маркер состояния.</span><span class="sxs-lookup"><span data-stu-id="b13e3-145">In this example, the specified calendar view in the signed-in user's default calendar is being synchronized for the first time, so the initial sync request does not include any state token.</span></span> <span data-ttu-id="b13e3-146">В этом цикле возвращаются все события в представлении календаря.</span><span class="sxs-lookup"><span data-stu-id="b13e3-146">This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="b13e3-147">Первый запрос задает следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="b13e3-147">The first request specifies the following:</span></span>

- <span data-ttu-id="b13e3-148">значения даты и времени для параметров _startDateTime_ и _endDateTime_;</span><span class="sxs-lookup"><span data-stu-id="b13e3-148">Date/time values for the _startDateTime_ and _endDateTime_ parameters.</span></span>
- <span data-ttu-id="b13e3-149">[необязательный заголовок запроса](#optional-request-header) _odata.maxpagesize_, возвращающий 2 события одновременно.</span><span class="sxs-lookup"><span data-stu-id="b13e3-149">The [optional request header](#optional-request-header), _odata.maxpagesize_, returning 2 events at a time.</span></span>


# <a name="http"></a>[<span data-ttu-id="b13e3-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="b13e3-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime=2016-12-01T00:00:00Z&enddatetime=2016-12-30T00:00:00Z HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="b13e3-151">C#</span><span class="sxs-lookup"><span data-stu-id="b13e3-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b13e3-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b13e3-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b13e3-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b13e3-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b13e3-154">Java</span><span class="sxs-lookup"><span data-stu-id="b13e3-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="sample-initial-response"></a><span data-ttu-id="b13e3-155">Пример исходного ответа</span><span class="sxs-lookup"><span data-stu-id="b13e3-155">Sample initial response</span></span>

<span data-ttu-id="b13e3-p113">Ответ включает два события и заголовок ответа `@odata.nextLink` с маркером `skipToken`. URL-адрес `nextLink` указывает, что получены не все события в представлении календаря.</span><span class="sxs-lookup"><span data-stu-id="b13e3-p113">The response includes two events and a `@odata.nextLink` response header with a `skipToken`. The `nextLink` URL indicates there are more events in the calendar view to get.</span></span>

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

### <a name="step-2-sample-second-request"></a><span data-ttu-id="b13e3-158">Шаг 2. Пример второго запроса</span><span class="sxs-lookup"><span data-stu-id="b13e3-158">Step 2: sample second request</span></span>

<span data-ttu-id="b13e3-p114">Второй запрос указывает URL-адрес `nextLink`, полученный из предыдущего ответа. Обратите внимание, что в нем больше не требуется указывать те же параметры _startDateTime_ и _endDateTime_, что и в исходном запросе, так как маркер `skipToken` в URL-адресе `nextLink` кодирует и включает их.</span><span class="sxs-lookup"><span data-stu-id="b13e3-p114">The second request specifies the `nextLink` URL returned from the previous response. Notice that it no longer has to specify the same _startDateTime_ and _endDateTime_ parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>


# <a name="http"></a>[<span data-ttu-id="b13e3-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="b13e3-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="b13e3-162">C#</span><span class="sxs-lookup"><span data-stu-id="b13e3-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b13e3-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b13e3-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b13e3-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b13e3-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b13e3-165">Java</span><span class="sxs-lookup"><span data-stu-id="b13e3-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="sample-second-response"></a><span data-ttu-id="b13e3-166">Пример второго ответа</span><span class="sxs-lookup"><span data-stu-id="b13e3-166">Sample second response</span></span> 

<span data-ttu-id="b13e3-167">Второй ответ содержит следующие 2 события в представлении календаря и еще одну ссылку `nextLink`, указывающую, что получены не все события в представлении календаря.</span><span class="sxs-lookup"><span data-stu-id="b13e3-167">The second response returns the next 2 events in the calendar view and another `nextLink`, indicating there are more events to get from the calendar view.</span></span>

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


### <a name="step-3-sample-third-request"></a><span data-ttu-id="b13e3-168">Шаг 3. Пример третьего запроса</span><span class="sxs-lookup"><span data-stu-id="b13e3-168">Step 3: sample third request</span></span>

<span data-ttu-id="b13e3-169">Третий запрос продолжает использовать маркер `nextLink`, полученный из последнего запроса на синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="b13e3-169">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span> 
 


# <a name="http"></a>[<span data-ttu-id="b13e3-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="b13e3-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4 HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="b13e3-171">C#</span><span class="sxs-lookup"><span data-stu-id="b13e3-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b13e3-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b13e3-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b13e3-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b13e3-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b13e3-174">Java</span><span class="sxs-lookup"><span data-stu-id="b13e3-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="sample-third-and-final-response"></a><span data-ttu-id="b13e3-175">Пример третьего и последнего ответа</span><span class="sxs-lookup"><span data-stu-id="b13e3-175">Sample third and final response</span></span>

<span data-ttu-id="b13e3-p115">Третий ответ содержат последнее оставшееся событие из представления календаря и URL-адрес `deltaLink`, указывающий, что синхронизация для этого представления календаря завершена. Сохраните URL-адрес `deltaLink` и используйте его в [следующем цикле синхронизации этого представления календаря](#the-next-round-sample-first-request).</span><span class="sxs-lookup"><span data-stu-id="b13e3-p115">The third response returns the only remaining event in the calendar view, and a `deltaLink` URL which indicates synchronization is complete for this calendar view. Save and use the `deltaLink` URL to [synchronize that calendar view in the next round](#the-next-round-sample-first-request).</span></span>


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


### <a name="the-next-round-sample-first-request"></a><span data-ttu-id="b13e3-178">Следующий цикл: пример первого запроса</span><span class="sxs-lookup"><span data-stu-id="b13e3-178">The next round: sample first request</span></span>

<span data-ttu-id="b13e3-p116">С помощью ссылки `deltaLink` из последнего цикла [прошлого запроса](#step-3-sample-third-request) вы сможете получить только те события, которые изменились (путем добавления, удаления или обновления) в этом представлении календаря с момента последней синхронизации. При условии, что вы не хотите менять максимальный размер страницы ответа, первый запрос следующего цикла будет выглядеть следующим образом:</span><span class="sxs-lookup"><span data-stu-id="b13e3-p116">Using the `deltaLink` from the [last request](#step-3-sample-third-request) in the last round, you will be able to get only those events that have changed (by being added, deleted, or updated) in that calendar view since then. Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>


# <a name="http"></a>[<span data-ttu-id="b13e3-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="b13e3-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_next"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="b13e3-182">C#</span><span class="sxs-lookup"><span data-stu-id="b13e3-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-next-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b13e3-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b13e3-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-next-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b13e3-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b13e3-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-next-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b13e3-185">Java</span><span class="sxs-lookup"><span data-stu-id="b13e3-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-next-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="the-next-round-sample-first-response"></a><span data-ttu-id="b13e3-186">Следующий цикл: пример первого ответа</span><span class="sxs-lookup"><span data-stu-id="b13e3-186">The next round: sample first response</span></span>

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

## <a name="see-also"></a><span data-ttu-id="b13e3-187">См. также</span><span class="sxs-lookup"><span data-stu-id="b13e3-187">See also</span></span>

- [<span data-ttu-id="b13e3-188">Запрос изменений Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b13e3-188">Microsoft Graph delta query</span></span>](delta-query-overview.md)
- [<span data-ttu-id="b13e3-189">Получение добавочных изменений для сообщений</span><span class="sxs-lookup"><span data-stu-id="b13e3-189">Get incremental changes to messages</span></span>](delta-query-messages.md)
- [<span data-ttu-id="b13e3-190">Получение добавочных изменений для групп</span><span class="sxs-lookup"><span data-stu-id="b13e3-190">Get incremental changes to groups</span></span>](delta-query-groups.md)
- [<span data-ttu-id="b13e3-191">Получение добавочных изменений пользователей</span><span class="sxs-lookup"><span data-stu-id="b13e3-191">Get incremental changes to users</span></span>](delta-query-users.md)
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example to synchronize events in a calendar view",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
