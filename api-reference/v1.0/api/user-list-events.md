---
title: Список событий
description: 'Получение списка объектов event в почтовом ящике пользователя. Этот список содержит '
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6d1f83f272f505c5dc18819f1d71929e29358bf0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439956"
---
# <a name="list-events"></a><span data-ttu-id="a0e88-104">Перечисление событий</span><span class="sxs-lookup"><span data-stu-id="a0e88-104">List events</span></span>

<span data-ttu-id="a0e88-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0e88-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a0e88-p102">Получение списка объектов [event](../resources/event.md) в почтовом ящике пользователя. Этот список содержит собрания с одним экземпляром и образцы рядов.</span><span class="sxs-lookup"><span data-stu-id="a0e88-p102">Get a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="a0e88-108">Чтобы получить расширенные экземпляры события, вы можете [получить представление календаря](calendar-list-calendarview.md) или [экземпляры события](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="a0e88-108">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

<span data-ttu-id="a0e88-109">В настоящее время эта операция возвращает текст события только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="a0e88-109">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="a0e88-110">Существует два сценария, в которых приложение может получить события из календаря другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="a0e88-110">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="a0e88-111">если у приложения есть разрешения для приложений;</span><span class="sxs-lookup"><span data-stu-id="a0e88-111">If the app has application permissions, or,</span></span>
* <span data-ttu-id="a0e88-112">если у приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним календарем или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="a0e88-112">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="a0e88-113">См. [подробные сведения и пример](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="a0e88-113">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

### <a name="support-various-time-zones"></a><span data-ttu-id="a0e88-114">Поддержка разных часовых поясов</span><span class="sxs-lookup"><span data-stu-id="a0e88-114">Support various time zones</span></span>

<span data-ttu-id="a0e88-115">Для всех операций GET, которые возвращают события, можно использовать заголовок `Prefer: outlook.timezone`, чтобы задать часовой пояс для указанного в отклике времени начала и завершения события.</span><span class="sxs-lookup"><span data-stu-id="a0e88-115">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="a0e88-116">Например, заголовок `Prefer: outlook.timezone` задает в отклике время начала и завершения согласно североамериканскому восточному времени.</span><span class="sxs-lookup"><span data-stu-id="a0e88-116">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="a0e88-p104">Если событие создано с применением другого часового пояса, время начала и завершения будет изменено в соответствии с часовым поясом, указанным в заголовке `Prefer`. Поддерживаемые часовые пояса указаны в этом [списке](../resources/datetimetimezone.md). Если заголовок `Prefer: outlook.timezone` не указан, время начала и завершения возвращается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="a0e88-p104">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="a0e88-120">Узнать, какой именно часовой пояс использовался при создании события, позволят свойства **OriginalStartTimeZone** и **OriginalEndTimeZone** ресурса **event**.</span><span class="sxs-lookup"><span data-stu-id="a0e88-120">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0e88-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0e88-121">Permissions</span></span>
<span data-ttu-id="a0e88-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0e88-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0e88-124">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0e88-124">Permission type</span></span>      | <span data-ttu-id="a0e88-125">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0e88-125">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0e88-126">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0e88-126">Delegated (work or school account)</span></span> | <span data-ttu-id="a0e88-127">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0e88-127">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a0e88-128">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0e88-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0e88-129">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0e88-129">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a0e88-130">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0e88-130">Application</span></span> | <span data-ttu-id="a0e88-131">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0e88-131">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0e88-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0e88-132">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="a0e88-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a0e88-133">Optional query parameters</span></span>
<span data-ttu-id="a0e88-134">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a0e88-134">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a0e88-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0e88-135">Request headers</span></span>
| <span data-ttu-id="a0e88-136">Имя</span><span class="sxs-lookup"><span data-stu-id="a0e88-136">Name</span></span>       | <span data-ttu-id="a0e88-137">Тип</span><span class="sxs-lookup"><span data-stu-id="a0e88-137">Type</span></span> | <span data-ttu-id="a0e88-138">Описание</span><span class="sxs-lookup"><span data-stu-id="a0e88-138">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="a0e88-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0e88-139">Authorization</span></span>  | <span data-ttu-id="a0e88-140">string</span><span class="sxs-lookup"><span data-stu-id="a0e88-140">string</span></span> | <span data-ttu-id="a0e88-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0e88-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a0e88-143">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="a0e88-143">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="a0e88-144">string</span><span class="sxs-lookup"><span data-stu-id="a0e88-144">string</span></span> | <span data-ttu-id="a0e88-145">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="a0e88-145">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="a0e88-146">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="a0e88-146">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="a0e88-147">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a0e88-147">Optional.</span></span> |
| <span data-ttu-id="a0e88-148">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="a0e88-148">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="a0e88-149">string</span><span class="sxs-lookup"><span data-stu-id="a0e88-149">string</span></span> | <span data-ttu-id="a0e88-150">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="a0e88-150">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="a0e88-151">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="a0e88-151">Values can be "text" or "html".</span></span> <span data-ttu-id="a0e88-152">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="a0e88-152">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="a0e88-153">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="a0e88-153">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="a0e88-154">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a0e88-154">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0e88-155">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0e88-155">Request body</span></span>
<span data-ttu-id="a0e88-156">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0e88-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0e88-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0e88-157">Response</span></span>

<span data-ttu-id="a0e88-158">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a0e88-158">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a0e88-159">Пример</span><span class="sxs-lookup"><span data-stu-id="a0e88-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0e88-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0e88-160">Request</span></span>
<span data-ttu-id="a0e88-p109">Ниже приведен пример запроса. Он указывает следующее:</span><span class="sxs-lookup"><span data-stu-id="a0e88-p109">Here is an example of the request. It specifies the following:</span></span>

- <span data-ttu-id="a0e88-163">Заголовок `Prefer: outlook.timezone` для получения значений даты и времени, которые возвращаются для стандартного тихоокеанского времени.</span><span class="sxs-lookup"><span data-stu-id="a0e88-163">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="a0e88-p110">Параметр запроса `$select`, который возвращает конкретные свойства. Без параметра `$select` будут возвращены все свойства событий.</span><span class="sxs-lookup"><span data-stu-id="a0e88-p110">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>


# <a name="http"></a>[<span data-ttu-id="a0e88-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0e88-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[<span data-ttu-id="a0e88-167">C#</span><span class="sxs-lookup"><span data-stu-id="a0e88-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0e88-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0e88-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0e88-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0e88-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0e88-170">Java</span><span class="sxs-lookup"><span data-stu-id="a0e88-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a0e88-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0e88-171">Response</span></span>
<span data-ttu-id="a0e88-p111">Ниже приведен пример отклика. Свойство **body** возвращается в формате HTML по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a0e88-p111">Here is an example of the response. The **body** property is returned in the default HTML format.</span></span>
<!-- {
  "blockType": "response",
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
