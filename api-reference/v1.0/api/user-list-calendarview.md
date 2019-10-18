---
title: Список calendarView
description: 'Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря пользователя, которое определяется заданным диапазоном времени. '
localization_priority: Priority
doc_type: apiPageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: c787b7c3eb9be5e1baa88342e97176260acc7c05
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729072"
---
# <a name="list-calendarview"></a><span data-ttu-id="71e2a-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="71e2a-103">List calendarView</span></span>

<span data-ttu-id="71e2a-104">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного либо другого календаря пользователя, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="71e2a-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="71e2a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71e2a-105">Permissions</span></span>
<span data-ttu-id="71e2a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71e2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71e2a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71e2a-108">Permission type</span></span>      | <span data-ttu-id="71e2a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71e2a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71e2a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71e2a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="71e2a-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71e2a-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="71e2a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71e2a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71e2a-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71e2a-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="71e2a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71e2a-114">Application</span></span> | <span data-ttu-id="71e2a-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71e2a-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="71e2a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71e2a-116">HTTP request</span></span>

<span data-ttu-id="71e2a-117">Экземпляр [calendar](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="71e2a-117">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="71e2a-118">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="71e2a-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="71e2a-119">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="71e2a-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="71e2a-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="71e2a-120">Query parameters</span></span>

<span data-ttu-id="71e2a-121">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="71e2a-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="71e2a-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="71e2a-122">Parameter</span></span>    | <span data-ttu-id="71e2a-123">Тип</span><span class="sxs-lookup"><span data-stu-id="71e2a-123">Type</span></span>   |<span data-ttu-id="71e2a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="71e2a-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71e2a-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="71e2a-125">startDateTime</span></span>|<span data-ttu-id="71e2a-126">String</span><span class="sxs-lookup"><span data-stu-id="71e2a-126">String</span></span>|<span data-ttu-id="71e2a-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="71e2a-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="71e2a-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="71e2a-129">endDateTime</span></span>|<span data-ttu-id="71e2a-130">String</span><span class="sxs-lookup"><span data-stu-id="71e2a-130">String</span></span>|<span data-ttu-id="71e2a-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="71e2a-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="71e2a-133">Этот метод также поддерживает некоторые [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="71e2a-133">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE] 
> <span data-ttu-id="71e2a-134">Свойства **createdDateTime** и **lastModifiedDateTime** [события](../resources/event.md) не поддерживают `$select`.</span><span class="sxs-lookup"><span data-stu-id="71e2a-134">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="71e2a-135">Чтобы получить их значения, просто запросите **calendarView**, не применяя `$select`.</span><span class="sxs-lookup"><span data-stu-id="71e2a-135">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71e2a-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71e2a-136">Request headers</span></span>
| <span data-ttu-id="71e2a-137">Имя</span><span class="sxs-lookup"><span data-stu-id="71e2a-137">Name</span></span>       | <span data-ttu-id="71e2a-138">Тип</span><span class="sxs-lookup"><span data-stu-id="71e2a-138">Type</span></span> | <span data-ttu-id="71e2a-139">Описание</span><span class="sxs-lookup"><span data-stu-id="71e2a-139">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="71e2a-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="71e2a-140">Authorization</span></span>  | <span data-ttu-id="71e2a-141">string</span><span class="sxs-lookup"><span data-stu-id="71e2a-141">string</span></span> | <span data-ttu-id="71e2a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71e2a-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="71e2a-144">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="71e2a-144">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="71e2a-145">string</span><span class="sxs-lookup"><span data-stu-id="71e2a-145">string</span></span> | <span data-ttu-id="71e2a-146">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="71e2a-146">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="71e2a-147">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="71e2a-147">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="71e2a-148">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="71e2a-148">Optional.</span></span> |
| <span data-ttu-id="71e2a-149">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="71e2a-149">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="71e2a-150">string</span><span class="sxs-lookup"><span data-stu-id="71e2a-150">string</span></span> | <span data-ttu-id="71e2a-151">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="71e2a-151">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="71e2a-152">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="71e2a-152">Values can be "text" or "html".</span></span> <span data-ttu-id="71e2a-153">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="71e2a-153">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="71e2a-154">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="71e2a-154">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="71e2a-155">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="71e2a-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71e2a-156">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="71e2a-156">Request body</span></span>
<span data-ttu-id="71e2a-157">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71e2a-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71e2a-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="71e2a-158">Response</span></span>

<span data-ttu-id="71e2a-159">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="71e2a-159">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71e2a-160">Пример</span><span class="sxs-lookup"><span data-stu-id="71e2a-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71e2a-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="71e2a-161">Request</span></span>
<span data-ttu-id="71e2a-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71e2a-162">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="71e2a-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="71e2a-163">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="71e2a-164">C#</span><span class="sxs-lookup"><span data-stu-id="71e2a-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71e2a-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71e2a-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="71e2a-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71e2a-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="71e2a-167">Java</span><span class="sxs-lookup"><span data-stu-id="71e2a-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="71e2a-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="71e2a-168">Response</span></span>
<span data-ttu-id="71e2a-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71e2a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
