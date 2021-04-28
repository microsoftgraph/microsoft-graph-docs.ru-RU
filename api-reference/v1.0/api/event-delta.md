---
title: 'event: delta'
description: 'Получение списка событий, которые были добавлены в **calendarView** (диапазон событий), обновлены в нем или удалены из него '
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e62229a704ce51b31f0d192107d480ff97f7fd08
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039638"
---
# <a name="event-delta"></a><span data-ttu-id="df2e6-103">event: delta</span><span class="sxs-lookup"><span data-stu-id="df2e6-103">event: delta</span></span>

<span data-ttu-id="df2e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df2e6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df2e6-105">Получение списка событий, которые были добавлены в **calendarView** (диапазон событий) основного календаря пользователя, обновлены в нем или удалены из него.</span><span class="sxs-lookup"><span data-stu-id="df2e6-105">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>

<span data-ttu-id="df2e6-p101">Вызов функции **delta** для событий схож с отправкой запроса `GET /calendarview` на получение диапазона дат в основном календаре пользователя. С тем исключением, что можно запрашивать добавочные изменения в представлении календаря, правильно применяя [маркеры состояния](/graph/delta-query-overview) при этих вызовах. Это позволяет обслуживать и синхронизировать локальное хранилище таких событий пользователя, не загружая каждый раз все события этого календаря с сервера.</span><span class="sxs-lookup"><span data-stu-id="df2e6-p101">A **delta** function call for events is similar to a `GET /calendarview` request for a range of dates in the user's primary calendar, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in that calender view. This allows you to maintain and synchronize a local store of a user's events in the primary calendar, without having to fetch all the events of that calendar from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="df2e6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df2e6-108">Permissions</span></span>
<span data-ttu-id="df2e6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df2e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="df2e6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df2e6-111">Permission type</span></span>      | <span data-ttu-id="df2e6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df2e6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df2e6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df2e6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="df2e6-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="df2e6-114">Calendars.Read</span></span>    |
|<span data-ttu-id="df2e6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df2e6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df2e6-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="df2e6-116">Calendars.Read</span></span>    |
|<span data-ttu-id="df2e6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df2e6-117">Application</span></span> | <span data-ttu-id="df2e6-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="df2e6-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="df2e6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df2e6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}

