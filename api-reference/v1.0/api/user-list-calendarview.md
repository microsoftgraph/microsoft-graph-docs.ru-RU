---
title: Список calendarView
description: 'Получите вхождения, исключений и отдельные экземпляры событий в представлении календаря, определенные в диапазон времени из календаря по умолчанию пользователя, '
ms.openlocfilehash: db2c0b4d5fe2b3929aab7c30e00aff0f30dff5b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025274"
---
# <a name="list-calendarview"></a><span data-ttu-id="cfedd-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="cfedd-103">List calendarView</span></span>

<span data-ttu-id="cfedd-104">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного либо другого календаря пользователя, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="cfedd-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="cfedd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cfedd-105">Permissions</span></span>
<span data-ttu-id="cfedd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfedd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfedd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cfedd-108">Permission type</span></span>      | <span data-ttu-id="cfedd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cfedd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfedd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cfedd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cfedd-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfedd-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cfedd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cfedd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfedd-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfedd-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cfedd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cfedd-114">Application</span></span> | <span data-ttu-id="cfedd-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfedd-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfedd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cfedd-116">HTTP request</span></span>

<span data-ttu-id="cfedd-117">Экземпляр [calendar](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="cfedd-117">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="cfedd-118">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="cfedd-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="cfedd-119">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="cfedd-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="cfedd-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="cfedd-120">Query parameters</span></span>

<span data-ttu-id="cfedd-121">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="cfedd-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="cfedd-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="cfedd-122">Parameter</span></span>    | <span data-ttu-id="cfedd-123">Тип</span><span class="sxs-lookup"><span data-stu-id="cfedd-123">Type</span></span>   |<span data-ttu-id="cfedd-124">Описание</span><span class="sxs-lookup"><span data-stu-id="cfedd-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfedd-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cfedd-125">startDateTime</span></span>|<span data-ttu-id="cfedd-126">String</span><span class="sxs-lookup"><span data-stu-id="cfedd-126">String</span></span>|<span data-ttu-id="cfedd-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="cfedd-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="cfedd-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="cfedd-129">endDateTime</span></span>|<span data-ttu-id="cfedd-130">String</span><span class="sxs-lookup"><span data-stu-id="cfedd-130">String</span></span>|<span data-ttu-id="cfedd-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="cfedd-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="cfedd-133">Этот метод также поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cfedd-133">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cfedd-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cfedd-134">Request headers</span></span>
| <span data-ttu-id="cfedd-135">Имя</span><span class="sxs-lookup"><span data-stu-id="cfedd-135">Name</span></span>       | <span data-ttu-id="cfedd-136">Тип</span><span class="sxs-lookup"><span data-stu-id="cfedd-136">Type</span></span> | <span data-ttu-id="cfedd-137">Описание</span><span class="sxs-lookup"><span data-stu-id="cfedd-137">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="cfedd-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfedd-138">Authorization</span></span>  | <span data-ttu-id="cfedd-139">string</span><span class="sxs-lookup"><span data-stu-id="cfedd-139">string</span></span> | <span data-ttu-id="cfedd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfedd-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cfedd-142">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="cfedd-142">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="cfedd-143">string</span><span class="sxs-lookup"><span data-stu-id="cfedd-143">string</span></span> | <span data-ttu-id="cfedd-144">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="cfedd-144">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="cfedd-145">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="cfedd-145">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="cfedd-146">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="cfedd-146">Optional.</span></span> |
| <span data-ttu-id="cfedd-147">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="cfedd-147">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="cfedd-148">string</span><span class="sxs-lookup"><span data-stu-id="cfedd-148">string</span></span> | <span data-ttu-id="cfedd-149">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="cfedd-149">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="cfedd-150">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="cfedd-150">Values can be "text" or "html".</span></span> <span data-ttu-id="cfedd-151">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="cfedd-151">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="cfedd-152">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="cfedd-152">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="cfedd-153">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="cfedd-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfedd-154">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cfedd-154">Request body</span></span>
<span data-ttu-id="cfedd-155">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cfedd-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfedd-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfedd-156">Response</span></span>

<span data-ttu-id="cfedd-157">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cfedd-157">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cfedd-158">Пример</span><span class="sxs-lookup"><span data-stu-id="cfedd-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cfedd-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfedd-159">Request</span></span>
<span data-ttu-id="cfedd-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cfedd-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000 
```
##### <a name="response"></a><span data-ttu-id="cfedd-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="cfedd-161">Response</span></span>
<span data-ttu-id="cfedd-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cfedd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
