---
title: Вывод события
description: Получение свойств и отношений указанного объекта event.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 44007d0c4b8ad4feaf97cb3940fac388b9cca902
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436234"
---
# <a name="get-event"></a><span data-ttu-id="6bfa8-103">Вывод события</span><span class="sxs-lookup"><span data-stu-id="6bfa8-103">Get event</span></span>

<span data-ttu-id="6bfa8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bfa8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bfa8-105">Получение свойств и отношений указанного объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="6bfa8-105">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="6bfa8-106">Приложение может получить событие в календаре другого пользователя, если:</span><span class="sxs-lookup"><span data-stu-id="6bfa8-106">An app can get an event in another user's calendar if:</span></span>

* <span data-ttu-id="6bfa8-107">У приложения есть разрешения на приложения</span><span class="sxs-lookup"><span data-stu-id="6bfa8-107">The app has application permissions</span></span>
* <span data-ttu-id="6bfa8-108">Приложение имеет соответствующие [](#permissions) делегированные разрешения от одного пользователя, а другой пользователь поделился календарем с этим пользователем или предоставил ему делегированную возможность доступа.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-108">The app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or has given delegated access to that user.</span></span> <span data-ttu-id="6bfa8-109">См. [подробные сведения и пример](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="6bfa8-109">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

<span data-ttu-id="6bfa8-110">Так как **ресурс событий** поддерживает [расширения,](/graph/extensibility-overview)вы также можете использовать операцию для получения настраиваемой информации о свойствах и расширении `GET` в **экземпляре** события.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-110">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="6bfa8-111">Поддержка разных часовых поясов</span><span class="sxs-lookup"><span data-stu-id="6bfa8-111">Support various time zones</span></span>

<span data-ttu-id="6bfa8-112">Для всех операций GET, которые возвращают события, можно использовать заголовок `Prefer: outlook.timezone`, чтобы задать часовой пояс для указанного в отклике времени начала и завершения события.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-112">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="6bfa8-113">Например, заголовок `Prefer: outlook.timezone` задает в отклике время начала и завершения согласно североамериканскому восточному времени.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-113">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="6bfa8-p102">Если событие создано с применением другого часового пояса, время начала и завершения будет изменено в соответствии с часовым поясом, указанным в заголовке `Prefer`. Поддерживаемые часовые пояса указаны в этом [списке](../resources/datetimetimezone.md). Если заголовок `Prefer: outlook.timezone` не указан, время начала и завершения возвращается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="6bfa8-117">Узнать, какой именно часовой пояс использовался при создании события, позволят свойства **OriginalStartTimeZone** и **OriginalEndTimeZone** ресурса **event**.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-117">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="6bfa8-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6bfa8-118">Permissions</span></span>
<span data-ttu-id="6bfa8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bfa8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bfa8-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6bfa8-121">Permission type</span></span>      | <span data-ttu-id="6bfa8-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6bfa8-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6bfa8-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6bfa8-123">Delegated (work or school account)</span></span> | <span data-ttu-id="6bfa8-124">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6bfa8-124">Calendars.Read</span></span>    |
|<span data-ttu-id="6bfa8-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6bfa8-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bfa8-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6bfa8-126">Calendars.Read</span></span>    |
|<span data-ttu-id="6bfa8-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6bfa8-127">Application</span></span> | <span data-ttu-id="6bfa8-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6bfa8-128">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="6bfa8-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6bfa8-129">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="6bfa8-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6bfa8-130">Optional query parameters</span></span>
<span data-ttu-id="6bfa8-131">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-131">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6bfa8-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6bfa8-132">Request headers</span></span>
| <span data-ttu-id="6bfa8-133">Имя</span><span class="sxs-lookup"><span data-stu-id="6bfa8-133">Name</span></span>       | <span data-ttu-id="6bfa8-134">Тип</span><span class="sxs-lookup"><span data-stu-id="6bfa8-134">Type</span></span> | <span data-ttu-id="6bfa8-135">Описание</span><span class="sxs-lookup"><span data-stu-id="6bfa8-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6bfa8-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bfa8-136">Authorization</span></span>  | <span data-ttu-id="6bfa8-137">string</span><span class="sxs-lookup"><span data-stu-id="6bfa8-137">string</span></span>  | <span data-ttu-id="6bfa8-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6bfa8-140">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="6bfa8-140">Prefer: outlook.timezone</span></span> | <span data-ttu-id="6bfa8-141">string</span><span class="sxs-lookup"><span data-stu-id="6bfa8-141">string</span></span> | <span data-ttu-id="6bfa8-142">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="6bfa8-143">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="6bfa8-144">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-144">Optional.</span></span> |
| <span data-ttu-id="6bfa8-145">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="6bfa8-145">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="6bfa8-146">string</span><span class="sxs-lookup"><span data-stu-id="6bfa8-146">string</span></span> | <span data-ttu-id="6bfa8-147">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-147">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="6bfa8-148">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="6bfa8-148">Values can be "text" or "html".</span></span> <span data-ttu-id="6bfa8-149">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-149">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="6bfa8-150">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-150">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="6bfa8-151">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6bfa8-152">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6bfa8-152">Request body</span></span>
<span data-ttu-id="6bfa8-153">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bfa8-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bfa8-154">Response</span></span>

<span data-ttu-id="6bfa8-155">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-155">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="6bfa8-156">Примеры</span><span class="sxs-lookup"><span data-stu-id="6bfa8-156">Examples</span></span>

### <a name="example-1-get-a-specified-event"></a><span data-ttu-id="6bfa8-157">Пример 1. Получить указанное событие</span><span class="sxs-lookup"><span data-stu-id="6bfa8-157">Example 1: Get a specified event</span></span>
#### <a name="request"></a><span data-ttu-id="6bfa8-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bfa8-158">Request</span></span>
<span data-ttu-id="6bfa8-159">В следующем примере получается указанное событие.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-159">The following example gets the specified event.</span></span> <span data-ttu-id="6bfa8-160">В нем указывается:</span><span class="sxs-lookup"><span data-stu-id="6bfa8-160">It specifies the following:</span></span>

- <span data-ttu-id="6bfa8-161">Заголовок `Prefer: outlook.timezone` для получения значений даты и времени, которые возвращаются для стандартного тихоокеанского времени.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-161">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="6bfa8-p108">Параметр запроса `$select`, который возвращает конкретные свойства. Без параметра `$select` будут возвращены все свойства событий.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-p108">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="6bfa8-164">В запросе не определен никакой заголовок `Prefer: outlook.body-content-type`, чтобы указать конкретный формат для текста возвращаемого события.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-164">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 


# <a name="http"></a>[<span data-ttu-id="6bfa8-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="6bfa8-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGIAAAoZDOFAAA=/?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees 
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[<span data-ttu-id="6bfa8-166">C#</span><span class="sxs-lookup"><span data-stu-id="6bfa8-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6bfa8-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6bfa8-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6bfa8-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6bfa8-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6bfa8-169">Java</span><span class="sxs-lookup"><span data-stu-id="6bfa8-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6bfa8-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bfa8-170">Response</span></span>
<span data-ttu-id="6bfa8-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-171">Here is an example of the response.</span></span> <span data-ttu-id="6bfa8-172">Так как заголовок `Prefer: outlook.body-content-type` не указан, свойство **body** возвращается в формате HTML по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-172">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span> 

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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees)/$entity",
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
### <a name="example-2-get-the-body-property-in-text-format"></a><span data-ttu-id="6bfa8-173">Пример 2. Получить свойство body в текстовом формате</span><span class="sxs-lookup"><span data-stu-id="6bfa8-173">Example 2: Get the body property in text format</span></span>
#### <a name="request"></a><span data-ttu-id="6bfa8-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bfa8-174">Request</span></span>
<span data-ttu-id="6bfa8-175">В следующем примере показано, как использовать заголовка для получения свойства тела указанного события `Prefer: outlook.body-content-type="text"` в текстовом  формате.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-175">The following example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified event in text format.</span></span>

<span data-ttu-id="6bfa8-176">В запросе также используется параметр `$select` для возврата отдельных свойств.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-176">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="6bfa8-177">Без параметра `$select` будут возвращены все свойства событий.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-177">Without a `$select` parameter, all of the event properties will be returned.</span></span>


# <a name="http"></a>[<span data-ttu-id="6bfa8-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="6bfa8-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGI1AAAoZDOFAAA=/?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="6bfa8-179">C#</span><span class="sxs-lookup"><span data-stu-id="6bfa8-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6bfa8-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6bfa8-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6bfa8-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6bfa8-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6bfa8-182">Java</span><span class="sxs-lookup"><span data-stu-id="6bfa8-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6bfa8-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bfa8-183">Response</span></span>
<span data-ttu-id="6bfa8-184">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-184">Here is an example of the response.</span></span> <span data-ttu-id="6bfa8-185">Свойство **body** возвращается в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-185">The **body** property is returned in text format.</span></span> 

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

### <a name="example-3-get-an-event-that-specifies-more-than-one-location"></a><span data-ttu-id="6bfa8-186">Пример 3. Получить событие, которое указывает несколько местоположений</span><span class="sxs-lookup"><span data-stu-id="6bfa8-186">Example 3: Get an event that specifies more than one location</span></span>
#### <a name="request"></a><span data-ttu-id="6bfa8-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bfa8-187">Request</span></span>

<span data-ttu-id="6bfa8-188">В следующем примере показано получение события, которое указывает несколько расположений.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-188">The following example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="6bfa8-189">В запросе указан параметр `$select` для возврата отдельных свойств.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-189">The request specifies a `$select` query parameter to return specific properties.</span></span> 


# <a name="http"></a>[<span data-ttu-id="6bfa8-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="6bfa8-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_multiple_locations"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkADAGAADDdm4NAAA=/?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
# <a name="c"></a>[<span data-ttu-id="6bfa8-191">C#</span><span class="sxs-lookup"><span data-stu-id="6bfa8-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-multiple-locations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6bfa8-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6bfa8-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-multiple-locations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6bfa8-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6bfa8-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-multiple-locations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6bfa8-194">Java</span><span class="sxs-lookup"><span data-stu-id="6bfa8-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-multiple-locations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6bfa8-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bfa8-195">Response</span></span>
<span data-ttu-id="6bfa8-196">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-196">Here is an example of the response.</span></span> <span data-ttu-id="6bfa8-197">Свойство **locations** включает информацию о трех местах, для которых организовано событие.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-197">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="6bfa8-198">Так как в запросе не указаны какие-либо заголовки или заголовки, свойства запуска и окончания отображаются в часовом поясе UTC по умолчанию, а тело находится в `Prefer: outlook.timezone` HTML-формате `Prefer: outlook.body-content-type` по умолчанию.  </span><span class="sxs-lookup"><span data-stu-id="6bfa8-198">Because the request does not specify any `Prefer: outlook.timezone` or `Prefer: outlook.body-content-type` header, the **start** and **end** properties are displayed in the default UTC time zone, and the body is in the default HTML format.</span></span>  

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
### <a name="example-4-expand-a-series-master-event"></a><span data-ttu-id="6bfa8-199">Пример 4. Расширение мастер-события серии</span><span class="sxs-lookup"><span data-stu-id="6bfa8-199">Example 4: Expand a series master event</span></span>
#### <a name="request"></a><span data-ttu-id="6bfa8-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bfa8-200">Request</span></span>

<span data-ttu-id="6bfa8-201">В следующем примере показано расширение мастер-события серии повторяющихся серий с исключениями и отмененными событиями.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-201">The following example shows expanding a series master event of a recurring series with exceptions and cancelled occurences.</span></span> <span data-ttu-id="6bfa8-202">В запросе указан параметр `$select` для возврата отдельных свойств.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-202">The request specifies a `$select` query parameter to return specific properties.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_event_seriesMaster_expansion"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkADAGAADDdm4NAAA=/?$select=subject,start,end,occurrenceId,exceptionOccurrences,cancelledOccurrences$expand=exceptionOccurrences
```
#### <a name="response"></a><span data-ttu-id="6bfa8-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bfa8-203">Response</span></span>
<span data-ttu-id="6bfa8-204">Операция GET возвращает выбранные свойства для мастер-события серии.</span><span class="sxs-lookup"><span data-stu-id="6bfa8-204">The GET operation returns the selected properties for the series master event.</span></span> <span data-ttu-id="6bfa8-205">В частности, для событий в коллекции **exceptionOccurrences** операция возвращает свойство **id** и применимые, выбранные свойства **(subject,** **start**, **end**, **occurrenceId).**</span><span class="sxs-lookup"><span data-stu-id="6bfa8-205">Specifically, for events in the **exceptionOccurrences** collection, the operation returns the **id** property, and the applicable, selected properties (**subject**, **start**, **end**, **occurrenceId**).</span></span> <span data-ttu-id="6bfa8-206">Что касается событий в **коллекции cancelledOccurrences,** так как события больше не существуют, операция возвращает только значения **свойств occurrenceId.**</span><span class="sxs-lookup"><span data-stu-id="6bfa8-206">As for events in the **cancelledOccurrences** collection, because the events no longer exist, the operation returns only their **occurrenceId** property values.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_event_seriesMaster_expansion",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1992

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,start,end,occurrenceId,exceptionOccurrences,cancelledOccurrences)/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "subject": "Daily stand-up",
  "cancelledOccurrences": [
     "OID.AAMkADAGAADDdm4NAAA=.2020-04-30",
     "OID.AAMkADAGAADDdm4NAAA=.2020-05-07",
     "OID.AAMkADAGAADDdm4NAAA=.2020-05-14"
    ],
  "occurrenceId": null,
    "start": {
        "dateTime": "2020-04-23T11:30:00.0000000",
        "timeZone": "UTC"
    },
  "end": {
        "dateTime": "2020-04-23T12:00:00.0000000",
        "timeZone": "UTC"
    },
  "exceptionOccurrences": [
        {
            "id": "AAMkADM0ZGRhMjdjLTA==",
            "Subject": "SM update 24",
            "occurrenceId": "OID.AAMkADAGAADDdm4NAAA=.2020-05-21",
            "start": {
                "dateTime": "2020-05-21T11:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2020-05-21T12:00:00.0000000",
                "timeZone": "UTC"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="6bfa8-207">См. также</span><span class="sxs-lookup"><span data-stu-id="6bfa8-207">See also</span></span>

- [<span data-ttu-id="6bfa8-208">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="6bfa8-208">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6bfa8-209">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="6bfa8-209">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="6bfa8-210">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="6bfa8-210">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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


