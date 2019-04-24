---
title: Получение события
description: Получение свойств и отношений указанного объекта event.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 49a4e16e6f24ebac22c760cf11e63c220181d0b9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457487"
---
# <a name="get-event"></a><span data-ttu-id="ea0e5-103">Получение события</span><span class="sxs-lookup"><span data-stu-id="ea0e5-103">Get event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea0e5-104">Получение свойств и отношений указанного объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="ea0e5-104">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="ea0e5-105">Существует два сценария, в которых приложение может получить событие в календаре другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="ea0e5-105">There are two scenarios where an app can get an event in another user's calendar:</span></span>

* <span data-ttu-id="ea0e5-106">если у приложения есть разрешения для приложений;</span><span class="sxs-lookup"><span data-stu-id="ea0e5-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="ea0e5-107">если у приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним календарем или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="ea0e5-108">См. [подробные сведения и пример](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="ea0e5-108">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

<span data-ttu-id="ea0e5-109">Так как ресурс **event** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` вы можете получить настраиваемые свойства и данные расширения в экземпляре **события**.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-109">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="ea0e5-110">Поддержка разных часовых поясов</span><span class="sxs-lookup"><span data-stu-id="ea0e5-110">Support various time zones</span></span>

<span data-ttu-id="ea0e5-111">Для всех операций GET, которые возвращают события, можно использовать заголовок `Prefer: outlook.timezone`, чтобы задать часовой пояс для указанного в отклике времени начала и завершения события.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-111">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="ea0e5-112">Например, заголовок `Prefer: outlook.timezone` задает в отклике время начала и завершения согласно североамериканскому восточному времени.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-112">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="ea0e5-p102">Если событие создано с применением другого часового пояса, время начала и завершения будет изменено в соответствии с часовым поясом, указанным в заголовке `Prefer`. Поддерживаемые часовые пояса указаны в этом [списке](../resources/datetimetimezone.md). Если заголовок `Prefer: outlook.timezone` не указан, время начала и завершения возвращается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="ea0e5-116">Узнать, какой именно часовой пояс использовался при создании события, позволят свойства **OriginalStartTimeZone** и **OriginalEndTimeZone** ресурса **event**.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-116">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea0e5-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea0e5-117">Permissions</span></span>
<span data-ttu-id="ea0e5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea0e5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea0e5-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea0e5-120">Permission type</span></span>      | <span data-ttu-id="ea0e5-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea0e5-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea0e5-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea0e5-122">Delegated (work or school account)</span></span> | <span data-ttu-id="ea0e5-123">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ea0e5-123">Calendars.Read</span></span>    |
|<span data-ttu-id="ea0e5-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea0e5-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea0e5-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ea0e5-125">Calendars.Read</span></span>    |
|<span data-ttu-id="ea0e5-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea0e5-126">Application</span></span> | <span data-ttu-id="ea0e5-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ea0e5-127">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea0e5-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea0e5-128">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="ea0e5-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ea0e5-129">Optional query parameters</span></span>
<span data-ttu-id="ea0e5-130">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ea0e5-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea0e5-131">Request headers</span></span>
| <span data-ttu-id="ea0e5-132">Имя</span><span class="sxs-lookup"><span data-stu-id="ea0e5-132">Name</span></span>       | <span data-ttu-id="ea0e5-133">Тип</span><span class="sxs-lookup"><span data-stu-id="ea0e5-133">Type</span></span> | <span data-ttu-id="ea0e5-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ea0e5-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ea0e5-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea0e5-135">Authorization</span></span>  | <span data-ttu-id="ea0e5-136">string</span><span class="sxs-lookup"><span data-stu-id="ea0e5-136">string</span></span>  | <span data-ttu-id="ea0e5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ea0e5-139">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="ea0e5-139">Prefer: outlook.timezone</span></span> | <span data-ttu-id="ea0e5-140">string</span><span class="sxs-lookup"><span data-stu-id="ea0e5-140">string</span></span> | <span data-ttu-id="ea0e5-141">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-141">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="ea0e5-142">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-142">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="ea0e5-143">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-143">Optional.</span></span> |
| <span data-ttu-id="ea0e5-144">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="ea0e5-144">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="ea0e5-145">string</span><span class="sxs-lookup"><span data-stu-id="ea0e5-145">string</span></span> | <span data-ttu-id="ea0e5-146">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-146">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="ea0e5-147">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="ea0e5-147">Values can be "text" or "html".</span></span> <span data-ttu-id="ea0e5-148">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-148">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="ea0e5-149">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-149">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="ea0e5-150">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-150">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea0e5-151">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea0e5-151">Request body</span></span>
<span data-ttu-id="ea0e5-152">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea0e5-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea0e5-153">Response</span></span>

<span data-ttu-id="ea0e5-154">В случае успеха этот метод возвратит код отклика `200 OK` и объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-154">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ea0e5-155">Пример</span><span class="sxs-lookup"><span data-stu-id="ea0e5-155">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="ea0e5-156">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="ea0e5-156">Request 1</span></span>
<span data-ttu-id="ea0e5-p107">Первый пример возвращает указанное событие. Он указывает следующее:</span><span class="sxs-lookup"><span data-stu-id="ea0e5-p107">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="ea0e5-159">Заголовок `Prefer: outlook.timezone` для получения значений даты и времени, которые возвращаются для стандартного тихоокеанского времени.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-159">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="ea0e5-p108">Параметр запроса `$select`, который возвращает конкретные свойства. Без параметра `$select` будут возвращены все свойства событий.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-p108">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="ea0e5-162">В запросе не определен никакой заголовок `Prefer: outlook.body-content-type`, чтобы указать конкретный формат для текста возвращаемого события.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-162">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_event"
}-->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGIAAAoZDOFAAA=')?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response-1"></a><span data-ttu-id="ea0e5-163">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="ea0e5-163">Response 1</span></span>
<span data-ttu-id="ea0e5-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-164">Here is an example of the response.</span></span> <span data-ttu-id="ea0e5-165">Так как заголовок `Prefer: outlook.body-content-type` не указан, свойство **body** возвращается в формате HTML по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-165">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span> 

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
```

