---
title: Список calendarView
description: Получите вхождения, исключений и отдельные экземпляры событий в представлении календаря, определенные в диапазон времени из календаря по умолчанию пользователя,
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 57c3f184b89db2c0aa983c84db42f7bef1fc5269
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934963"
---
# <a name="list-calendarview"></a><span data-ttu-id="c7c6d-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="c7c6d-103">List calendarView</span></span>

> <span data-ttu-id="c7c6d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7c6d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7c6d-106">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного либо другого календаря пользователя, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-106">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="c7c6d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7c6d-107">Permissions</span></span>
<span data-ttu-id="c7c6d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7c6d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7c6d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7c6d-110">Permission type</span></span>      | <span data-ttu-id="c7c6d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7c6d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7c6d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7c6d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c7c6d-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7c6d-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c7c6d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7c6d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7c6d-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7c6d-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c7c6d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7c6d-116">Application</span></span> | <span data-ttu-id="c7c6d-117">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7c6d-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7c6d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7c6d-118">HTTP request</span></span>
<span data-ttu-id="c7c6d-119">Экземпляр [calendar](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-119">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="c7c6d-120">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="c7c6d-120">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="c7c6d-121">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="c7c6d-121">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="c7c6d-122">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="c7c6d-122">Query parameters</span></span>

<span data-ttu-id="c7c6d-123">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-123">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="c7c6d-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="c7c6d-124">Parameter</span></span>    | <span data-ttu-id="c7c6d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="c7c6d-125">Type</span></span>   |<span data-ttu-id="c7c6d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="c7c6d-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7c6d-127">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c7c6d-127">startDateTime</span></span>|<span data-ttu-id="c7c6d-128">String</span><span class="sxs-lookup"><span data-stu-id="c7c6d-128">String</span></span>|<span data-ttu-id="c7c6d-p103">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="c7c6d-p103">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="c7c6d-131">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c7c6d-131">endDateTime</span></span>|<span data-ttu-id="c7c6d-132">String</span><span class="sxs-lookup"><span data-stu-id="c7c6d-132">String</span></span>|<span data-ttu-id="c7c6d-p104">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="c7c6d-p104">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="c7c6d-135">Этот метод также поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-135">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c7c6d-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7c6d-136">Request headers</span></span>
| <span data-ttu-id="c7c6d-137">Имя</span><span class="sxs-lookup"><span data-stu-id="c7c6d-137">Name</span></span>       | <span data-ttu-id="c7c6d-138">Тип</span><span class="sxs-lookup"><span data-stu-id="c7c6d-138">Type</span></span> | <span data-ttu-id="c7c6d-139">Описание</span><span class="sxs-lookup"><span data-stu-id="c7c6d-139">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="c7c6d-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7c6d-140">Authorization</span></span>  | <span data-ttu-id="c7c6d-141">строка</span><span class="sxs-lookup"><span data-stu-id="c7c6d-141">string</span></span> | <span data-ttu-id="c7c6d-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c7c6d-144">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="c7c6d-144">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="c7c6d-145">строка</span><span class="sxs-lookup"><span data-stu-id="c7c6d-145">string</span></span> | <span data-ttu-id="c7c6d-146">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-146">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="c7c6d-147">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-147">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="c7c6d-148">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-148">Optional.</span></span> |
| <span data-ttu-id="c7c6d-149">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="c7c6d-149">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="c7c6d-150">строка</span><span class="sxs-lookup"><span data-stu-id="c7c6d-150">string</span></span> | <span data-ttu-id="c7c6d-151">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-151">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="c7c6d-152">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="c7c6d-152">Values can be "text" or "html".</span></span> <span data-ttu-id="c7c6d-153">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-153">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="c7c6d-154">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-154">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="c7c6d-155">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7c6d-156">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c7c6d-156">Request body</span></span>
<span data-ttu-id="c7c6d-157">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7c6d-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7c6d-158">Response</span></span>

<span data-ttu-id="c7c6d-159">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-159">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7c6d-160">Пример</span><span class="sxs-lookup"><span data-stu-id="c7c6d-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7c6d-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7c6d-161">Request</span></span>
<span data-ttu-id="c7c6d-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-162">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="c7c6d-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7c6d-163">Response</span></span>
<span data-ttu-id="c7c6d-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c7c6d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
