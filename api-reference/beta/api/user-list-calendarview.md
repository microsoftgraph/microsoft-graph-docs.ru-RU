---
title: Список calendarView
description: Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря пользователя, которое определяется заданным диапазоном времени.
localization_priority: Normal
doc_type: apiPageType
author: harini84
ms.prod: outlook
ms.openlocfilehash: 314d49f3325ebe6966a8a55bf9325779e91a26bd
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473726"
---
# <a name="list-calendarview"></a><span data-ttu-id="553dd-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="553dd-103">List calendarView</span></span>

<span data-ttu-id="553dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="553dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="553dd-105">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного либо другого календаря пользователя, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="553dd-105">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="553dd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="553dd-106">Permissions</span></span>
<span data-ttu-id="553dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="553dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="553dd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="553dd-109">Permission type</span></span>      | <span data-ttu-id="553dd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="553dd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="553dd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="553dd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="553dd-112">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="553dd-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="553dd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="553dd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="553dd-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="553dd-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="553dd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="553dd-115">Application</span></span> | <span data-ttu-id="553dd-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="553dd-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="553dd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="553dd-117">HTTP request</span></span>
<span data-ttu-id="553dd-118">Экземпляр [calendar](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="553dd-118">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="553dd-119">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="553dd-119">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="553dd-120">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="553dd-120">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="553dd-121">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="553dd-121">Query parameters</span></span>

<span data-ttu-id="553dd-122">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="553dd-122">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="553dd-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="553dd-123">Parameter</span></span>     | <span data-ttu-id="553dd-124">Тип</span><span class="sxs-lookup"><span data-stu-id="553dd-124">Type</span></span>   | <span data-ttu-id="553dd-125">Описание</span><span class="sxs-lookup"><span data-stu-id="553dd-125">Description</span></span>                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="553dd-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="553dd-126">startDateTime</span></span> | <span data-ttu-id="553dd-127">String</span><span class="sxs-lookup"><span data-stu-id="553dd-127">String</span></span> | <span data-ttu-id="553dd-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2019-11-08T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="553dd-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00".</span></span> |
| <span data-ttu-id="553dd-130">endDateTime</span><span class="sxs-lookup"><span data-stu-id="553dd-130">endDateTime</span></span>   | <span data-ttu-id="553dd-131">String</span><span class="sxs-lookup"><span data-stu-id="553dd-131">String</span></span> | <span data-ttu-id="553dd-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2019-11-08T20:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="553dd-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00".</span></span>   |

<span data-ttu-id="553dd-134">Значения `startDateTime` и `endDateTime` интерпретируются с использованием смещения часового пояса, указанного в значении, и на них не влияет значение заголовка `Prefer: outlook.timezone` при его наличии.</span><span class="sxs-lookup"><span data-stu-id="553dd-134">The values of `startDateTime` and `endDateTime` are interpreted using the timezone offset specified in the value and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="553dd-135">Если в значении не указано смещение часового пояса, оно интерпретируется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="553dd-135">If no timezone offset is included in the value, it is interpreted as UTC.</span></span>

<span data-ttu-id="553dd-136">Этот метод также поддерживает некоторые [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="553dd-136">This method also supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

> [!NOTE]
> <span data-ttu-id="553dd-137">Свойства **createdDateTime** и **lastModifiedDateTime** [события](../resources/event.md) не поддерживают `$select`.</span><span class="sxs-lookup"><span data-stu-id="553dd-137">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="553dd-138">Чтобы получить их значения, просто запросите **calendarView**, не применяя `$select`.</span><span class="sxs-lookup"><span data-stu-id="553dd-138">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="553dd-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="553dd-139">Request headers</span></span>
| <span data-ttu-id="553dd-140">Имя</span><span class="sxs-lookup"><span data-stu-id="553dd-140">Name</span></span>       | <span data-ttu-id="553dd-141">Тип</span><span class="sxs-lookup"><span data-stu-id="553dd-141">Type</span></span> | <span data-ttu-id="553dd-142">Описание</span><span class="sxs-lookup"><span data-stu-id="553dd-142">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="553dd-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="553dd-143">Authorization</span></span>  | <span data-ttu-id="553dd-144">string</span><span class="sxs-lookup"><span data-stu-id="553dd-144">string</span></span> | <span data-ttu-id="553dd-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="553dd-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="553dd-147">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="553dd-147">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="553dd-148">string</span><span class="sxs-lookup"><span data-stu-id="553dd-148">string</span></span> | <span data-ttu-id="553dd-149">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="553dd-149">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="553dd-150">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="553dd-150">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="553dd-151">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="553dd-151">Optional.</span></span> |
| <span data-ttu-id="553dd-152">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="553dd-152">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="553dd-153">string</span><span class="sxs-lookup"><span data-stu-id="553dd-153">string</span></span> | <span data-ttu-id="553dd-154">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="553dd-154">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="553dd-155">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="553dd-155">Values can be "text" or "html".</span></span> <span data-ttu-id="553dd-156">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="553dd-156">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="553dd-157">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="553dd-157">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="553dd-158">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="553dd-158">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="553dd-159">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="553dd-159">Request body</span></span>
<span data-ttu-id="553dd-160">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="553dd-160">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="553dd-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="553dd-161">Response</span></span>

<span data-ttu-id="553dd-162">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="553dd-162">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="553dd-163">Пример</span><span class="sxs-lookup"><span data-stu-id="553dd-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="553dd-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="553dd-164">Request</span></span>
<span data-ttu-id="553dd-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="553dd-165">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="553dd-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="553dd-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2020-01-01T19:00:00-08:00&endDateTime=2020-01-02T19:00:00-08:00
```
# <a name="c"></a>[<span data-ttu-id="553dd-167">C#</span><span class="sxs-lookup"><span data-stu-id="553dd-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="553dd-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="553dd-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="553dd-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="553dd-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="553dd-170">Java</span><span class="sxs-lookup"><span data-stu-id="553dd-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="553dd-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="553dd-171">Response</span></span>
<span data-ttu-id="553dd-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="553dd-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "originalStartTimeZone": "Pacific Standard Time",
      "originalEndTimeZone": "Pacific Standard Time",
      "responseStatus": {
        "response": "accepted",
        "time": "2016-10-19T10:37:00Z"
      },
      "uid": "040000008200E00074C5B7101A82E00800000000D3D70B8A6A17D70100000000000000001000000074665914A06C3F49BB4B7D7EEE4304DA",
      "reminderMinutesBeforeStart": 15,
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
  "keywords": "calendar",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
