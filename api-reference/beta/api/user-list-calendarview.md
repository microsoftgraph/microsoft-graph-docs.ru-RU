---
title: Список calendarView
description: Получите вхождения, исключений и отдельные экземпляры событий в представлении календаря, определенные в диапазон времени из календаря по умолчанию пользователя,
localization_priority: Normal
ms.openlocfilehash: 8db54c6ad12254957fd2c95509ddbebd34813906
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876078"
---
# <a name="list-calendarview"></a><span data-ttu-id="94b5e-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="94b5e-103">List calendarView</span></span>

> <span data-ttu-id="94b5e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="94b5e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94b5e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94b5e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94b5e-106">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного либо другого календаря пользователя, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="94b5e-106">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="94b5e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94b5e-107">Permissions</span></span>
<span data-ttu-id="94b5e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94b5e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94b5e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94b5e-110">Permission type</span></span>      | <span data-ttu-id="94b5e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94b5e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94b5e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94b5e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="94b5e-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94b5e-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="94b5e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94b5e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94b5e-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94b5e-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="94b5e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94b5e-116">Application</span></span> | <span data-ttu-id="94b5e-117">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94b5e-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="94b5e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94b5e-118">HTTP request</span></span>
<span data-ttu-id="94b5e-119">Экземпляр [calendar](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="94b5e-119">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="94b5e-120">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="94b5e-120">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="94b5e-121">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="94b5e-121">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="94b5e-122">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="94b5e-122">Query parameters</span></span>

<span data-ttu-id="94b5e-123">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="94b5e-123">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="94b5e-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="94b5e-124">Parameter</span></span>    | <span data-ttu-id="94b5e-125">Тип</span><span class="sxs-lookup"><span data-stu-id="94b5e-125">Type</span></span>   |<span data-ttu-id="94b5e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="94b5e-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94b5e-127">startDateTime</span><span class="sxs-lookup"><span data-stu-id="94b5e-127">startDateTime</span></span>|<span data-ttu-id="94b5e-128">String</span><span class="sxs-lookup"><span data-stu-id="94b5e-128">String</span></span>|<span data-ttu-id="94b5e-p103">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="94b5e-p103">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="94b5e-131">endDateTime</span><span class="sxs-lookup"><span data-stu-id="94b5e-131">endDateTime</span></span>|<span data-ttu-id="94b5e-132">String</span><span class="sxs-lookup"><span data-stu-id="94b5e-132">String</span></span>|<span data-ttu-id="94b5e-p104">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="94b5e-p104">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="94b5e-135">Этот метод также поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="94b5e-135">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="94b5e-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94b5e-136">Request headers</span></span>
| <span data-ttu-id="94b5e-137">Имя</span><span class="sxs-lookup"><span data-stu-id="94b5e-137">Name</span></span>       | <span data-ttu-id="94b5e-138">Тип</span><span class="sxs-lookup"><span data-stu-id="94b5e-138">Type</span></span> | <span data-ttu-id="94b5e-139">Описание</span><span class="sxs-lookup"><span data-stu-id="94b5e-139">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="94b5e-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="94b5e-140">Authorization</span></span>  | <span data-ttu-id="94b5e-141">string</span><span class="sxs-lookup"><span data-stu-id="94b5e-141">string</span></span> | <span data-ttu-id="94b5e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94b5e-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="94b5e-144">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="94b5e-144">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="94b5e-145">string</span><span class="sxs-lookup"><span data-stu-id="94b5e-145">string</span></span> | <span data-ttu-id="94b5e-146">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="94b5e-146">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="94b5e-147">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="94b5e-147">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="94b5e-148">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="94b5e-148">Optional.</span></span> |
| <span data-ttu-id="94b5e-149">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="94b5e-149">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="94b5e-150">string</span><span class="sxs-lookup"><span data-stu-id="94b5e-150">string</span></span> | <span data-ttu-id="94b5e-151">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="94b5e-151">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="94b5e-152">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="94b5e-152">Values can be "text" or "html".</span></span> <span data-ttu-id="94b5e-153">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="94b5e-153">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="94b5e-154">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="94b5e-154">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="94b5e-155">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="94b5e-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94b5e-156">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="94b5e-156">Request body</span></span>
<span data-ttu-id="94b5e-157">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94b5e-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94b5e-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="94b5e-158">Response</span></span>

<span data-ttu-id="94b5e-159">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="94b5e-159">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94b5e-160">Пример</span><span class="sxs-lookup"><span data-stu-id="94b5e-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94b5e-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="94b5e-161">Request</span></span>
<span data-ttu-id="94b5e-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94b5e-162">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="94b5e-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="94b5e-163">Response</span></span>
<span data-ttu-id="94b5e-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="94b5e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List calendarView",
  "keywords": "calendar",
  "section": "documentation",
  "tocPath": ""
}-->
