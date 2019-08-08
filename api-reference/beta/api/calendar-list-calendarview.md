---
title: Список calendarView
description: Получение исключений, повторяемых или единичных экземпляров событий в представлении календаря, которое определяется заданным диапазоном времени,
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fb912124ac903f74672b21bf42882b5a059da72b
ms.sourcegitcommit: eb5f63deafcdd6db44e791f2d1f4c46604ab06fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/07/2019
ms.locfileid: "36245616"
---
# <a name="list-calendarview"></a><span data-ttu-id="51f13-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="51f13-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51f13-104">Получение вхождений, исключений и отдельных экземпляров событий в представлении календаря, определенного диапазоном времени, из календаря `(../me/calendarview)` пользователя по умолчанию или другого календаря пользователя.</span><span class="sxs-lookup"><span data-stu-id="51f13-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from a user's default calendar `(../me/calendarview)` or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="51f13-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51f13-105">Permissions</span></span>
<span data-ttu-id="51f13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51f13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51f13-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51f13-108">Permission type</span></span>      | <span data-ttu-id="51f13-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51f13-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51f13-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51f13-110">Delegated (work or school account)</span></span> | <span data-ttu-id="51f13-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51f13-111">Calendars.Read, Calendars.ReadWrite</span></span> |
|<span data-ttu-id="51f13-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51f13-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51f13-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51f13-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="51f13-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51f13-114">Application</span></span> | <span data-ttu-id="51f13-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51f13-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="51f13-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51f13-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="51f13-117">Экземпляр [calendar](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="51f13-117">A user's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="51f13-118">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="51f13-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="51f13-119">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="51f13-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="51f13-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="51f13-120">Query parameters</span></span>

<span data-ttu-id="51f13-121">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="51f13-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="51f13-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="51f13-122">Parameter</span></span>    | <span data-ttu-id="51f13-123">Тип</span><span class="sxs-lookup"><span data-stu-id="51f13-123">Type</span></span>   |<span data-ttu-id="51f13-124">Описание</span><span class="sxs-lookup"><span data-stu-id="51f13-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51f13-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="51f13-125">startDateTime</span></span>|<span data-ttu-id="51f13-126">String</span><span class="sxs-lookup"><span data-stu-id="51f13-126">String</span></span>|<span data-ttu-id="51f13-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="51f13-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="51f13-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="51f13-129">endDateTime</span></span>|<span data-ttu-id="51f13-130">String</span><span class="sxs-lookup"><span data-stu-id="51f13-130">String</span></span>|<span data-ttu-id="51f13-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="51f13-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="51f13-133">Этот метод также поддерживает некоторые [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="51f13-133">This method also supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE] 
> <span data-ttu-id="51f13-134">Свойства **createdDateTime** и **lastModifiedDateTime** для [события](../resources/event.md) не поддерживаются `$select`.</span><span class="sxs-lookup"><span data-stu-id="51f13-134">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="51f13-135">Чтобы получить их значения, просто запросите запрос в `$select` **calendarView** , не прибегая к применению.</span><span class="sxs-lookup"><span data-stu-id="51f13-135">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51f13-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51f13-136">Request headers</span></span>
| <span data-ttu-id="51f13-137">Имя</span><span class="sxs-lookup"><span data-stu-id="51f13-137">Name</span></span>       | <span data-ttu-id="51f13-138">Тип</span><span class="sxs-lookup"><span data-stu-id="51f13-138">Type</span></span> | <span data-ttu-id="51f13-139">Описание</span><span class="sxs-lookup"><span data-stu-id="51f13-139">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="51f13-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="51f13-140">Authorization</span></span>  | <span data-ttu-id="51f13-141">string</span><span class="sxs-lookup"><span data-stu-id="51f13-141">string</span></span> | <span data-ttu-id="51f13-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51f13-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="51f13-144">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="51f13-144">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="51f13-145">string</span><span class="sxs-lookup"><span data-stu-id="51f13-145">string</span></span> | <span data-ttu-id="51f13-146">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="51f13-146">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="51f13-147">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="51f13-147">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="51f13-148">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="51f13-148">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51f13-149">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51f13-149">Request body</span></span>
<span data-ttu-id="51f13-150">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51f13-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51f13-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="51f13-151">Response</span></span>

<span data-ttu-id="51f13-152">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="51f13-152">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="51f13-153">Пример</span><span class="sxs-lookup"><span data-stu-id="51f13-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51f13-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="51f13-154">Request</span></span>
<span data-ttu-id="51f13-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51f13-155">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="51f13-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="51f13-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="51f13-157">C#</span><span class="sxs-lookup"><span data-stu-id="51f13-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="51f13-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="51f13-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="51f13-159">Цель — C</span><span class="sxs-lookup"><span data-stu-id="51f13-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="51f13-160">Java</span><span class="sxs-lookup"><span data-stu-id="51f13-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="51f13-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="51f13-161">Response</span></span>
<span data-ttu-id="51f13-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51f13-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
