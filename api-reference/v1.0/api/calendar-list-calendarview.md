---
title: Список calendarView
description: Получение исключений, повторяемых или единичных экземпляров событий в представлении календаря, которое определяется заданным диапазоном времени,
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f965f3686215d423bcf92744708ba83a6186a66c
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459909"
---
# <a name="list-calendarview"></a><span data-ttu-id="682de-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="682de-103">List calendarView</span></span>

<span data-ttu-id="682de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="682de-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="682de-105">Получение в представлении календаря исключений, повторяемых или единичных экземпляров событий за определенный диапазон времени, указанных в стандартном `(../me/calendarview)` или любом другом календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="682de-105">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from a user's default calendar `(../me/calendarview)` or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="682de-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="682de-106">Permissions</span></span>
<span data-ttu-id="682de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="682de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="682de-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="682de-109">Permission type</span></span>      | <span data-ttu-id="682de-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="682de-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="682de-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="682de-111">Delegated (work or school account)</span></span> | <span data-ttu-id="682de-112">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="682de-112">Calendars.Read, Calendars.ReadWrite</span></span> |
|<span data-ttu-id="682de-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="682de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="682de-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="682de-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="682de-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="682de-115">Application</span></span> | <span data-ttu-id="682de-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="682de-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="682de-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="682de-117">HTTP request</span></span>

<span data-ttu-id="682de-118">Экземпляр [calendar](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="682de-118">A user's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="682de-119">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="682de-119">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="682de-120">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="682de-120">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="682de-121">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="682de-121">Query parameters</span></span>

<span data-ttu-id="682de-122">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="682de-122">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="682de-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="682de-123">Parameter</span></span>     | <span data-ttu-id="682de-124">Тип</span><span class="sxs-lookup"><span data-stu-id="682de-124">Type</span></span>   | <span data-ttu-id="682de-125">Описание</span><span class="sxs-lookup"><span data-stu-id="682de-125">Description</span></span>                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="682de-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="682de-126">startDateTime</span></span> | <span data-ttu-id="682de-127">String</span><span class="sxs-lookup"><span data-stu-id="682de-127">String</span></span> | <span data-ttu-id="682de-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2019-11-08T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="682de-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00".</span></span> |
| <span data-ttu-id="682de-130">endDateTime</span><span class="sxs-lookup"><span data-stu-id="682de-130">endDateTime</span></span>   | <span data-ttu-id="682de-131">String</span><span class="sxs-lookup"><span data-stu-id="682de-131">String</span></span> | <span data-ttu-id="682de-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2019-11-08T20:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="682de-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00".</span></span>   |

<span data-ttu-id="682de-134">Значения `startDateTime` и `endDateTime` интерпретируются с использованием смещения часового пояса, указанного в значении, и на них не влияет значение заголовка `Prefer: outlook.timezone` при его наличии.</span><span class="sxs-lookup"><span data-stu-id="682de-134">The values of `startDateTime` and `endDateTime` are interpreted using the timezone offset specified in the value and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="682de-135">Если в значении не указано смещение часового пояса, оно интерпретируется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="682de-135">If no timezone offset is included in the value, it is interpreted as UTC.</span></span>

<span data-ttu-id="682de-136">Этот метод также поддерживает некоторые [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="682de-136">This method also supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

> [!NOTE]
> <span data-ttu-id="682de-137">Свойства **createdDateTime** и **lastModifiedDateTime** [события](../resources/event.md) не поддерживают `$select`.</span><span class="sxs-lookup"><span data-stu-id="682de-137">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="682de-138">Чтобы получить их значения, просто запросите **calendarView**, не применяя `$select`.</span><span class="sxs-lookup"><span data-stu-id="682de-138">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="682de-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="682de-139">Request headers</span></span>
| <span data-ttu-id="682de-140">Имя</span><span class="sxs-lookup"><span data-stu-id="682de-140">Name</span></span>       | <span data-ttu-id="682de-141">Тип</span><span class="sxs-lookup"><span data-stu-id="682de-141">Type</span></span> | <span data-ttu-id="682de-142">Описание</span><span class="sxs-lookup"><span data-stu-id="682de-142">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="682de-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="682de-143">Authorization</span></span>  | <span data-ttu-id="682de-144">string</span><span class="sxs-lookup"><span data-stu-id="682de-144">string</span></span> | <span data-ttu-id="682de-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="682de-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="682de-147">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="682de-147">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="682de-148">string</span><span class="sxs-lookup"><span data-stu-id="682de-148">string</span></span> | <span data-ttu-id="682de-149">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="682de-149">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="682de-150">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="682de-150">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="682de-151">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="682de-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="682de-152">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="682de-152">Request body</span></span>
<span data-ttu-id="682de-153">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="682de-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="682de-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="682de-154">Response</span></span>

<span data-ttu-id="682de-155">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="682de-155">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="682de-156">Пример</span><span class="sxs-lookup"><span data-stu-id="682de-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="682de-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="682de-157">Request</span></span>
<span data-ttu-id="682de-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="682de-158">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="682de-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="682de-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-01-07T19:00:00-08:00
```
# <a name="c"></a>[<span data-ttu-id="682de-160">C#</span><span class="sxs-lookup"><span data-stu-id="682de-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="682de-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="682de-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="682de-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="682de-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="682de-163">Java</span><span class="sxs-lookup"><span data-stu-id="682de-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="682de-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="682de-164">Response</span></span>
<span data-ttu-id="682de-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="682de-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
