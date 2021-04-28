---
title: Список calendarView
description: Получение исключений, повторяемых или единичных экземпляров событий в представлении календаря, которое определяется заданным диапазоном времени,
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4a3caa3aa190f899163c75d7f4b89a14b88465b5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052525"
---
# <a name="list-calendarview"></a><span data-ttu-id="26850-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="26850-103">List calendarView</span></span>

<span data-ttu-id="26850-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26850-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="26850-105">Получение в представлении календаря исключений, повторяемых или единичных экземпляров событий за определенный диапазон времени, указанных в стандартном `(../me/calendarview)` или любом другом календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="26850-105">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from a user's default calendar `(../me/calendarview)` or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="26850-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26850-106">Permissions</span></span>
<span data-ttu-id="26850-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26850-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26850-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26850-109">Permission type</span></span>      | <span data-ttu-id="26850-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26850-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26850-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26850-111">Delegated (work or school account)</span></span> | <span data-ttu-id="26850-112">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26850-112">Calendars.Read, Calendars.ReadWrite</span></span> |
|<span data-ttu-id="26850-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26850-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26850-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26850-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="26850-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26850-115">Application</span></span> | <span data-ttu-id="26850-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26850-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="26850-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26850-117">HTTP request</span></span>

<span data-ttu-id="26850-118">Экземпляр [calendar](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="26850-118">A user's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="26850-119">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="26850-119">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="26850-120">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="26850-120">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="26850-121">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="26850-121">Query parameters</span></span>

<span data-ttu-id="26850-122">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="26850-122">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="26850-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="26850-123">Parameter</span></span>     | <span data-ttu-id="26850-124">Тип</span><span class="sxs-lookup"><span data-stu-id="26850-124">Type</span></span>   | <span data-ttu-id="26850-125">Описание</span><span class="sxs-lookup"><span data-stu-id="26850-125">Description</span></span>                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="26850-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="26850-126">startDateTime</span></span> | <span data-ttu-id="26850-127">String</span><span class="sxs-lookup"><span data-stu-id="26850-127">String</span></span> | <span data-ttu-id="26850-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2019-11-08T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="26850-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00".</span></span> |
| <span data-ttu-id="26850-130">endDateTime</span><span class="sxs-lookup"><span data-stu-id="26850-130">endDateTime</span></span>   | <span data-ttu-id="26850-131">String</span><span class="sxs-lookup"><span data-stu-id="26850-131">String</span></span> | <span data-ttu-id="26850-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2019-11-08T20:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="26850-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00".</span></span>   |

<span data-ttu-id="26850-134">Значения `startDateTime` и `endDateTime` интерпретируются с использованием смещения часового пояса, указанного в значении, и на них не влияет значение заголовка `Prefer: outlook.timezone` при его наличии.</span><span class="sxs-lookup"><span data-stu-id="26850-134">The values of `startDateTime` and `endDateTime` are interpreted using the timezone offset specified in the value and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="26850-135">Если в значении не указано смещение часового пояса, оно интерпретируется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="26850-135">If no timezone offset is included in the value, it is interpreted as UTC.</span></span>

<span data-ttu-id="26850-136">Этот метод также поддерживает некоторые [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="26850-136">This method also supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

> [!NOTE]
> <span data-ttu-id="26850-137">Свойства **createdDateTime** и **lastModifiedDateTime** [события](../resources/event.md) не поддерживают `$select`.</span><span class="sxs-lookup"><span data-stu-id="26850-137">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="26850-138">Чтобы получить их значения, просто запросите **calendarView**, не применяя `$select`.</span><span class="sxs-lookup"><span data-stu-id="26850-138">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="26850-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26850-139">Request headers</span></span>
| <span data-ttu-id="26850-140">Имя</span><span class="sxs-lookup"><span data-stu-id="26850-140">Name</span></span>       | <span data-ttu-id="26850-141">Тип</span><span class="sxs-lookup"><span data-stu-id="26850-141">Type</span></span> | <span data-ttu-id="26850-142">Описание</span><span class="sxs-lookup"><span data-stu-id="26850-142">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="26850-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="26850-143">Authorization</span></span>  | <span data-ttu-id="26850-144">string</span><span class="sxs-lookup"><span data-stu-id="26850-144">string</span></span> | <span data-ttu-id="26850-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26850-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="26850-147">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="26850-147">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="26850-148">string</span><span class="sxs-lookup"><span data-stu-id="26850-148">string</span></span> | <span data-ttu-id="26850-p107">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в отклике. Если он не задан, эти значения времени возвращаются в формате UTC. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="26850-p107">Use this to specify the time zone for start and end times in the response. If not specified, those time values are returned in UTC. Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26850-152">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26850-152">Request body</span></span>
<span data-ttu-id="26850-153">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26850-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26850-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="26850-154">Response</span></span>

<span data-ttu-id="26850-155">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="26850-155">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="26850-156">Пример</span><span class="sxs-lookup"><span data-stu-id="26850-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26850-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="26850-157">Request</span></span>
<span data-ttu-id="26850-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26850-158">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26850-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="26850-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-01-07T19:00:00-08:00
```
# <a name="c"></a>[<span data-ttu-id="26850-160">C#</span><span class="sxs-lookup"><span data-stu-id="26850-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26850-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26850-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26850-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26850-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26850-163">Java</span><span class="sxs-lookup"><span data-stu-id="26850-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="26850-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="26850-164">Response</span></span>
<span data-ttu-id="26850-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="26850-165">Here is an example of the response.</span></span> <span data-ttu-id="26850-166">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="26850-166">Note: The response object shown here might be shortened for readability.</span></span>
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
