---
title: Список событий
description: Получение списка событий в календаре.  Этот список содержит собрания с одним экземпляром и образцы рядов.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 7d3f4110b33cb401126200eadc57c14fef379f9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814233"
---
# <a name="list-events"></a><span data-ttu-id="d30be-104">Список событий</span><span class="sxs-lookup"><span data-stu-id="d30be-104">List events</span></span>

> <span data-ttu-id="d30be-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d30be-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d30be-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d30be-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d30be-p103">Получение списка событий в календаре.  Этот список содержит собрания с одним экземпляром и образцы рядов.</span><span class="sxs-lookup"><span data-stu-id="d30be-p103">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="d30be-109">Чтобы получить расширенные экземпляры события, вы можете [получить представление календаря](calendar-list-calendarview.md) или [экземпляры события](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="d30be-109">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d30be-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d30be-110">Permissions</span></span>
<span data-ttu-id="d30be-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d30be-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d30be-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d30be-113">Permission type</span></span>      | <span data-ttu-id="d30be-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d30be-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d30be-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d30be-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d30be-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d30be-116">Calendars.Read</span></span>    |
|<span data-ttu-id="d30be-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d30be-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d30be-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d30be-118">Calendars.Read</span></span>    |
|<span data-ttu-id="d30be-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d30be-119">Application</span></span> | <span data-ttu-id="d30be-120">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d30be-120">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d30be-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d30be-121">HTTP request</span></span>
<span data-ttu-id="d30be-122"><!-- { "blockType": "ignored" } -->Пользователя или группы по умолчанию [календаря](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="d30be-122"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="d30be-123">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="d30be-123">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="d30be-124">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="d30be-124">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d30be-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d30be-125">Optional query parameters</span></span>
<span data-ttu-id="d30be-126">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d30be-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d30be-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d30be-127">Request headers</span></span>
| <span data-ttu-id="d30be-128">Имя</span><span class="sxs-lookup"><span data-stu-id="d30be-128">Name</span></span>       | <span data-ttu-id="d30be-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d30be-129">Type</span></span> | <span data-ttu-id="d30be-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d30be-130">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="d30be-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="d30be-131">Authorization</span></span>  | <span data-ttu-id="d30be-132">string</span><span class="sxs-lookup"><span data-stu-id="d30be-132">string</span></span> | <span data-ttu-id="d30be-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d30be-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d30be-135">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="d30be-135">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="d30be-136">string</span><span class="sxs-lookup"><span data-stu-id="d30be-136">string</span></span> | <span data-ttu-id="d30be-137">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="d30be-137">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="d30be-138">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="d30be-138">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="d30be-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d30be-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d30be-140">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d30be-140">Request body</span></span>
<span data-ttu-id="d30be-141">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d30be-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d30be-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d30be-142">Response</span></span>

<span data-ttu-id="d30be-143">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d30be-143">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d30be-144">Пример</span><span class="sxs-lookup"><span data-stu-id="d30be-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d30be-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="d30be-145">Request</span></span>
<span data-ttu-id="d30be-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d30be-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/events
```
##### <a name="response"></a><span data-ttu-id="d30be-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="d30be-147">Response</span></span>
<span data-ttu-id="d30be-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d30be-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
