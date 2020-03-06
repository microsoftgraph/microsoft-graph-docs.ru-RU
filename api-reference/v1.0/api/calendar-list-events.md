---
title: Список событий
description: Получение списка событий в календаре. Этот список содержит собрания с одним экземпляром и образцы рядов.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0b21a267c79fbde4c2a2f0099446206e9c5d2bd4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518800"
---
# <a name="list-events"></a><span data-ttu-id="573af-104">Перечисление событий</span><span class="sxs-lookup"><span data-stu-id="573af-104">List events</span></span>

<span data-ttu-id="573af-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="573af-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="573af-106">Получение списка событий в календаре.</span><span class="sxs-lookup"><span data-stu-id="573af-106">Retrieve a list of events in a calendar.</span></span>  <span data-ttu-id="573af-107">Это может быть календарь для ресурса [user](../resources/user.md) или стандартный календарь для ресурса [group](../resources/group.md), представляющего группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="573af-107">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span> <span data-ttu-id="573af-108">В этом списке указаны единичные собрания и главные собрания в соответствующих рядах.</span><span class="sxs-lookup"><span data-stu-id="573af-108">The list of events contains single instance meetings and series masters.</span></span>

<span data-ttu-id="573af-109">Чтобы получить расширенные экземпляры события, вы можете [получить представление календаря](calendar-list-calendarview.md) или [экземпляры события](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="573af-109">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="573af-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="573af-110">Permissions</span></span>
<span data-ttu-id="573af-111">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="573af-111">Depending on the type of calendar that the events are in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="573af-112">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="573af-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="573af-113">Календарь</span><span class="sxs-lookup"><span data-stu-id="573af-113">Calendar</span></span> | <span data-ttu-id="573af-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="573af-114">Delegated (work or school account)</span></span> | <span data-ttu-id="573af-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="573af-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="573af-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="573af-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="573af-117">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="573af-117">user calendar</span></span> | <span data-ttu-id="573af-118">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="573af-118">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="573af-119">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="573af-119">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="573af-120">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="573af-120">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="573af-121">календарь группы</span><span class="sxs-lookup"><span data-stu-id="573af-121">group calendar</span></span> | <span data-ttu-id="573af-122">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="573af-122">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="573af-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="573af-123">Not supported.</span></span> | <span data-ttu-id="573af-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="573af-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="573af-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="573af-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="573af-126">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="573af-126">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="573af-127">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="573af-127">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="573af-128">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="573af-128">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="573af-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="573af-129">Optional query parameters</span></span>
<span data-ttu-id="573af-130">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="573af-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="573af-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="573af-131">Request headers</span></span>
| <span data-ttu-id="573af-132">Имя</span><span class="sxs-lookup"><span data-stu-id="573af-132">Name</span></span>       | <span data-ttu-id="573af-133">Тип</span><span class="sxs-lookup"><span data-stu-id="573af-133">Type</span></span> | <span data-ttu-id="573af-134">Описание</span><span class="sxs-lookup"><span data-stu-id="573af-134">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="573af-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="573af-135">Authorization</span></span>  | <span data-ttu-id="573af-136">string</span><span class="sxs-lookup"><span data-stu-id="573af-136">string</span></span> | <span data-ttu-id="573af-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="573af-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="573af-139">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="573af-139">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="573af-140">string</span><span class="sxs-lookup"><span data-stu-id="573af-140">string</span></span> | <span data-ttu-id="573af-141">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="573af-141">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="573af-142">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="573af-142">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="573af-143">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="573af-143">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="573af-144">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="573af-144">Request body</span></span>
<span data-ttu-id="573af-145">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="573af-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="573af-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="573af-146">Response</span></span>

<span data-ttu-id="573af-147">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="573af-147">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="573af-148">Пример</span><span class="sxs-lookup"><span data-stu-id="573af-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="573af-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="573af-149">Request</span></span>
<span data-ttu-id="573af-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="573af-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="573af-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="573af-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendar_get_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar/events
```
# <a name="c"></a>[<span data-ttu-id="573af-152">C#</span><span class="sxs-lookup"><span data-stu-id="573af-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="573af-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="573af-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="573af-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="573af-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="573af-155">Java</span><span class="sxs-lookup"><span data-stu-id="573af-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendar-get-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="573af-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="573af-156">Response</span></span>
<span data-ttu-id="573af-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="573af-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
