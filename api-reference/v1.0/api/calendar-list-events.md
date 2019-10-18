---
title: Список событий
description: Получение списка событий в календаре. Этот список содержит собрания с одним экземпляром и образцы рядов.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fe16c1c586277967e8de41a67a92f851dc4e1b7d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726517"
---
# <a name="list-events"></a><span data-ttu-id="276a0-104">Перечисление событий</span><span class="sxs-lookup"><span data-stu-id="276a0-104">List events</span></span>

<span data-ttu-id="276a0-105">Получение списка событий в календаре.</span><span class="sxs-lookup"><span data-stu-id="276a0-105">Retrieve a list of events in a calendar.</span></span>  <span data-ttu-id="276a0-106">Это может быть календарь для ресурса [user](../resources/user.md) или стандартный календарь для ресурса [group](../resources/group.md), представляющего группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="276a0-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span> <span data-ttu-id="276a0-107">В этом списке указаны единичные собрания и главные собрания в соответствующих рядах.</span><span class="sxs-lookup"><span data-stu-id="276a0-107">The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="276a0-108">Чтобы получить расширенные экземпляры события, вы можете [получить представление календаря](calendar-list-calendarview.md) или [экземпляры события](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="276a0-108">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="276a0-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="276a0-109">Permissions</span></span>
<span data-ttu-id="276a0-110">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="276a0-110">Depending on the type of calendar that the events are in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="276a0-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="276a0-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="276a0-112">Календарь</span><span class="sxs-lookup"><span data-stu-id="276a0-112">Calendar</span></span> | <span data-ttu-id="276a0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="276a0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="276a0-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="276a0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="276a0-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="276a0-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="276a0-116">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="276a0-116">user calendar</span></span> | <span data-ttu-id="276a0-117">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="276a0-117">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="276a0-118">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="276a0-118">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="276a0-119">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="276a0-119">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="276a0-120">календарь группы</span><span class="sxs-lookup"><span data-stu-id="276a0-120">group calendar</span></span> | <span data-ttu-id="276a0-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="276a0-121">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="276a0-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="276a0-122">Not supported.</span></span> | <span data-ttu-id="276a0-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="276a0-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="276a0-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="276a0-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="276a0-125">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="276a0-125">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="276a0-126">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="276a0-126">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="276a0-127">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="276a0-127">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="276a0-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="276a0-128">Optional query parameters</span></span>
<span data-ttu-id="276a0-129">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="276a0-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="276a0-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="276a0-130">Request headers</span></span>
| <span data-ttu-id="276a0-131">Имя</span><span class="sxs-lookup"><span data-stu-id="276a0-131">Name</span></span>       | <span data-ttu-id="276a0-132">Тип</span><span class="sxs-lookup"><span data-stu-id="276a0-132">Type</span></span> | <span data-ttu-id="276a0-133">Описание</span><span class="sxs-lookup"><span data-stu-id="276a0-133">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="276a0-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="276a0-134">Authorization</span></span>  | <span data-ttu-id="276a0-135">string</span><span class="sxs-lookup"><span data-stu-id="276a0-135">string</span></span> | <span data-ttu-id="276a0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="276a0-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="276a0-138">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="276a0-138">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="276a0-139">string</span><span class="sxs-lookup"><span data-stu-id="276a0-139">string</span></span> | <span data-ttu-id="276a0-140">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="276a0-140">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="276a0-141">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="276a0-141">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="276a0-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="276a0-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="276a0-143">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="276a0-143">Request body</span></span>
<span data-ttu-id="276a0-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="276a0-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="276a0-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="276a0-145">Response</span></span>

<span data-ttu-id="276a0-146">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="276a0-146">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="276a0-147">Пример</span><span class="sxs-lookup"><span data-stu-id="276a0-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="276a0-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="276a0-148">Request</span></span>
<span data-ttu-id="276a0-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="276a0-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="276a0-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="276a0-150">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendar_get_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar/events
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="276a0-151">C#</span><span class="sxs-lookup"><span data-stu-id="276a0-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="276a0-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="276a0-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="276a0-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="276a0-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="276a0-154">Java</span><span class="sxs-lookup"><span data-stu-id="276a0-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendar-get-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="276a0-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="276a0-155">Response</span></span>
<span data-ttu-id="276a0-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="276a0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
