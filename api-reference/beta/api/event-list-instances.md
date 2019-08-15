---
title: Список экземпляров
description: Получение экземпляров (повторов) события для заданного диапазона времени.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f98e725ef67709c91b0b049d4f6f41481696139c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419939"
---
# <a name="list-instances"></a><span data-ttu-id="ef2fc-103">Список экземпляров</span><span class="sxs-lookup"><span data-stu-id="ef2fc-103">List instances</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef2fc-104">Получение экземпляров (повторов) события для заданного диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="ef2fc-104">Get the instances (occurrences) of an event for a specified time range.</span></span> 

<span data-ttu-id="ef2fc-105">Если событие относится к типу `seriesMaster`, возвращаются экземпляры и исключения события для указанного диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="ef2fc-105">If the event is a `seriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef2fc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef2fc-106">Permissions</span></span>
<span data-ttu-id="ef2fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef2fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef2fc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef2fc-109">Permission type</span></span>      | <span data-ttu-id="ef2fc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef2fc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef2fc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef2fc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ef2fc-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ef2fc-112">Calendars.Read</span></span>    |
|<span data-ttu-id="ef2fc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef2fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef2fc-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ef2fc-114">Calendars.Read</span></span>    |
|<span data-ttu-id="ef2fc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef2fc-115">Application</span></span> | <span data-ttu-id="ef2fc-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ef2fc-116">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef2fc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef2fc-117">HTTP request</span></span>
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

GET /me/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="ef2fc-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="ef2fc-118">Query parameters</span></span>

<span data-ttu-id="ef2fc-119">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ef2fc-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="ef2fc-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="ef2fc-120">Parameter</span></span>    | <span data-ttu-id="ef2fc-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ef2fc-121">Type</span></span>   |<span data-ttu-id="ef2fc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ef2fc-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef2fc-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ef2fc-123">startDateTime</span></span>|<span data-ttu-id="ef2fc-124">String</span><span class="sxs-lookup"><span data-stu-id="ef2fc-124">String</span></span>|<span data-ttu-id="ef2fc-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="ef2fc-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="ef2fc-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ef2fc-127">endDateTime</span></span>|<span data-ttu-id="ef2fc-128">String</span><span class="sxs-lookup"><span data-stu-id="ef2fc-128">String</span></span>|<span data-ttu-id="ef2fc-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="ef2fc-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="ef2fc-131">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ef2fc-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ef2fc-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef2fc-132">Request headers</span></span>
| <span data-ttu-id="ef2fc-133">Имя</span><span class="sxs-lookup"><span data-stu-id="ef2fc-133">Name</span></span>       | <span data-ttu-id="ef2fc-134">Тип</span><span class="sxs-lookup"><span data-stu-id="ef2fc-134">Type</span></span> | <span data-ttu-id="ef2fc-135">Описание</span><span class="sxs-lookup"><span data-stu-id="ef2fc-135">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="ef2fc-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef2fc-136">Authorization</span></span>  | <span data-ttu-id="ef2fc-137">string</span><span class="sxs-lookup"><span data-stu-id="ef2fc-137">string</span></span> | <span data-ttu-id="ef2fc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef2fc-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ef2fc-140">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="ef2fc-140">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="ef2fc-141">string</span><span class="sxs-lookup"><span data-stu-id="ef2fc-141">string</span></span> | <span data-ttu-id="ef2fc-142">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="ef2fc-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="ef2fc-143">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="ef2fc-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="ef2fc-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ef2fc-144">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef2fc-145">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef2fc-145">Request body</span></span>
<span data-ttu-id="ef2fc-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef2fc-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef2fc-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef2fc-147">Response</span></span>

<span data-ttu-id="ef2fc-148">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ef2fc-148">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ef2fc-149">Пример</span><span class="sxs-lookup"><span data-stu-id="ef2fc-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef2fc-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef2fc-150">Request</span></span>
<span data-ttu-id="ef2fc-151">В приведенном ниже примере выполняется получение в заданном диапазоне времени вхождений и исключений события, которое является главным событием повторяющейся серии.</span><span class="sxs-lookup"><span data-stu-id="ef2fc-151">The following example gets within the specified time range the occurrences and exceptions of an event which is the master event of a recurring series.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ef2fc-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef2fc-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGUzYRgWAAA="],
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/AAMkAGUzYRgWAAA=/instances?startDateTime=2019-04-08T09:00:00.0000000&endDateTime=2019-04-30T09:00:00.0000000&$select=subject,bodyPreview,seriesMasterId,type,recurrence,start,end
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ef2fc-153">C#</span><span class="sxs-lookup"><span data-stu-id="ef2fc-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-instances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef2fc-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef2fc-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-instances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ef2fc-155">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ef2fc-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-instances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ef2fc-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef2fc-156">Response</span></span>
<span data-ttu-id="ef2fc-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ef2fc-157">Here is an example of the response.</span></span> 
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/events('AAMkAGUzYRgWAAA%3D')/instances(subject,bodyPreview,seriesMasterId,type,recurrence,start,end)",
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
<!--
{
  "type": "#page.annotation",
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
