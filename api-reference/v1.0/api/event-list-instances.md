---
title: Список экземпляров
description: 'Получение экземпляров (вхождений) события для заданного интервала времени. Если событие `SeriesMaster` типа, при этом будет получен '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6e18572a0c9f8d7d20ad8f3740559d645e4fa9e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977019"
---
# <a name="list-instances"></a><span data-ttu-id="c0159-104">Список экземпляров</span><span class="sxs-lookup"><span data-stu-id="c0159-104">List instances</span></span>

<span data-ttu-id="c0159-p102">Получение экземпляров события в течение заданного диапазона времени. Если событие относится к типу `SeriesMaster`, возвращаются экземпляры и исключения события в рамках указанного диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="c0159-p102">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0159-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0159-107">Permissions</span></span>
<span data-ttu-id="c0159-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0159-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0159-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0159-110">Permission type</span></span>      | <span data-ttu-id="c0159-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0159-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0159-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0159-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c0159-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c0159-113">Calendars.Read</span></span>    |
|<span data-ttu-id="c0159-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0159-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0159-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c0159-115">Calendars.Read</span></span>    |
|<span data-ttu-id="c0159-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0159-116">Application</span></span> | <span data-ttu-id="c0159-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c0159-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0159-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0159-118">HTTP request</span></span>
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
## <a name="query-parameters"></a><span data-ttu-id="c0159-119">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="c0159-119">Query parameters</span></span>

<span data-ttu-id="c0159-120">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="c0159-120">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="c0159-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="c0159-121">Parameter</span></span>    | <span data-ttu-id="c0159-122">Тип</span><span class="sxs-lookup"><span data-stu-id="c0159-122">Type</span></span>   |<span data-ttu-id="c0159-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c0159-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0159-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c0159-124">startDateTime</span></span>|<span data-ttu-id="c0159-125">String</span><span class="sxs-lookup"><span data-stu-id="c0159-125">String</span></span>|<span data-ttu-id="c0159-p104">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="c0159-p104">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="c0159-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c0159-128">endDateTime</span></span>|<span data-ttu-id="c0159-129">String</span><span class="sxs-lookup"><span data-stu-id="c0159-129">String</span></span>|<span data-ttu-id="c0159-p105">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="c0159-p105">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="c0159-132">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c0159-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c0159-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0159-133">Request headers</span></span>
| <span data-ttu-id="c0159-134">Имя</span><span class="sxs-lookup"><span data-stu-id="c0159-134">Name</span></span>       | <span data-ttu-id="c0159-135">Тип</span><span class="sxs-lookup"><span data-stu-id="c0159-135">Type</span></span> | <span data-ttu-id="c0159-136">Описание</span><span class="sxs-lookup"><span data-stu-id="c0159-136">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="c0159-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0159-137">Authorization</span></span>  | <span data-ttu-id="c0159-138">строка</span><span class="sxs-lookup"><span data-stu-id="c0159-138">string</span></span> | <span data-ttu-id="c0159-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0159-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c0159-141">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="c0159-141">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="c0159-142">строка</span><span class="sxs-lookup"><span data-stu-id="c0159-142">string</span></span> | <span data-ttu-id="c0159-143">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="c0159-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="c0159-144">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c0159-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="c0159-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c0159-145">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0159-146">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c0159-146">Request body</span></span>
<span data-ttu-id="c0159-147">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0159-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0159-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0159-148">Response</span></span>

<span data-ttu-id="c0159-149">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c0159-149">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0159-150">Пример</span><span class="sxs-lookup"><span data-stu-id="c0159-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0159-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0159-151">Request</span></span>
<span data-ttu-id="c0159-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0159-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="c0159-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0159-153">Response</span></span>
<span data-ttu-id="c0159-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c0159-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
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
