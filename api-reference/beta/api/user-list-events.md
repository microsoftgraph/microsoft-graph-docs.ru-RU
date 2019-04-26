---
title: Перечисление событий
description: 'Получение списка объектов event из стандартного календаря пользователя или '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ef16f9f0db1bc1e489bc7322ff72f58598d8d0a6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547860"
---
# <a name="list-events"></a><span data-ttu-id="0778b-103">Перечисление событий</span><span class="sxs-lookup"><span data-stu-id="0778b-103">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0778b-104">Получение списка объектов [event](../resources/event.md) из стандартного календаря пользователя или указанного календаря.</span><span class="sxs-lookup"><span data-stu-id="0778b-104">Get a list of [event](../resources/event.md) objects from the user's default calendar or from a specified calendar.</span></span> <span data-ttu-id="0778b-105">В этом списке указаны единичные собрания и главные собрания в соответствующих рядах.</span><span class="sxs-lookup"><span data-stu-id="0778b-105">The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="0778b-106">Чтобы получить расширенные экземпляры события, вы можете [получить представление календаря](calendar-list-calendarview.md) или [экземпляры события](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="0778b-106">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

<span data-ttu-id="0778b-107">Существует два сценария, в которых приложение может получить события из календаря другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="0778b-107">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="0778b-108">если у приложения есть разрешения для приложений;</span><span class="sxs-lookup"><span data-stu-id="0778b-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="0778b-109">если у приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним календарем или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="0778b-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="0778b-110">См. [подробные сведения и пример](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="0778b-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="0778b-111">Поддержка разных часовых поясов</span><span class="sxs-lookup"><span data-stu-id="0778b-111">Support various time zones</span></span>

<span data-ttu-id="0778b-112">Для всех операций GET, которые возвращают события, можно использовать заголовок `Prefer: outlook.timezone`, чтобы задать часовой пояс для указанного в отклике времени начала и завершения события.</span><span class="sxs-lookup"><span data-stu-id="0778b-112">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="0778b-113">Например, заголовок `Prefer: outlook.timezone` задает в отклике время начала и завершения согласно североамериканскому восточному времени.</span><span class="sxs-lookup"><span data-stu-id="0778b-113">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="0778b-p103">Если событие создано с применением другого часового пояса, время начала и завершения будет изменено в соответствии с часовым поясом, указанным в заголовке `Prefer`. Поддерживаемые часовые пояса указаны в этом [списке](../resources/datetimetimezone.md). Если заголовок `Prefer: outlook.timezone` не указан, время начала и завершения возвращается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0778b-p103">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="0778b-117">Узнать, какой именно часовой пояс использовался при создании события, позволят свойства **OriginalStartTimeZone** и **OriginalEndTimeZone** ресурса **event**.</span><span class="sxs-lookup"><span data-stu-id="0778b-117">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="0778b-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0778b-118">Permissions</span></span>
<span data-ttu-id="0778b-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0778b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0778b-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0778b-121">Permission type</span></span>      | <span data-ttu-id="0778b-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0778b-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0778b-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0778b-123">Delegated (work or school account)</span></span> | <span data-ttu-id="0778b-124">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0778b-124">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0778b-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0778b-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0778b-126">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0778b-126">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0778b-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0778b-127">Application</span></span> | <span data-ttu-id="0778b-128">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0778b-128">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0778b-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0778b-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events
GET /users/{id | userPrincipalName}/events

GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events

GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendargroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events

GET /me/calendargroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0778b-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0778b-130">Optional query parameters</span></span>
<span data-ttu-id="0778b-131">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0778b-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0778b-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0778b-132">Request headers</span></span>
| <span data-ttu-id="0778b-133">Имя</span><span class="sxs-lookup"><span data-stu-id="0778b-133">Name</span></span>       | <span data-ttu-id="0778b-134">Тип</span><span class="sxs-lookup"><span data-stu-id="0778b-134">Type</span></span> | <span data-ttu-id="0778b-135">Описание</span><span class="sxs-lookup"><span data-stu-id="0778b-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0778b-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="0778b-136">Authorization</span></span>  | <span data-ttu-id="0778b-137">string</span><span class="sxs-lookup"><span data-stu-id="0778b-137">string</span></span>  | <span data-ttu-id="0778b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0778b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0778b-140">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="0778b-140">Prefer: outlook.timezone</span></span> | <span data-ttu-id="0778b-141">string</span><span class="sxs-lookup"><span data-stu-id="0778b-141">string</span></span> | <span data-ttu-id="0778b-142">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="0778b-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="0778b-143">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0778b-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="0778b-144">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="0778b-144">Optional.</span></span> |
| <span data-ttu-id="0778b-145">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="0778b-145">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="0778b-146">string</span><span class="sxs-lookup"><span data-stu-id="0778b-146">string</span></span> | <span data-ttu-id="0778b-147">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="0778b-147">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="0778b-148">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="0778b-148">Values can be "text" or "html".</span></span> <span data-ttu-id="0778b-149">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="0778b-149">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="0778b-150">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="0778b-150">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="0778b-151">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="0778b-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0778b-152">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0778b-152">Request body</span></span>
<span data-ttu-id="0778b-153">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0778b-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0778b-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="0778b-154">Response</span></span>

<span data-ttu-id="0778b-155">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0778b-155">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0778b-156">Пример</span><span class="sxs-lookup"><span data-stu-id="0778b-156">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="0778b-157">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="0778b-157">Request 1</span></span>
<span data-ttu-id="0778b-158">В первом примере возвращаются все события пользователя.</span><span class="sxs-lookup"><span data-stu-id="0778b-158">The first example gets all the user's events.</span></span> <span data-ttu-id="0778b-159">В нем указывается:</span><span class="sxs-lookup"><span data-stu-id="0778b-159">It specifies the following:</span></span>

- <span data-ttu-id="0778b-160">Заголовок `Prefer: outlook.timezone` для получения значений даты и времени, которые возвращаются для стандартного тихоокеанского времени.</span><span class="sxs-lookup"><span data-stu-id="0778b-160">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="0778b-p109">Параметр запроса `$select`, который возвращает конкретные свойства. Без параметра `$select` будут возвращены все свойства событий.</span><span class="sxs-lookup"><span data-stu-id="0778b-p109">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="0778b-163">В запросе не определен никакой заголовок `Prefer: outlook.body-content-type`, чтобы указать конкретный формат для текста возвращаемого события.</span><span class="sxs-lookup"><span data-stu-id="0778b-163">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response-1"></a><span data-ttu-id="0778b-164">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="0778b-164">Response 1</span></span>
<span data-ttu-id="0778b-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0778b-165">Here is an example of the response.</span></span> <span data-ttu-id="0778b-166">Так как заголовок `Prefer: outlook.body-content-type` не указан, свойство **body** возвращается в формате HTML по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0778b-166">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="0778b-167">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="0778b-167">Request 2</span></span>
<span data-ttu-id="0778b-168">Во втором примере показано, как использовать заголовок `Prefer: outlook.body-content-type="text"`, чтобы получить свойство **body** указанного сообщения в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="0778b-168">The second example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified message in text format.</span></span>

<span data-ttu-id="0778b-169">В запросе также используется параметр `$select` для возврата отдельных свойств.</span><span class="sxs-lookup"><span data-stu-id="0778b-169">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="0778b-170">Без параметра `$select` будут возвращены все свойства событий.</span><span class="sxs-lookup"><span data-stu-id="0778b-170">Without a `$select` parameter, all of the event properties will be returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/events?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text" 
```
##### <a name="response-2"></a><span data-ttu-id="0778b-171">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="0778b-171">Response 2</span></span>
<span data-ttu-id="0778b-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0778b-172">Here is an example of the response.</span></span> <span data-ttu-id="0778b-173">Свойство **body** возвращается в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="0778b-173">The **body** property is returned in text format.</span></span> 

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
    "Error: /api-reference/beta/api/user-list-events.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
