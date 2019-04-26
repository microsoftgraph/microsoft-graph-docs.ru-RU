---
title: Список событий
description: Получение списка событий в календаре. Этот список содержит собрания с одним экземпляром и образцы рядов.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f229960ee5fc8f0541fb3c1b91f02ddc9b0a28c6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570598"
---
# <a name="list-events"></a><span data-ttu-id="81634-104">Список событий</span><span class="sxs-lookup"><span data-stu-id="81634-104">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81634-p102">Получение списка событий в календаре.  Этот список содержит собрания с одним экземпляром и образцы рядов.</span><span class="sxs-lookup"><span data-stu-id="81634-p102">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="81634-107">Чтобы получить расширенные экземпляры события, вы можете [получить представление календаря](calendar-list-calendarview.md) или [экземпляры события](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="81634-107">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="81634-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81634-108">Permissions</span></span>
<span data-ttu-id="81634-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81634-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81634-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81634-111">Permission type</span></span>      | <span data-ttu-id="81634-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81634-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81634-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81634-113">Delegated (work or school account)</span></span> | <span data-ttu-id="81634-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="81634-114">Calendars.Read</span></span>    |
|<span data-ttu-id="81634-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81634-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81634-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="81634-116">Calendars.Read</span></span>    |
|<span data-ttu-id="81634-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81634-117">Application</span></span> | <span data-ttu-id="81634-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="81634-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="81634-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81634-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="81634-120">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="81634-120">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="81634-121">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="81634-121">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="81634-122">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="81634-122">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="81634-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="81634-123">Optional query parameters</span></span>
<span data-ttu-id="81634-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="81634-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="81634-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81634-125">Request headers</span></span>
| <span data-ttu-id="81634-126">Имя</span><span class="sxs-lookup"><span data-stu-id="81634-126">Name</span></span>       | <span data-ttu-id="81634-127">Тип</span><span class="sxs-lookup"><span data-stu-id="81634-127">Type</span></span> | <span data-ttu-id="81634-128">Описание</span><span class="sxs-lookup"><span data-stu-id="81634-128">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="81634-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="81634-129">Authorization</span></span>  | <span data-ttu-id="81634-130">string</span><span class="sxs-lookup"><span data-stu-id="81634-130">string</span></span> | <span data-ttu-id="81634-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81634-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="81634-133">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="81634-133">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="81634-134">string</span><span class="sxs-lookup"><span data-stu-id="81634-134">string</span></span> | <span data-ttu-id="81634-135">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="81634-135">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="81634-136">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="81634-136">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="81634-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="81634-137">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81634-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="81634-138">Request body</span></span>
<span data-ttu-id="81634-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="81634-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81634-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="81634-140">Response</span></span>

<span data-ttu-id="81634-141">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="81634-141">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="81634-142">Пример</span><span class="sxs-lookup"><span data-stu-id="81634-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81634-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="81634-143">Request</span></span>
<span data-ttu-id="81634-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81634-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/events
```
##### <a name="response"></a><span data-ttu-id="81634-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="81634-145">Response</span></span>
<span data-ttu-id="81634-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="81634-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
