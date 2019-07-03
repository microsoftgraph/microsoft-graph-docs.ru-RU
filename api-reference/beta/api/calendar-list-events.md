---
title: Список событий
description: Получение списка событий в календаре. Этот список содержит собрания с одним экземпляром и образцы рядов.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 912388f99e56e71c5828765f7a8169005b772169
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438897"
---
# <a name="list-events"></a><span data-ttu-id="dbd6f-104">Список событий</span><span class="sxs-lookup"><span data-stu-id="dbd6f-104">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbd6f-p102">Получение списка событий в календаре.  Этот список содержит собрания с одним экземпляром и образцы рядов.</span><span class="sxs-lookup"><span data-stu-id="dbd6f-p102">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="dbd6f-107">Чтобы получить расширенные экземпляры события, вы можете [получить представление календаря](calendar-list-calendarview.md) или [экземпляры события](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="dbd6f-107">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dbd6f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dbd6f-108">Permissions</span></span>
<span data-ttu-id="dbd6f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbd6f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbd6f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbd6f-111">Permission type</span></span>      | <span data-ttu-id="dbd6f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbd6f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbd6f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbd6f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dbd6f-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dbd6f-114">Calendars.Read</span></span>    |
|<span data-ttu-id="dbd6f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbd6f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbd6f-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dbd6f-116">Calendars.Read</span></span>    |
|<span data-ttu-id="dbd6f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbd6f-117">Application</span></span> | <span data-ttu-id="dbd6f-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dbd6f-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbd6f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbd6f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="dbd6f-120">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dbd6f-120">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="dbd6f-121">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="dbd6f-121">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="dbd6f-122">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="dbd6f-122">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dbd6f-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dbd6f-123">Optional query parameters</span></span>
<span data-ttu-id="dbd6f-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dbd6f-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dbd6f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbd6f-125">Request headers</span></span>
| <span data-ttu-id="dbd6f-126">Имя</span><span class="sxs-lookup"><span data-stu-id="dbd6f-126">Name</span></span>       | <span data-ttu-id="dbd6f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="dbd6f-127">Type</span></span> | <span data-ttu-id="dbd6f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="dbd6f-128">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="dbd6f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbd6f-129">Authorization</span></span>  | <span data-ttu-id="dbd6f-130">string</span><span class="sxs-lookup"><span data-stu-id="dbd6f-130">string</span></span> | <span data-ttu-id="dbd6f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dbd6f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dbd6f-133">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="dbd6f-133">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="dbd6f-134">string</span><span class="sxs-lookup"><span data-stu-id="dbd6f-134">string</span></span> | <span data-ttu-id="dbd6f-135">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="dbd6f-135">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="dbd6f-136">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="dbd6f-136">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="dbd6f-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="dbd6f-137">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbd6f-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dbd6f-138">Request body</span></span>
<span data-ttu-id="dbd6f-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dbd6f-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbd6f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbd6f-140">Response</span></span>

<span data-ttu-id="dbd6f-141">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dbd6f-141">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dbd6f-142">Пример</span><span class="sxs-lookup"><span data-stu-id="dbd6f-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dbd6f-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbd6f-143">Request</span></span>
<span data-ttu-id="dbd6f-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbd6f-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dbd6f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbd6f-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/events
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dbd6f-146">C#</span><span class="sxs-lookup"><span data-stu-id="dbd6f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dbd6f-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="dbd6f-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dbd6f-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dbd6f-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dbd6f-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbd6f-149">Response</span></span>
<span data-ttu-id="dbd6f-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dbd6f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
  ]
}
-->
