---
title: Список calendarView
description: Получение исключений, повторяемых или единичных экземпляров событий в представлении календаря, которое определяется заданным диапазоном времени,
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d91456806e4e81b4b211680e85dc12aca04f3084
ms.sourcegitcommit: b198efc2391a12a840e4f1b8c42c18a55b06037f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2019
ms.locfileid: "35820670"
---
# <a name="list-calendarview"></a><span data-ttu-id="c9aae-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="c9aae-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9aae-104">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря `(../me/calendarview)`, принадлежащего пользователю или группе, либо другого календаря пользователя, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="c9aae-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9aae-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9aae-105">Permissions</span></span>
<span data-ttu-id="c9aae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9aae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="c9aae-108">События в календаре пользователя: Calendars.Read или Calendars.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="c9aae-108">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="c9aae-109">События в календаре группы: Group.Read.All или Group.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="c9aae-109">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c9aae-110">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9aae-110">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="c9aae-111">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c9aae-111">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="c9aae-112">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="c9aae-112">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="c9aae-113">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="c9aae-113">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="c9aae-114">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="c9aae-114">Query parameters</span></span>

<span data-ttu-id="c9aae-115">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="c9aae-115">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="c9aae-116">Параметр</span><span class="sxs-lookup"><span data-stu-id="c9aae-116">Parameter</span></span>    | <span data-ttu-id="c9aae-117">Тип</span><span class="sxs-lookup"><span data-stu-id="c9aae-117">Type</span></span>   |<span data-ttu-id="c9aae-118">Описание</span><span class="sxs-lookup"><span data-stu-id="c9aae-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9aae-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c9aae-119">startDateTime</span></span>|<span data-ttu-id="c9aae-120">String</span><span class="sxs-lookup"><span data-stu-id="c9aae-120">String</span></span>|<span data-ttu-id="c9aae-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="c9aae-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="c9aae-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c9aae-123">endDateTime</span></span>|<span data-ttu-id="c9aae-124">String</span><span class="sxs-lookup"><span data-stu-id="c9aae-124">String</span></span>|<span data-ttu-id="c9aae-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="c9aae-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="c9aae-127">Этот метод также поддерживает некоторые [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c9aae-127">This method also supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE] 
> <span data-ttu-id="c9aae-128">Свойства **createdDateTime** и **lastModifiedDateTime** для [события](../resources/event.md) не поддерживаются `$select`.</span><span class="sxs-lookup"><span data-stu-id="c9aae-128">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="c9aae-129">Чтобы получить их значения, просто запросите запрос в `$select` **calendarView** , не прибегая к применению.</span><span class="sxs-lookup"><span data-stu-id="c9aae-129">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9aae-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9aae-130">Request headers</span></span>
| <span data-ttu-id="c9aae-131">Имя</span><span class="sxs-lookup"><span data-stu-id="c9aae-131">Name</span></span>       | <span data-ttu-id="c9aae-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c9aae-132">Type</span></span> | <span data-ttu-id="c9aae-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c9aae-133">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="c9aae-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9aae-134">Authorization</span></span>  | <span data-ttu-id="c9aae-135">string</span><span class="sxs-lookup"><span data-stu-id="c9aae-135">string</span></span> | <span data-ttu-id="c9aae-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9aae-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c9aae-138">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="c9aae-138">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="c9aae-139">string</span><span class="sxs-lookup"><span data-stu-id="c9aae-139">string</span></span> | <span data-ttu-id="c9aae-140">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="c9aae-140">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="c9aae-141">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c9aae-141">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="c9aae-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c9aae-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9aae-143">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9aae-143">Request body</span></span>
<span data-ttu-id="c9aae-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9aae-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9aae-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9aae-145">Response</span></span>

<span data-ttu-id="c9aae-146">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c9aae-146">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c9aae-147">Пример</span><span class="sxs-lookup"><span data-stu-id="c9aae-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c9aae-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9aae-148">Request</span></span>
<span data-ttu-id="c9aae-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9aae-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c9aae-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9aae-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c9aae-151">C#</span><span class="sxs-lookup"><span data-stu-id="c9aae-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9aae-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="c9aae-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c9aae-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c9aae-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c9aae-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9aae-154">Response</span></span>
<span data-ttu-id="c9aae-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9aae-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
