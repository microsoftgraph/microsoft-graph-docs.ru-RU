---
title: Список экземпляров
description: Получение экземпляров (повторов) события для заданного диапазона времени.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 73db9643de5fa34d3ff1efff1a22773d859e5055
ms.sourcegitcommit: e6168b868660ad0078d460424d4e6f987d2684a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2019
ms.locfileid: "31026019"
---
# <a name="list-instances"></a><span data-ttu-id="7328a-103">Список экземпляров</span><span class="sxs-lookup"><span data-stu-id="7328a-103">List instances</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7328a-104">Получение экземпляров (повторов) события для заданного диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="7328a-104">Get the instances (occurrences) of an event for a specified time range.</span></span> 

<span data-ttu-id="7328a-105">Если событие относится к типу `seriesMaster`, возвращаются экземпляры и исключения события для указанного диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="7328a-105">If the event is a `seriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="7328a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7328a-106">Permissions</span></span>
<span data-ttu-id="7328a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7328a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7328a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7328a-109">Permission type</span></span>      | <span data-ttu-id="7328a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7328a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7328a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7328a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7328a-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7328a-112">Calendars.Read</span></span>    |
|<span data-ttu-id="7328a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7328a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7328a-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7328a-114">Calendars.Read</span></span>    |
|<span data-ttu-id="7328a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7328a-115">Application</span></span> | <span data-ttu-id="7328a-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7328a-116">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="7328a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7328a-117">HTTP request</span></span>
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
## <a name="query-parameters"></a><span data-ttu-id="7328a-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="7328a-118">Query parameters</span></span>

<span data-ttu-id="7328a-119">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="7328a-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="7328a-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="7328a-120">Parameter</span></span>    | <span data-ttu-id="7328a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="7328a-121">Type</span></span>   |<span data-ttu-id="7328a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7328a-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7328a-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7328a-123">startDateTime</span></span>|<span data-ttu-id="7328a-124">String</span><span class="sxs-lookup"><span data-stu-id="7328a-124">String</span></span>|<span data-ttu-id="7328a-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="7328a-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="7328a-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7328a-127">endDateTime</span></span>|<span data-ttu-id="7328a-128">String</span><span class="sxs-lookup"><span data-stu-id="7328a-128">String</span></span>|<span data-ttu-id="7328a-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="7328a-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="7328a-131">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7328a-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7328a-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7328a-132">Request headers</span></span>
| <span data-ttu-id="7328a-133">Имя</span><span class="sxs-lookup"><span data-stu-id="7328a-133">Name</span></span>       | <span data-ttu-id="7328a-134">Тип</span><span class="sxs-lookup"><span data-stu-id="7328a-134">Type</span></span> | <span data-ttu-id="7328a-135">Описание</span><span class="sxs-lookup"><span data-stu-id="7328a-135">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="7328a-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="7328a-136">Authorization</span></span>  | <span data-ttu-id="7328a-137">string</span><span class="sxs-lookup"><span data-stu-id="7328a-137">string</span></span> | <span data-ttu-id="7328a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7328a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7328a-140">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="7328a-140">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="7328a-141">string</span><span class="sxs-lookup"><span data-stu-id="7328a-141">string</span></span> | <span data-ttu-id="7328a-142">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="7328a-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="7328a-143">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="7328a-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="7328a-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7328a-144">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7328a-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7328a-145">Request body</span></span>
<span data-ttu-id="7328a-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7328a-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7328a-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="7328a-147">Response</span></span>

<span data-ttu-id="7328a-148">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7328a-148">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7328a-149">Пример</span><span class="sxs-lookup"><span data-stu-id="7328a-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7328a-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="7328a-150">Request</span></span>
<span data-ttu-id="7328a-151">В приведенном ниже примере выполняется получение в заданном диапазоне времени вхождений и исключений события, которое является главным событием повторяющейся серии.</span><span class="sxs-lookup"><span data-stu-id="7328a-151">The following example gets within the specified time range the occurrences and exceptions of an event which is the master event of a recurring series.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/AAMkAGUzYRgWAAA=/instances?startDateTime=2019-04-08T09:00:00.0000000&endDateTime=2019-04-30T09:00:00.0000000&$select=subject,bodyPreview,seriesMasterId,type,recurrence,start,end
```
##### <a name="response"></a><span data-ttu-id="7328a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="7328a-152">Response</span></span>
<span data-ttu-id="7328a-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7328a-153">Here is an example of the response.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances",
  "sampleKeys": ["AAMkAGUzYRgWAAA="],
  "name": "get_instances"
}-->
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
    "Error: /api-reference/beta/api/event-list-instances.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