```

## <a name="query-parameters"></a><span data-ttu-id="df2e6-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="df2e6-120">Query parameters</span></span>

<span data-ttu-id="df2e6-p103">Отслеживание изменений в событиях представляет собой цикл из одного или нескольких вызовов функции **delta**. Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в токене, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик. Параметры запроса нужно указать только один раз в первом запросе. Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего отклика в последующих запросах, так как в нем уже содержатся необходимые закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="df2e6-p103">Tracking changes in events incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>


| <span data-ttu-id="df2e6-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="df2e6-126">Query parameter</span></span>      | <span data-ttu-id="df2e6-127">Тип</span><span class="sxs-lookup"><span data-stu-id="df2e6-127">Type</span></span>   |<span data-ttu-id="df2e6-128">Описание</span><span class="sxs-lookup"><span data-stu-id="df2e6-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df2e6-129">startDateTime</span><span class="sxs-lookup"><span data-stu-id="df2e6-129">startDateTime</span></span>|<span data-ttu-id="df2e6-130">String</span><span class="sxs-lookup"><span data-stu-id="df2e6-130">String</span></span>|<span data-ttu-id="df2e6-p104">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="df2e6-p104">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="df2e6-133">endDateTime</span><span class="sxs-lookup"><span data-stu-id="df2e6-133">endDateTime</span></span>|<span data-ttu-id="df2e6-134">String</span><span class="sxs-lookup"><span data-stu-id="df2e6-134">String</span></span>|<span data-ttu-id="df2e6-p105">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="df2e6-p105">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|
| <span data-ttu-id="df2e6-137">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="df2e6-137">$deltatoken</span></span> | <span data-ttu-id="df2e6-138">string</span><span class="sxs-lookup"><span data-stu-id="df2e6-138">string</span></span> | <span data-ttu-id="df2e6-p106">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` при предыдущем вызове функции **delta** для этого же представления календаря и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этого представления календаря.</span><span class="sxs-lookup"><span data-stu-id="df2e6-p106">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same calendar view, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that calendar view.</span></span>|
| <span data-ttu-id="df2e6-141">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="df2e6-141">$skiptoken</span></span> | <span data-ttu-id="df2e6-142">string</span><span class="sxs-lookup"><span data-stu-id="df2e6-142">string</span></span> | <span data-ttu-id="df2e6-143">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` при предыдущем вызове функции **delta** и указывает на то, что в представлении календаря остаются не отслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="df2e6-143">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same calendar view.</span></span> |

<span data-ttu-id="df2e6-p107">При выполнении разностного запроса для представления календаря следует ожидать получения всех свойств, которые обычно получают с помощью запроса `GET /calendarview`. `$select` в этом случае не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df2e6-p107">When you do a delta query on a calendar view, expect to get all the properties you'd normally get from a `GET /calendarview` request. `$select` is not supported in this case.</span></span> 


## <a name="request-headers"></a><span data-ttu-id="df2e6-146">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df2e6-146">Request headers</span></span>
| <span data-ttu-id="df2e6-147">Имя</span><span class="sxs-lookup"><span data-stu-id="df2e6-147">Name</span></span>       | <span data-ttu-id="df2e6-148">Тип</span><span class="sxs-lookup"><span data-stu-id="df2e6-148">Type</span></span> | <span data-ttu-id="df2e6-149">Описание</span><span class="sxs-lookup"><span data-stu-id="df2e6-149">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="df2e6-150">Authorization</span><span class="sxs-lookup"><span data-stu-id="df2e6-150">Authorization</span></span>  | <span data-ttu-id="df2e6-151">string</span><span class="sxs-lookup"><span data-stu-id="df2e6-151">string</span></span>  | <span data-ttu-id="df2e6-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df2e6-p108">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="df2e6-154">Content-Type</span><span class="sxs-lookup"><span data-stu-id="df2e6-154">Content-Type</span></span>  | <span data-ttu-id="df2e6-155">string</span><span class="sxs-lookup"><span data-stu-id="df2e6-155">string</span></span>  | <span data-ttu-id="df2e6-p109">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df2e6-p109">application/json. Required.</span></span> |
| <span data-ttu-id="df2e6-158">Prefer</span><span class="sxs-lookup"><span data-stu-id="df2e6-158">Prefer</span></span> | <span data-ttu-id="df2e6-159">string</span><span class="sxs-lookup"><span data-stu-id="df2e6-159">string</span></span>  | <span data-ttu-id="df2e6-p110">odata.maxpagesize={x}. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="df2e6-p110">odata.maxpagesize={x}. Optional.</span></span> |
| <span data-ttu-id="df2e6-162">Prefer</span><span class="sxs-lookup"><span data-stu-id="df2e6-162">Prefer</span></span> | <span data-ttu-id="df2e6-163">string</span><span class="sxs-lookup"><span data-stu-id="df2e6-163">string</span></span> | <span data-ttu-id="df2e6-p111">{Часовой пояс}. Необязательный. Если параметр не указан, по умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="df2e6-p111">{Time zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="response"></a><span data-ttu-id="df2e6-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="df2e6-166">Response</span></span>

<span data-ttu-id="df2e6-167">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект коллекции [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="df2e6-167">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df2e6-168">Пример</span><span class="sxs-lookup"><span data-stu-id="df2e6-168">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df2e6-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="df2e6-169">Request</span></span>

<span data-ttu-id="df2e6-170">В следующем примере показано, как выполнить один вызов функции **delta** и ограничить максимальное количество событий в теле отклика двумя.</span><span class="sxs-lookup"><span data-stu-id="df2e6-170">The following example shows how to make a single **delta** function call, and limit the maximum number of events in the response body to 2.</span></span>

<span data-ttu-id="df2e6-171">Чтобы отследить изменения в представлении календаря, выполните один или несколько вызовов функции **delta** с правильными [маркерами состояния](/graph/delta-query-overview), чтобы получить набор добавочных изменений с момента последнего разностного запроса.</span><span class="sxs-lookup"><span data-stu-id="df2e6-171">To track changes in a calendar view, you would make one or more **delta** function calls, with appropriate [state tokens](/graph/delta-query-overview), to get the set of incremental changes since the last delta query.</span></span> 


# <a name="http"></a>[<span data-ttu-id="df2e6-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="df2e6-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime={start_datetime}&enddatetime={end_datetime}

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="df2e6-173">C#</span><span class="sxs-lookup"><span data-stu-id="df2e6-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df2e6-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df2e6-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df2e6-175">Java</span><span class="sxs-lookup"><span data-stu-id="df2e6-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="df2e6-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="df2e6-176">Response</span></span>
<span data-ttu-id="df2e6-p112">В случае успешного выполнения запроса отклик будет включать маркер состояния — _skipToken_ или _deltaToken_. Первый указан в заголовке отклика _@odata.nextLink_, второй — в заголовке отклика _@odata.deltaLink_. Первый указывает на необходимость продолжать цикл, второй — на наличие всех изменений для определенного цикла.</span><span class="sxs-lookup"><span data-stu-id="df2e6-p112">If the request is successful, the response would include a state token, which is either a _skipToken_ (in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="df2e6-179">Ниже показан отклик с маркером состояния _skipToken_ в заголовке отклика _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="df2e6-179">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="df2e6-180">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="df2e6-180">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 359

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "response-value",
        "time": "datetime-value"
      },
      "transactionId": null,
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isDraft": false,
      "isReminderOn": true
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="df2e6-181">См. также</span><span class="sxs-lookup"><span data-stu-id="df2e6-181">See also</span></span>

- [<span data-ttu-id="df2e6-182">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="df2e6-182">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="df2e6-183">Получение добавочных изменений событий в календаре</span><span class="sxs-lookup"><span data-stu-id="df2e6-183">Get incremental changes to events in a calendar</span></span>](/graph/delta-query-events)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

