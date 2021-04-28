---
title: Список событий
description: Получение списка событий в календаре. Этот список содержит собрания с одним экземпляром и образцы рядов.
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 33bdadb28129183972f8fb6f7ee051708a3f2e55
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054604"
---
# <a name="list-events"></a><span data-ttu-id="ddffd-104">Перечисление событий</span><span class="sxs-lookup"><span data-stu-id="ddffd-104">List events</span></span>

<span data-ttu-id="ddffd-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddffd-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ddffd-106">Получение списка событий в календаре.</span><span class="sxs-lookup"><span data-stu-id="ddffd-106">Retrieve a list of events in a calendar.</span></span>  <span data-ttu-id="ddffd-107">Это может быть календарь для [пользователя](../resources/user.md) или стандартный календарь для [группы](../resources/group.md) Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ddffd-107">The calendar can be one for a [user](../resources/user.md), or the default calendar of a Microsoft 365 [group](../resources/group.md).</span></span> <span data-ttu-id="ddffd-108">В этом списке указаны единичные собрания и главные собрания в соответствующих рядах.</span><span class="sxs-lookup"><span data-stu-id="ddffd-108">The list of events contains single instance meetings and series masters.</span></span>

<span data-ttu-id="ddffd-109">Чтобы получить расширенные экземпляры события, вы можете [получить представление календаря](calendar-list-calendarview.md) или [экземпляры события](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="ddffd-109">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ddffd-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ddffd-110">Permissions</span></span>
<span data-ttu-id="ddffd-111">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="ddffd-111">Depending on the type of calendar that the events are in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="ddffd-112">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddffd-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ddffd-113">Календарь</span><span class="sxs-lookup"><span data-stu-id="ddffd-113">Calendar</span></span> | <span data-ttu-id="ddffd-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddffd-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ddffd-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddffd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddffd-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ddffd-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="ddffd-117">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="ddffd-117">user calendar</span></span> | <span data-ttu-id="ddffd-118">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddffd-118">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="ddffd-119">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddffd-119">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="ddffd-120">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddffd-120">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="ddffd-121">календарь группы</span><span class="sxs-lookup"><span data-stu-id="ddffd-121">group calendar</span></span> | <span data-ttu-id="ddffd-122">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddffd-122">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="ddffd-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddffd-123">Not supported.</span></span> | <span data-ttu-id="ddffd-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddffd-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddffd-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddffd-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="ddffd-126">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ddffd-126">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="ddffd-127">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="ddffd-127">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events
```
<span data-ttu-id="ddffd-128">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="ddffd-128">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ddffd-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ddffd-129">Optional query parameters</span></span>
<span data-ttu-id="ddffd-130">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ddffd-130">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ddffd-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddffd-131">Request headers</span></span>
| <span data-ttu-id="ddffd-132">Имя</span><span class="sxs-lookup"><span data-stu-id="ddffd-132">Name</span></span>       | <span data-ttu-id="ddffd-133">Тип</span><span class="sxs-lookup"><span data-stu-id="ddffd-133">Type</span></span> | <span data-ttu-id="ddffd-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ddffd-134">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="ddffd-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddffd-135">Authorization</span></span>  | <span data-ttu-id="ddffd-136">string</span><span class="sxs-lookup"><span data-stu-id="ddffd-136">string</span></span> | <span data-ttu-id="ddffd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddffd-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ddffd-139">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="ddffd-139">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="ddffd-140">string</span><span class="sxs-lookup"><span data-stu-id="ddffd-140">string</span></span> | <span data-ttu-id="ddffd-p105">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в отклике. Если он не задан, эти значения времени возвращаются в формате UTC. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="ddffd-p105">Use this to specify the time zone for start and end times in the response. If not specified, those time values are returned in UTC. Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddffd-144">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddffd-144">Request body</span></span>
<span data-ttu-id="ddffd-145">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ddffd-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddffd-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddffd-146">Response</span></span>

<span data-ttu-id="ddffd-147">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ddffd-147">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ddffd-148">Пример</span><span class="sxs-lookup"><span data-stu-id="ddffd-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ddffd-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddffd-149">Request</span></span>
<span data-ttu-id="ddffd-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddffd-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ddffd-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddffd-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendar_get_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar/events
```
# <a name="c"></a>[<span data-ttu-id="ddffd-152">C#</span><span class="sxs-lookup"><span data-stu-id="ddffd-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddffd-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddffd-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddffd-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddffd-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ddffd-155">Java</span><span class="sxs-lookup"><span data-stu-id="ddffd-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendar-get-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ddffd-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddffd-156">Response</span></span>
<span data-ttu-id="ddffd-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ddffd-157">Here is an example of the response.</span></span> <span data-ttu-id="ddffd-158">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ddffd-158">Note: The response object shown here might be shortened for readability.</span></span>
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