##### <a name="request-2"></a><span data-ttu-id="ea0e5-166">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="ea0e5-166">Request 2</span></span>
<span data-ttu-id="ea0e5-167">Во втором примере показано, как использовать `Prefer: outlook.body-content-type="text"` заголовок для получения свойства **Body** указанного события в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-167">The second example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified event in text format.</span></span>

<span data-ttu-id="ea0e5-168">В запросе также используется параметр `$select` для возврата отдельных свойств.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-168">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="ea0e5-169">Без параметра `$select` будут возвращены все свойства событий.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-169">Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_event_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGI1AAAoZDOFAAA=')?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text"
```
##### <a name="response-2"></a><span data-ttu-id="ea0e5-170">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="ea0e5-170">Response 2</span></span>
<span data-ttu-id="ea0e5-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-171">Here is an example of the response.</span></span> <span data-ttu-id="ea0e5-172">Свойство **body** возвращается в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-172">The **body** property is returned in text format.</span></span> 

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


##### <a name="request-3"></a><span data-ttu-id="ea0e5-173">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="ea0e5-173">Request 3</span></span>

<span data-ttu-id="ea0e5-174">В третьем примере показано, как получается событие, задающее несколько расположений.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-174">The third example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="ea0e5-175">В запросе указан параметр `$select` для возврата отдельных свойств.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-175">The request specifies a `$select` query parameter to return specific properties.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_event_multiple_locations"
}-->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkADAGAADDdm4NAAA=')?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
##### <a name="response-3"></a><span data-ttu-id="ea0e5-176">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="ea0e5-176">Response 3</span></span>
<span data-ttu-id="ea0e5-177">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-177">Here is an example of the response.</span></span> <span data-ttu-id="ea0e5-178">Свойство **locations** включает информацию о трех местах, для которых организовано событие.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-178">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="ea0e5-179">Так как в запросе не указано ни `Prefer: outlook.timezone` одного `Prefer: outlook.body-content-type` заголовка или заголовка, свойства **Start** и **End** отображаются в ЧАСОВОМ поясе по умолчанию в формате UTC, а текст по умолчанию — в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="ea0e5-179">Because the request does not specify any `Prefer: outlook.timezone` or `Prefer: outlook.body-content-type` header, the **start** and **end** properties are displayed in the default UTC time zone, and the body is in the default HTML format.</span></span>  

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

## <a name="see-also"></a><span data-ttu-id="ea0e5-180">См. также</span><span class="sxs-lookup"><span data-stu-id="ea0e5-180">See also</span></span>

- [<span data-ttu-id="ea0e5-181">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="ea0e5-181">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ea0e5-182">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="ea0e5-182">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="ea0e5-183">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="ea0e5-183">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/event-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
