---
title: Список calendarView
description: Получение исключений, повторяемых или единичных экземпляров событий в представлении календаря, которое определяется заданным диапазоном времени,
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a2b16788e4c312816d2a8336f002e0a30fafb109
ms.sourcegitcommit: 2a601cffdb8df375b2ee32a1f35b8f71e0ffd04f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2020
ms.locfileid: "41023070"
---
# <a name="list-calendarview"></a><span data-ttu-id="2e311-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="2e311-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e311-104">Получение в представлении календаря исключений, повторяемых или единичных экземпляров событий за определенный диапазон времени, указанных в стандартном `(../me/calendarview)` или любом другом календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="2e311-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from a user's default calendar `(../me/calendarview)` or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e311-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e311-105">Permissions</span></span>
<span data-ttu-id="2e311-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e311-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e311-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e311-108">Permission type</span></span>      | <span data-ttu-id="2e311-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e311-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e311-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e311-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2e311-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e311-111">Calendars.Read, Calendars.ReadWrite</span></span> |
|<span data-ttu-id="2e311-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e311-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e311-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e311-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2e311-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e311-114">Application</span></span> | <span data-ttu-id="2e311-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e311-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e311-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e311-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="2e311-117">Экземпляр [calendar](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="2e311-117">A user's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="2e311-118">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="2e311-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="2e311-119">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="2e311-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="2e311-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="2e311-120">Query parameters</span></span>

<span data-ttu-id="2e311-121">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="2e311-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="2e311-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="2e311-122">Parameter</span></span>     | <span data-ttu-id="2e311-123">Тип</span><span class="sxs-lookup"><span data-stu-id="2e311-123">Type</span></span>   | <span data-ttu-id="2e311-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2e311-124">Description</span></span>                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2e311-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2e311-125">startDateTime</span></span> | <span data-ttu-id="2e311-126">String</span><span class="sxs-lookup"><span data-stu-id="2e311-126">String</span></span> | <span data-ttu-id="2e311-p102">Дата и время начала периода времени, представленного в формате ISO 8601. Пример: "2019 – 11 – 08T19:00:00 – 08:00".</span><span class="sxs-lookup"><span data-stu-id="2e311-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00".</span></span> |
| <span data-ttu-id="2e311-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="2e311-129">endDateTime</span></span>   | <span data-ttu-id="2e311-130">String</span><span class="sxs-lookup"><span data-stu-id="2e311-130">String</span></span> | <span data-ttu-id="2e311-p103">Дата и время окончания периода времени, представленного в формате ISO 8601. Пример: "2019 – 11 – 08T20:00:00 – 08:00".</span><span class="sxs-lookup"><span data-stu-id="2e311-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00".</span></span>   |

<span data-ttu-id="2e311-133">Значения `startDateTime` и `endDateTime` интерпретируются с использованием смещения часового пояса, указанного в значении, и не влияют на значение `Prefer: outlook.timezone` заголовка, если оно присутствует.</span><span class="sxs-lookup"><span data-stu-id="2e311-133">The values of `startDateTime` and `endDateTime` are interpreted using the timezone offset specified in the value and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="2e311-134">Если значение смещения в часовом поясе не включено, оно интерпретируется как время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="2e311-134">If no timezone offset is included in the value, it is interpreted as UTC.</span></span>

<span data-ttu-id="2e311-135">Этот метод также поддерживает некоторые [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2e311-135">This method also supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE]
> <span data-ttu-id="2e311-136">Свойства **createdDateTime** и **lastModifiedDateTime** [события](../resources/event.md) не поддерживают `$select`.</span><span class="sxs-lookup"><span data-stu-id="2e311-136">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="2e311-137">Чтобы получить их значения, просто запросите **calendarView**, не применяя `$select`.</span><span class="sxs-lookup"><span data-stu-id="2e311-137">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e311-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e311-138">Request headers</span></span>
| <span data-ttu-id="2e311-139">Имя</span><span class="sxs-lookup"><span data-stu-id="2e311-139">Name</span></span>       | <span data-ttu-id="2e311-140">Тип</span><span class="sxs-lookup"><span data-stu-id="2e311-140">Type</span></span> | <span data-ttu-id="2e311-141">Описание</span><span class="sxs-lookup"><span data-stu-id="2e311-141">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="2e311-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e311-142">Authorization</span></span>  | <span data-ttu-id="2e311-143">string</span><span class="sxs-lookup"><span data-stu-id="2e311-143">string</span></span> | <span data-ttu-id="2e311-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e311-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2e311-146">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="2e311-146">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="2e311-147">string</span><span class="sxs-lookup"><span data-stu-id="2e311-147">string</span></span> | <span data-ttu-id="2e311-148">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="2e311-148">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="2e311-149">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="2e311-149">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="2e311-150">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="2e311-150">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e311-151">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e311-151">Request body</span></span>
<span data-ttu-id="2e311-152">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e311-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e311-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e311-153">Response</span></span>

<span data-ttu-id="2e311-154">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2e311-154">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2e311-155">Пример</span><span class="sxs-lookup"><span data-stu-id="2e311-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e311-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e311-156">Request</span></span>
<span data-ttu-id="2e311-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e311-157">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2e311-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e311-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-01-07T19:00:00-08:00
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2e311-159">C#</span><span class="sxs-lookup"><span data-stu-id="2e311-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2e311-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e311-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2e311-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e311-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2e311-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e311-162">Response</span></span>
<span data-ttu-id="2e311-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e311-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
