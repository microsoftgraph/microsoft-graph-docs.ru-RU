---
title: Вывод события
description: Получение свойств и отношений указанного объекта event.
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e3cfbeba9940c6c7fe69aeb271ff7847dce7749b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448314"
---
# <a name="get-event"></a><span data-ttu-id="f5b87-103">Вывод события</span><span class="sxs-lookup"><span data-stu-id="f5b87-103">Get event</span></span>

<span data-ttu-id="f5b87-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5b87-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f5b87-105">Получение свойств и отношений указанного объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="f5b87-105">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="f5b87-106">В настоящее время эта операция возвращает текст события только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="f5b87-106">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="f5b87-107">Существует два сценария, в которых приложение может получить событие из календаря другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="f5b87-107">There are two scenarios where an app can get an event in another user's calendar:</span></span>

* <span data-ttu-id="f5b87-108">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="f5b87-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="f5b87-109">если у приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним календарем или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="f5b87-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="f5b87-110">См. [подробные сведения и пример](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="f5b87-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

<span data-ttu-id="f5b87-111">Так как ресурс **event** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` вы можете получить настраиваемые свойства и данные расширения в экземпляре **события**.</span><span class="sxs-lookup"><span data-stu-id="f5b87-111">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="f5b87-112">Поддержка разных часовых поясов</span><span class="sxs-lookup"><span data-stu-id="f5b87-112">Support various time zones</span></span>

<span data-ttu-id="f5b87-113">Для всех операций GET, которые возвращают события, можно использовать заголовок `Prefer: outlook.timezone`, чтобы задать часовой пояс для указанного в отклике времени начала и завершения события.</span><span class="sxs-lookup"><span data-stu-id="f5b87-113">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="f5b87-114">Например, заголовок `Prefer: outlook.timezone` задает в отклике время начала и завершения согласно североамериканскому восточному времени.</span><span class="sxs-lookup"><span data-stu-id="f5b87-114">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="f5b87-p102">Если событие создано с применением другого часового пояса, время начала и завершения будет изменено в соответствии с часовым поясом, указанным в заголовке `Prefer`. Поддерживаемые часовые пояса указаны в этом [списке](../resources/datetimetimezone.md). Если заголовок `Prefer: outlook.timezone` не указан, время начала и завершения возвращается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="f5b87-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="f5b87-118">Узнать, какой именно часовой пояс использовался при создании события, позволят свойства **OriginalStartTimeZone** и **OriginalEndTimeZone** ресурса **event**.</span><span class="sxs-lookup"><span data-stu-id="f5b87-118">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>


## <a name="permissions"></a><span data-ttu-id="f5b87-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5b87-119">Permissions</span></span>
<span data-ttu-id="f5b87-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5b87-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5b87-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5b87-122">Permission type</span></span>      | <span data-ttu-id="f5b87-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5b87-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5b87-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5b87-124">Delegated (work or school account)</span></span> | <span data-ttu-id="f5b87-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f5b87-125">Calendars.Read</span></span>    |
|<span data-ttu-id="f5b87-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5b87-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5b87-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f5b87-127">Calendars.Read</span></span>    |
|<span data-ttu-id="f5b87-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5b87-128">Application</span></span> | <span data-ttu-id="f5b87-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f5b87-129">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5b87-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5b87-130">HTTP request</span></span>
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

GET /me/calendargroups/{id}/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f5b87-131">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f5b87-131">Optional query parameters</span></span>
<span data-ttu-id="f5b87-132">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f5b87-132">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f5b87-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5b87-133">Request headers</span></span>
| <span data-ttu-id="f5b87-134">Имя</span><span class="sxs-lookup"><span data-stu-id="f5b87-134">Name</span></span>       | <span data-ttu-id="f5b87-135">Тип</span><span class="sxs-lookup"><span data-stu-id="f5b87-135">Type</span></span> | <span data-ttu-id="f5b87-136">Описание</span><span class="sxs-lookup"><span data-stu-id="f5b87-136">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="f5b87-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5b87-137">Authorization</span></span>  | <span data-ttu-id="f5b87-138">string</span><span class="sxs-lookup"><span data-stu-id="f5b87-138">string</span></span> | <span data-ttu-id="f5b87-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5b87-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f5b87-141">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="f5b87-141">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="f5b87-142">string</span><span class="sxs-lookup"><span data-stu-id="f5b87-142">string</span></span> | <span data-ttu-id="f5b87-143">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="f5b87-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="f5b87-144">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="f5b87-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="f5b87-145">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="f5b87-145">Optional.</span></span> |
| <span data-ttu-id="f5b87-146">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="f5b87-146">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="f5b87-147">string</span><span class="sxs-lookup"><span data-stu-id="f5b87-147">string</span></span> | <span data-ttu-id="f5b87-148">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="f5b87-148">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="f5b87-149">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="f5b87-149">Values can be "text" or "html".</span></span> <span data-ttu-id="f5b87-150">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="f5b87-150">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="f5b87-151">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="f5b87-151">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="f5b87-152">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="f5b87-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5b87-153">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5b87-153">Request body</span></span>
<span data-ttu-id="f5b87-154">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f5b87-154">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5b87-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5b87-155">Response</span></span>

<span data-ttu-id="f5b87-156">В случае успеха этот метод возвратит код отклика `200 OK` и объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f5b87-156">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5b87-157">Пример</span><span class="sxs-lookup"><span data-stu-id="f5b87-157">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="f5b87-158">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="f5b87-158">Request 1</span></span>
<span data-ttu-id="f5b87-p107">Первый пример возвращает указанное событие. Он указывает следующее:</span><span class="sxs-lookup"><span data-stu-id="f5b87-p107">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="f5b87-161">Заголовок `Prefer: outlook.timezone` для получения значений даты и времени, которые возвращаются для стандартного тихоокеанского времени.</span><span class="sxs-lookup"><span data-stu-id="f5b87-161">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="f5b87-p108">Параметр запроса `$select`, который возвращает конкретные свойства. Без параметра `$select` будут возвращены все свойства событий.</span><span class="sxs-lookup"><span data-stu-id="f5b87-p108">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>


# <a name="http"></a>[<span data-ttu-id="f5b87-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5b87-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGIAAAoZDOFAAA="],
  "name": "get_event"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/events/AAMkAGIAAAoZDOFAAA=?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees 
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[<span data-ttu-id="f5b87-165">C#</span><span class="sxs-lookup"><span data-stu-id="f5b87-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5b87-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5b87-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5b87-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5b87-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5b87-168">Java</span><span class="sxs-lookup"><span data-stu-id="f5b87-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="f5b87-169">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="f5b87-169">Response 1</span></span>

<span data-ttu-id="f5b87-p109">Ниже приведен пример отклика. Свойство **body** возвращается в формате HTML по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f5b87-p109">Here is an example of the response. The **body** property is returned in the default format of HTML.</span></span>

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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees)/$entity",
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
    "hideAttendees": false,
    "organizer":{
        "emailAddress":{
            "name":"Samantha Booth",
            "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
        }
    }
}
```


##### <a name="request-2"></a><span data-ttu-id="f5b87-172">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="f5b87-172">Request 2</span></span>

<span data-ttu-id="f5b87-173">Во втором примере показано получение события с указанием нескольких мест.</span><span class="sxs-lookup"><span data-stu-id="f5b87-173">The second example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="f5b87-174">В запросе указан параметр `$select` для возврата отдельных свойств.</span><span class="sxs-lookup"><span data-stu-id="f5b87-174">The request specifies a `$select` query parameter to return specific properties.</span></span> 


# <a name="http"></a>[<span data-ttu-id="f5b87-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5b87-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADAGAADDdm4NAAA="],
  "name": "get_event_multiple_locations"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/events/AAMkADAGAADDdm4NAAA=?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
# <a name="c"></a>[<span data-ttu-id="f5b87-176">C#</span><span class="sxs-lookup"><span data-stu-id="f5b87-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-multiple-locations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5b87-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5b87-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-multiple-locations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5b87-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5b87-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-multiple-locations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5b87-179">Java</span><span class="sxs-lookup"><span data-stu-id="f5b87-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-multiple-locations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="f5b87-180">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="f5b87-180">Response 2</span></span>
<span data-ttu-id="f5b87-181">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f5b87-181">Here is an example of the response.</span></span> <span data-ttu-id="f5b87-182">Свойство **locations** включает информацию о трех местах, для которых организовано событие.</span><span class="sxs-lookup"><span data-stu-id="f5b87-182">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="f5b87-183">Так как в запросе не указан заголовок `Prefer: outlook.timezone`, свойства **start** и **end** отображаются в стандартном часовом поясе UTC.</span><span class="sxs-lookup"><span data-stu-id="f5b87-183">Because the request does not specify any `Prefer: outlook.timezone` header, the **start** and **end** properties are displayed in the default UTC time zone.</span></span> 

<span data-ttu-id="f5b87-184">Тело события возвращается в стандартном формате HTML.</span><span class="sxs-lookup"><span data-stu-id="f5b87-184">The event body is in the default HTML format.</span></span>  

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,locations)/$entity",
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



## <a name="see-also"></a><span data-ttu-id="f5b87-185">См. также</span><span class="sxs-lookup"><span data-stu-id="f5b87-185">See also</span></span>

- [<span data-ttu-id="f5b87-186">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="f5b87-186">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f5b87-187">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="f5b87-187">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="f5b87-188">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="f5b87-188">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
