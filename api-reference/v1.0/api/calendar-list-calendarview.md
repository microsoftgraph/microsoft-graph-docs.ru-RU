---
title: Список calendarView
description: Получение исключений, повторяемых или единичных экземпляров событий в представлении календаря, которое определяется заданным диапазоном времени,
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 5f3b3c263ffd4f4a7a2a4663b087527791685573
ms.sourcegitcommit: b198efc2391a12a840e4f1b8c42c18a55b06037f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2019
ms.locfileid: "35820663"
---
# <a name="list-calendarview"></a><span data-ttu-id="51477-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="51477-103">List calendarView</span></span>

<span data-ttu-id="51477-104">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря `(../me/calendarview)`, принадлежащего пользователю или группе, либо другого календаря пользователя, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="51477-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="51477-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51477-105">Permissions</span></span>
<span data-ttu-id="51477-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51477-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="51477-108">События в календаре пользователя: Calendars.Read или Calendars.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="51477-108">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="51477-109">События в календаре группы: Group.Read.All или Group.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="51477-109">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="51477-110">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51477-110">HTTP request</span></span>

<span data-ttu-id="51477-111">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="51477-111">A user's or group's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="51477-112">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="51477-112">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="51477-113">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="51477-113">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="51477-114">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="51477-114">Query parameters</span></span>

<span data-ttu-id="51477-115">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="51477-115">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="51477-116">Параметр</span><span class="sxs-lookup"><span data-stu-id="51477-116">Parameter</span></span>    | <span data-ttu-id="51477-117">Тип</span><span class="sxs-lookup"><span data-stu-id="51477-117">Type</span></span>   |<span data-ttu-id="51477-118">Описание</span><span class="sxs-lookup"><span data-stu-id="51477-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51477-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="51477-119">startDateTime</span></span>|<span data-ttu-id="51477-120">String</span><span class="sxs-lookup"><span data-stu-id="51477-120">String</span></span>|<span data-ttu-id="51477-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="51477-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="51477-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="51477-123">endDateTime</span></span>|<span data-ttu-id="51477-124">String</span><span class="sxs-lookup"><span data-stu-id="51477-124">String</span></span>|<span data-ttu-id="51477-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="51477-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="51477-127">Этот метод также поддерживает некоторые [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="51477-127">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE] 
> <span data-ttu-id="51477-128">Свойства **createdDateTime** и **lastModifiedDateTime** [события](../resources/event.md) не поддерживают `$select`.</span><span class="sxs-lookup"><span data-stu-id="51477-128">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="51477-129">Чтобы получить их значения, просто запросите **calendarView**, не применяя `$select`.</span><span class="sxs-lookup"><span data-stu-id="51477-129">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51477-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51477-130">Request headers</span></span>
| <span data-ttu-id="51477-131">Имя</span><span class="sxs-lookup"><span data-stu-id="51477-131">Name</span></span>       | <span data-ttu-id="51477-132">Тип</span><span class="sxs-lookup"><span data-stu-id="51477-132">Type</span></span> | <span data-ttu-id="51477-133">Описание</span><span class="sxs-lookup"><span data-stu-id="51477-133">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="51477-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="51477-134">Authorization</span></span>  | <span data-ttu-id="51477-135">string</span><span class="sxs-lookup"><span data-stu-id="51477-135">string</span></span> | <span data-ttu-id="51477-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51477-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="51477-138">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="51477-138">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="51477-139">string</span><span class="sxs-lookup"><span data-stu-id="51477-139">string</span></span> | <span data-ttu-id="51477-140">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="51477-140">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="51477-141">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="51477-141">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="51477-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="51477-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51477-143">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51477-143">Request body</span></span>
<span data-ttu-id="51477-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51477-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51477-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="51477-145">Response</span></span>

<span data-ttu-id="51477-146">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="51477-146">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="51477-147">Пример</span><span class="sxs-lookup"><span data-stu-id="51477-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51477-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="51477-148">Request</span></span>
<span data-ttu-id="51477-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51477-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="51477-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="51477-150">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="51477-151">C#</span><span class="sxs-lookup"><span data-stu-id="51477-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="51477-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51477-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="51477-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51477-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="51477-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="51477-154">Response</span></span>
<span data-ttu-id="51477-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51477-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "response": "response-value",
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
