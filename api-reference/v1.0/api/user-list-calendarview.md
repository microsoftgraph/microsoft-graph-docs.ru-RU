---
title: Список calendarView
description: 'Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря пользователя, которое определяется заданным диапазоном времени. '
localization_priority: Priority
doc_type: apiPageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 9cbb8c31605ac389fb4e9607795ca5108f50a1f3
ms.sourcegitcommit: 2a601cffdb8df375b2ee32a1f35b8f71e0ffd04f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2020
ms.locfileid: "41023147"
---
# <a name="list-calendarview"></a><span data-ttu-id="93ff7-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="93ff7-103">List calendarView</span></span>

<span data-ttu-id="93ff7-104">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного либо другого календаря пользователя, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="93ff7-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="93ff7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93ff7-105">Permissions</span></span>
<span data-ttu-id="93ff7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93ff7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93ff7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93ff7-108">Permission type</span></span>      | <span data-ttu-id="93ff7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93ff7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93ff7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93ff7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="93ff7-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93ff7-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="93ff7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93ff7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93ff7-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93ff7-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="93ff7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93ff7-114">Application</span></span> | <span data-ttu-id="93ff7-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93ff7-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="93ff7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93ff7-116">HTTP request</span></span>

<span data-ttu-id="93ff7-117">Экземпляр [calendar](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="93ff7-117">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="93ff7-118">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="93ff7-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="93ff7-119">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="93ff7-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="93ff7-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="93ff7-120">Query parameters</span></span>

<span data-ttu-id="93ff7-121">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="93ff7-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="93ff7-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="93ff7-122">Parameter</span></span>     | <span data-ttu-id="93ff7-123">Тип</span><span class="sxs-lookup"><span data-stu-id="93ff7-123">Type</span></span>   | <span data-ttu-id="93ff7-124">Описание</span><span class="sxs-lookup"><span data-stu-id="93ff7-124">Description</span></span>                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="93ff7-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="93ff7-125">startDateTime</span></span> | <span data-ttu-id="93ff7-126">String</span><span class="sxs-lookup"><span data-stu-id="93ff7-126">String</span></span> | <span data-ttu-id="93ff7-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2019-11-08T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="93ff7-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span> |
| <span data-ttu-id="93ff7-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="93ff7-129">endDateTime</span></span>   | <span data-ttu-id="93ff7-130">String</span><span class="sxs-lookup"><span data-stu-id="93ff7-130">String</span></span> | <span data-ttu-id="93ff7-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2019-11-08T20:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="93ff7-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>   |

<span data-ttu-id="93ff7-133">Значения `startDateTime` и `endDateTime` интерпретируются с использованием смещения часового пояса, указанного в значении, и на них не влияет значение заголовка `Prefer: outlook.timezone` при его наличии.</span><span class="sxs-lookup"><span data-stu-id="93ff7-133">The values of `startDateTime` and `endDateTime` are interpreted using the timezone offset specified in the value and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="93ff7-134">Если в значении не указано смещение часового пояса, оно интерпретируется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="93ff7-134">If no timezone offset is included in the value, it is interpreted as UTC.</span></span>

<span data-ttu-id="93ff7-135">Этот метод также поддерживает некоторые [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="93ff7-135">This method also supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE]
> <span data-ttu-id="93ff7-136">Свойства **createdDateTime** и **lastModifiedDateTime** [события](../resources/event.md) не поддерживают `$select`.</span><span class="sxs-lookup"><span data-stu-id="93ff7-136">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="93ff7-137">Чтобы получить их значения, просто запросите **calendarView**, не применяя `$select`.</span><span class="sxs-lookup"><span data-stu-id="93ff7-137">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93ff7-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93ff7-138">Request headers</span></span>
| <span data-ttu-id="93ff7-139">Имя</span><span class="sxs-lookup"><span data-stu-id="93ff7-139">Name</span></span>       | <span data-ttu-id="93ff7-140">Тип</span><span class="sxs-lookup"><span data-stu-id="93ff7-140">Type</span></span> | <span data-ttu-id="93ff7-141">Описание</span><span class="sxs-lookup"><span data-stu-id="93ff7-141">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="93ff7-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="93ff7-142">Authorization</span></span>  | <span data-ttu-id="93ff7-143">string</span><span class="sxs-lookup"><span data-stu-id="93ff7-143">string</span></span> | <span data-ttu-id="93ff7-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93ff7-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="93ff7-146">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="93ff7-146">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="93ff7-147">string</span><span class="sxs-lookup"><span data-stu-id="93ff7-147">string</span></span> | <span data-ttu-id="93ff7-148">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="93ff7-148">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="93ff7-149">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="93ff7-149">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="93ff7-150">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="93ff7-150">Optional.</span></span> |
| <span data-ttu-id="93ff7-151">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="93ff7-151">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="93ff7-152">string</span><span class="sxs-lookup"><span data-stu-id="93ff7-152">string</span></span> | <span data-ttu-id="93ff7-153">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="93ff7-153">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="93ff7-154">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="93ff7-154">Values can be "text" or "html".</span></span> <span data-ttu-id="93ff7-155">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="93ff7-155">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="93ff7-156">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="93ff7-156">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="93ff7-157">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="93ff7-157">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93ff7-158">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="93ff7-158">Request body</span></span>
<span data-ttu-id="93ff7-159">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93ff7-159">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93ff7-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="93ff7-160">Response</span></span>

<span data-ttu-id="93ff7-161">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="93ff7-161">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="93ff7-162">Пример</span><span class="sxs-lookup"><span data-stu-id="93ff7-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93ff7-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="93ff7-163">Request</span></span>
<span data-ttu-id="93ff7-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93ff7-164">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="93ff7-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="93ff7-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2020-01-01T19:00:00-08:00&endDateTime=2020-01-02T19:00:00-08:00
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="93ff7-166">C#</span><span class="sxs-lookup"><span data-stu-id="93ff7-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93ff7-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93ff7-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="93ff7-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93ff7-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="93ff7-169">Java</span><span class="sxs-lookup"><span data-stu-id="93ff7-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="93ff7-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="93ff7-170">Response</span></span>
<span data-ttu-id="93ff7-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93ff7-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
