---
title: Список экземпляров
description: Получение экземпляров (вхождений) события для заданного интервала времени. Если событие `SeriesMaster` типа, при этом будет получен
ms.openlocfilehash: 101cc2988b96a0e865e448686095a187619c46ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079762"
---
# <a name="list-instances"></a><span data-ttu-id="e2250-104">экземпляры списков;</span><span class="sxs-lookup"><span data-stu-id="e2250-104">List instances</span></span>

> <span data-ttu-id="e2250-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e2250-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2250-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2250-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2250-p103">Получение экземпляров события в течение заданного диапазона времени. Если событие относится к типу `SeriesMaster`, возвращаются экземпляры и исключения события в рамках указанного диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="e2250-p103">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2250-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2250-109">Permissions</span></span>
<span data-ttu-id="e2250-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2250-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2250-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2250-112">Permission type</span></span>      | <span data-ttu-id="e2250-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2250-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2250-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2250-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e2250-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e2250-115">Calendars.Read</span></span>    |
|<span data-ttu-id="e2250-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2250-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2250-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e2250-117">Calendars.Read</span></span>    |
|<span data-ttu-id="e2250-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2250-118">Application</span></span> | <span data-ttu-id="e2250-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e2250-119">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2250-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2250-120">HTTP request</span></span>
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
## <a name="query-parameters"></a><span data-ttu-id="e2250-121">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="e2250-121">Query parameters</span></span>

<span data-ttu-id="e2250-122">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="e2250-122">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="e2250-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="e2250-123">Parameter</span></span>    | <span data-ttu-id="e2250-124">Тип</span><span class="sxs-lookup"><span data-stu-id="e2250-124">Type</span></span>   |<span data-ttu-id="e2250-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e2250-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2250-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e2250-126">startDateTime</span></span>|<span data-ttu-id="e2250-127">String</span><span class="sxs-lookup"><span data-stu-id="e2250-127">String</span></span>|<span data-ttu-id="e2250-p105">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="e2250-p105">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="e2250-130">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e2250-130">endDateTime</span></span>|<span data-ttu-id="e2250-131">String</span><span class="sxs-lookup"><span data-stu-id="e2250-131">String</span></span>|<span data-ttu-id="e2250-p106">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="e2250-p106">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="e2250-134">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e2250-134">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e2250-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2250-135">Request headers</span></span>
| <span data-ttu-id="e2250-136">Имя</span><span class="sxs-lookup"><span data-stu-id="e2250-136">Name</span></span>       | <span data-ttu-id="e2250-137">Тип</span><span class="sxs-lookup"><span data-stu-id="e2250-137">Type</span></span> | <span data-ttu-id="e2250-138">Описание</span><span class="sxs-lookup"><span data-stu-id="e2250-138">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="e2250-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2250-139">Authorization</span></span>  | <span data-ttu-id="e2250-140">string</span><span class="sxs-lookup"><span data-stu-id="e2250-140">string</span></span> | <span data-ttu-id="e2250-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2250-p107">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e2250-143">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="e2250-143">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="e2250-144">string</span><span class="sxs-lookup"><span data-stu-id="e2250-144">string</span></span> | <span data-ttu-id="e2250-145">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="e2250-145">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="e2250-146">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="e2250-146">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="e2250-147">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e2250-147">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2250-148">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e2250-148">Request body</span></span>
<span data-ttu-id="e2250-149">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2250-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2250-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2250-150">Response</span></span>

<span data-ttu-id="e2250-151">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e2250-151">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e2250-152">Пример</span><span class="sxs-lookup"><span data-stu-id="e2250-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2250-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2250-153">Request</span></span>
<span data-ttu-id="e2250-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2250-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="e2250-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2250-155">Response</span></span>
<span data-ttu-id="e2250-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e2250-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "",
        "time": "2016-10-19T10:37:00Z"
      },
      "uid": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
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
  "tocPath": ""
}-->
