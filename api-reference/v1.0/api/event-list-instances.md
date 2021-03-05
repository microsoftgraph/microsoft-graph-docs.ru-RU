---
title: Список экземпляров
description: Получение экземпляров (повторов) события для заданного диапазона времени.
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b19b452f029b7d4223bcc150f184b805a311cecd
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448293"
---
# <a name="list-instances"></a><span data-ttu-id="ff9fc-103">экземпляры списков;</span><span class="sxs-lookup"><span data-stu-id="ff9fc-103">List instances</span></span>

<span data-ttu-id="ff9fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff9fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ff9fc-105">Получение экземпляров (повторов) события для заданного диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="ff9fc-105">Get the instances (occurrences) of an event for a specified time range.</span></span> 

<span data-ttu-id="ff9fc-106">Если событие относится к типу `seriesMaster`, возвращаются экземпляры и исключения события для указанного диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="ff9fc-106">If the event is a `seriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff9fc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff9fc-107">Permissions</span></span>
<span data-ttu-id="ff9fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff9fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff9fc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff9fc-110">Permission type</span></span>      | <span data-ttu-id="ff9fc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff9fc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff9fc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff9fc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ff9fc-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ff9fc-113">Calendars.Read</span></span>    |
|<span data-ttu-id="ff9fc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff9fc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff9fc-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ff9fc-115">Calendars.Read</span></span>    |
|<span data-ttu-id="ff9fc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff9fc-116">Application</span></span> | <span data-ttu-id="ff9fc-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ff9fc-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff9fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff9fc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="ff9fc-119">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="ff9fc-119">Query parameters</span></span>

<span data-ttu-id="ff9fc-120">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ff9fc-120">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="ff9fc-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="ff9fc-121">Parameter</span></span>    | <span data-ttu-id="ff9fc-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ff9fc-122">Type</span></span>   |<span data-ttu-id="ff9fc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ff9fc-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff9fc-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ff9fc-124">startDateTime</span></span>|<span data-ttu-id="ff9fc-125">String</span><span class="sxs-lookup"><span data-stu-id="ff9fc-125">String</span></span>|<span data-ttu-id="ff9fc-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="ff9fc-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="ff9fc-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ff9fc-128">endDateTime</span></span>|<span data-ttu-id="ff9fc-129">String</span><span class="sxs-lookup"><span data-stu-id="ff9fc-129">String</span></span>|<span data-ttu-id="ff9fc-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="ff9fc-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="ff9fc-132">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ff9fc-132">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ff9fc-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff9fc-133">Request headers</span></span>
| <span data-ttu-id="ff9fc-134">Имя</span><span class="sxs-lookup"><span data-stu-id="ff9fc-134">Name</span></span>       | <span data-ttu-id="ff9fc-135">Тип</span><span class="sxs-lookup"><span data-stu-id="ff9fc-135">Type</span></span> | <span data-ttu-id="ff9fc-136">Описание</span><span class="sxs-lookup"><span data-stu-id="ff9fc-136">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="ff9fc-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff9fc-137">Authorization</span></span>  | <span data-ttu-id="ff9fc-138">string</span><span class="sxs-lookup"><span data-stu-id="ff9fc-138">string</span></span> | <span data-ttu-id="ff9fc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff9fc-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ff9fc-141">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="ff9fc-141">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="ff9fc-142">string</span><span class="sxs-lookup"><span data-stu-id="ff9fc-142">string</span></span> | <span data-ttu-id="ff9fc-143">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="ff9fc-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="ff9fc-144">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="ff9fc-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="ff9fc-145">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="ff9fc-145">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff9fc-146">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff9fc-146">Request body</span></span>
<span data-ttu-id="ff9fc-147">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff9fc-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff9fc-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff9fc-148">Response</span></span>

<span data-ttu-id="ff9fc-149">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ff9fc-149">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ff9fc-150">Пример</span><span class="sxs-lookup"><span data-stu-id="ff9fc-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff9fc-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff9fc-151">Request</span></span>
<span data-ttu-id="ff9fc-152">В следующем примере в указанном диапазоне времени заданы вхождения и исключения события, которое является мастер-событием повторяющейся серии.</span><span class="sxs-lookup"><span data-stu-id="ff9fc-152">The following example gets within the specified time range the occurrences and exceptions of an event which is the master event of a recurring series.</span></span>

# <a name="http"></a>[<span data-ttu-id="ff9fc-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff9fc-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGUzYRgWAAA="],
  "name": "get_instances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/events/AAMkAGUzYRgWAAA=/instances?startDateTime=2019-04-08T09:00:00.0000000&endDateTime=2019-04-30T09:00:00.0000000&$select=subject,bodyPreview,seriesMasterId,type,recurrence,start,end
```
# <a name="c"></a>[<span data-ttu-id="ff9fc-154">C#</span><span class="sxs-lookup"><span data-stu-id="ff9fc-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-instances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff9fc-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff9fc-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-instances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff9fc-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff9fc-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-instances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff9fc-157">Java</span><span class="sxs-lookup"><span data-stu-id="ff9fc-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-instances-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ff9fc-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff9fc-158">Response</span></span>
<span data-ttu-id="ff9fc-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ff9fc-159">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "get_instances",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/events('AAMkAGUzYRgWAAA%3D')/instances(subject,bodyPreview,seriesMasterId,type,recurrence,start,end)",
    "value": [
        {
            "@odata.etag": "W/\"x3IAvB5fbUWf4XNcBFLNUwAAKuA3yQ==\"",
            "id": "AAMkAGUzYAgI1sE1TatAAEYAAAAAlNFb2CNPe0ucP9you",
            "subject": "Review strategy for Q3",
            "bodyPreview": "Changing meeting from 4/15 to 4/16.",
            "seriesMasterId": "AAMkAGUzYRgWAAA=",
            "type": "exception",
            "recurrence": null,
            "start": {
                "dateTime": "2019-04-16T20:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2019-04-16T21:00:00.0000000",
                "timeZone": "UTC"
            }
        },
        {
            "@odata.etag": "W/\"x3IAvB5fbUWf4XNcBFLNUwAAKuA3yQ==\"",
            "id": "AAMkAGUzYAgI1ru1JMcAAEYAAAAAlNFb2CNPe0ucP9you",
            "subject": "Review strategy for Q3",
            "bodyPreview": "",
            "seriesMasterId": "AAMkAGUzYRgWAAA=",
            "type": "occurrence",
            "recurrence": null,
            "start": {
                "dateTime": "2019-04-08T20:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2019-04-08T21:00:00.0000000",
                "timeZone": "UTC"
            }
        },
        {
            "@odata.etag": "W/\"x3IAvB5fbUWf4XNcBFLNUwAAKuA3yQ==\"",
            "id": "AAMkAGUzYAgI1sa1do_AAEYAAAAAlNFb2CNPe0ucP9you",
            "subject": "Review strategy for Q3",
            "bodyPreview": "",
            "seriesMasterId": "AAMkAGUzYRgWAAA=",
            "type": "occurrence",
            "recurrence": null,
            "start": {
                "dateTime": "2019-04-22T20:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2019-04-22T21:00:00.0000000",
                "timeZone": "UTC"
            }
        },
        {
            "@odata.etag": "W/\"x3IAvB5fbUWf4XNcBFLNUwAAKuA3yQ==\"",
            "id": "AAMkAGUzYAgI1sw1n3PAAEYAAAAAlNFb2CNPe0ucP9you",
            "subject": "Review strategy for Q3",
            "bodyPreview": "",
            "seriesMasterId": "AAMkAGUzYRgWAAA=",
            "type": "occurrence",
            "recurrence": null,
            "start": {
                "dateTime": "2019-04-29T20:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2019-04-29T21:00:00.0000000",
                "timeZone": "UTC"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
