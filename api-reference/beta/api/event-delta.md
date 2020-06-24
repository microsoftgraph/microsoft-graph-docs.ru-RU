---
title: 'event: delta'
description: Получение списка событий, которые были добавлены в **calendarView** (диапазон событий), обновлены в нем или удалены из него
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8dac9c1ac5859a1a06a71a1d681b1468730639b1
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44862534"
---
# <a name="event-delta"></a><span data-ttu-id="c7880-103">event: delta</span><span class="sxs-lookup"><span data-stu-id="c7880-103">event: delta</span></span>

<span data-ttu-id="c7880-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7880-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7880-105">Получение набора ресурсов [событий](../resources/event.md) , которые были добавлены, удалены или обновлены в одном или нескольких календарях.</span><span class="sxs-lookup"><span data-stu-id="c7880-105">Get a set of [event](../resources/event.md) resources that have been added, deleted, or updated in one or more calendars.</span></span> 

<span data-ttu-id="c7880-106">Вы можете получать определенные типы этих добавочных изменений в событиях во всех календарях почтового ящика или в определенном календаре или в коллекции событий **calendarView** (диапазон событий, определенных датами начала и окончания) календаря.</span><span class="sxs-lookup"><span data-stu-id="c7880-106">You can get specific types of these incremental changes in the events in all the calendars of a mailbox or in a specific calendar, or in an event collection of a **calendarView** (range of events defined by start and end dates) of a calendar.</span></span> <span data-ttu-id="c7880-107">Календарь может быть календарем по умолчанию или другим указанным календарем пользователя.</span><span class="sxs-lookup"><span data-stu-id="c7880-107">The calendar can be the default calendar or some other specified calendar of the user's.</span></span> <span data-ttu-id="c7880-108">Если вы получаете добавочные изменения в **calendarView**, календарь также может быть календарем группы.</span><span class="sxs-lookup"><span data-stu-id="c7880-108">In the case of getting incremental changes on **calendarView**, the calendar can be a group calendar as well.</span></span>

<span data-ttu-id="c7880-109">Вызов функции **Delta** похож на `GET /events` `GET /calendarview` запрос или запрос для указанного календаря, за исключением того, что при соответствующем применении [маркеров состояния](/graph/delta-query-overview#state-tokens) в одном или нескольких вызовах Вы можете запросить добавочные изменения событий в этой Календер.</span><span class="sxs-lookup"><span data-stu-id="c7880-109">A **delta** function call is similar to a `GET /events` or `GET /calendarview` request for the specified calendar, except that by appropriately applying [state tokens](/graph/delta-query-overview#state-tokens) in one or more of these calls, you can query for incremental changes of events in that calender.</span></span> <span data-ttu-id="c7880-110">Это позволяет поддерживать и синхронизировать локальное хранилище событий в указанном календаре без необходимости каждый раз получать все события этого календаря с сервера.</span><span class="sxs-lookup"><span data-stu-id="c7880-110">This allows you to maintain and synchronize a local store of events in the specified calendar, without having to fetch all the events of that calendar from the server every time.</span></span>

<span data-ttu-id="c7880-111">В следующей таблице перечислены различия между функцией **Delta** в событиях и функцией **Delta** в **calendarView** в календаре.</span><span class="sxs-lookup"><span data-stu-id="c7880-111">The following table lists the differences between the **delta** function on events and the **delta** function on a **calendarView** in a calendar.</span></span>

| <span data-ttu-id="c7880-112">Функция Delta для событий</span><span class="sxs-lookup"><span data-stu-id="c7880-112">Delta function on events</span></span>  | <span data-ttu-id="c7880-113">Функция Delta в calendarView</span><span class="sxs-lookup"><span data-stu-id="c7880-113">Delta function on calendarView</span></span>  |
|:--------------------------|:---------------------------------------------------------|
| <span data-ttu-id="c7880-114">Получает добавочные изменения всех событий в календаре, которые не ограничены диапазоном дат начала и окончания.</span><span class="sxs-lookup"><span data-stu-id="c7880-114">Gets incremental changes of all the events in a calendar not bounded by a start and end date range.</span></span> <span data-ttu-id="c7880-115">Кроме того, вы можете получить добавочные изменения событий в календаре, ограниченные временем начала, начиная с или после даты/времени.</span><span class="sxs-lookup"><span data-stu-id="c7880-115">Alternatively, you can get incremental changes of the events in a calendar bounded by a start time, starting on or after that date/time.</span></span> | <span data-ttu-id="c7880-116">Получает добавочные изменения событий в начале и в конце даты и времени **calendarView**.</span><span class="sxs-lookup"><span data-stu-id="c7880-116">Gets incremental changes of events within the start and end date/time of the **calendarView**.</span></span> |
| <span data-ttu-id="c7880-117">Возвращает ограниченный набор свойств **события** по соображениям производительности.</span><span class="sxs-lookup"><span data-stu-id="c7880-117">Returns only a limited set of **event** properties for performance reasons.</span></span> <span data-ttu-id="c7880-118">Клиент для последующего использования `GET /events/{id}` для развертывания любых событий.</span><span class="sxs-lookup"><span data-stu-id="c7880-118">Client to subsequently use `GET /events/{id}` to expand any events.</span></span> | <span data-ttu-id="c7880-119">Расширение на стороне сервера возвращает более полный набор свойств **события** .</span><span class="sxs-lookup"><span data-stu-id="c7880-119">Server-side expansion returns a fuller set of **event** properties.</span></span> |
| <span data-ttu-id="c7880-120">Ответ включает в себя один экземпляр и образец повторяющегося ряда.</span><span class="sxs-lookup"><span data-stu-id="c7880-120">Response includes single instances and recurring series master.</span></span> | <span data-ttu-id="c7880-121">Ответ включает в себя одиночные экземпляры, а также экземпляры и исключения повторяющихся рядов.</span><span class="sxs-lookup"><span data-stu-id="c7880-121">Response includes single instances, and occurrences and exceptions of recurring series.</span></span> |
| <span data-ttu-id="c7880-122">Применяется к событиям в календарях пользователей, но не календарям групп.</span><span class="sxs-lookup"><span data-stu-id="c7880-122">Applies to events in user calendars but not group calendars.</span></span> | <span data-ttu-id="c7880-123">Применяется к событиям в календарях пользователей и групп.</span><span class="sxs-lookup"><span data-stu-id="c7880-123">Applies to events in user and group calendars.</span></span> |
| <span data-ttu-id="c7880-124">В настоящее время доступно только в бета-версии.</span><span class="sxs-lookup"><span data-stu-id="c7880-124">Currently available only in the beta version.</span></span> | <span data-ttu-id="c7880-125">Доступно в версиях 1.0 и бета-версиях.</span><span class="sxs-lookup"><span data-stu-id="c7880-125">Available in the v1.0 and beta versions.</span></span> |

## <a name="permissions"></a><span data-ttu-id="c7880-126">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7880-126">Permissions</span></span>
<span data-ttu-id="c7880-127">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c7880-127">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c7880-128">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7880-128">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7880-129">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7880-129">Permission type</span></span>      | <span data-ttu-id="c7880-130">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7880-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7880-131">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7880-131">Delegated (work or school account)</span></span> | <span data-ttu-id="c7880-132">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7880-132">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c7880-133">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7880-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7880-134">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7880-134">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c7880-135">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7880-135">Application</span></span> | <span data-ttu-id="c7880-136">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7880-136">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7880-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7880-137">HTTP request</span></span>

<span data-ttu-id="c7880-138">В этом разделе показан синтаксис HTTP-запроса для начального вызова функции **Delta** для запуска полной синхронизации, которая получает все события в указанном календаре или представлении календаря.</span><span class="sxs-lookup"><span data-stu-id="c7880-138">This section shows the HTTP request syntax for the initial **delta** function call to start a full synchronization that retrieves all the events in the specified calendar or calendar view.</span></span> <span data-ttu-id="c7880-139">Этот синтаксис не содержит [маркеров состояния](/graph/delta-query-overview#state-tokens).</span><span class="sxs-lookup"><span data-stu-id="c7880-139">This syntax does not contain any [state tokens](/graph/delta-query-overview#state-tokens).</span></span> 

<span data-ttu-id="c7880-140">URL-адрес запроса, возвращенный в `nextLink` `deltaLink` ответе или успешном ответе, содержит маркер состояния.</span><span class="sxs-lookup"><span data-stu-id="c7880-140">The query URL returned in a `nextLink` or `deltaLink` of a successful response includes a state token.</span></span> <span data-ttu-id="c7880-141">Для любого последующего вызова функции **Delta** используйте URL-адрес запроса в `nextLink` `deltaLink` начале или предшествующем ему запросе.</span><span class="sxs-lookup"><span data-stu-id="c7880-141">For any subsequent **delta** function call, use the query URL in a `nextLink` or `deltaLink` preceding it.</span></span>

### <a name="delta-function-on-events-in-a-user-calendar-preview"></a><span data-ttu-id="c7880-142">Функция Delta для событий в календаре пользователя (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="c7880-142">Delta function on events in a user calendar (preview)</span></span>
<span data-ttu-id="c7880-143">Примените функцию **Delta** ко всем событиям или событиям, начиная с определенной даты/времени или после нее, в указанных календарях пользователей:</span><span class="sxs-lookup"><span data-stu-id="c7880-143">Apply the **delta** function on all the events or events starting on or after a specific date/time, in the specified user calendar(s):</span></span>

* <span data-ttu-id="c7880-144">Для получения добавочных изменений всех событий или событий, начиная с указанной даты и времени или после нее, _в почтовом ящике пользователя_:</span><span class="sxs-lookup"><span data-stu-id="c7880-144">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the user's mailbox_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/events/delta 
  GET /users/{id | userPrincipalName}/events/delta 

  GET /me/events/delta?startDateTime={start_datetime}
  GET /users/{id | userPrincipalName}/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="c7880-145">Для получения добавочных изменений всех событий или событий, начиная с указанной даты или после указанной даты и времени _в календаре пользователя по умолчанию_:</span><span class="sxs-lookup"><span data-stu-id="c7880-145">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the user's default calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendar/events/delta 
  GET /users/{id | userPrincipalName}/calendar/events/delta 

  GET /me/calendar/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendar/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="c7880-146">Для получения добавочных изменений всех событий или событий, начиная с указанной даты и времени или после нее, _в указанном календаре пользователя_:</span><span class="sxs-lookup"><span data-stu-id="c7880-146">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the specified user calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta 

  GET /me/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="c7880-147">Для получения добавочных изменений всех событий или событий, начиная с указанной даты и времени или после нее, _в указанном календаре группы календарей по умолчанию_:</span><span class="sxs-lookup"><span data-stu-id="c7880-147">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the specified calendar of the default calendar group_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendargroup/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/delta 

  GET /me/calendargroup/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="c7880-148">Для получения добавочных изменений всех событий или событий, начиная с указанной даты и времени или после нее, _в указанной группе календаря и календаре_:</span><span class="sxs-lookup"><span data-stu-id="c7880-148">To get incremental changes all the events, or of events starting on or after the specified date/time _in the specified calendar group and calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendargroups/{id}/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/delta 

  GET /me/calendargroups/{id}/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

<!-- Add back and fix html when group calendars are supported

### Delta function on events in a group calendar (preview)
* To get incremental changes of all the events, or of events starting on or after the specified date/time _in a group calendar_:
  !-- { "blockType": "ignored" } --
  ```http
  GET /groups/{id}/events/delta
  GET /groups/{id}/calendar/events/delta

  GET /groups/{id}/events/delta?startDateTime={start_datetime}
  GET /groups/{id}/calendar/events/delta?startDateTime={start_datetime}
  ```

  -->

### <a name="delta-function-on-calendarview-in-a-user-calendar"></a><span data-ttu-id="c7880-149">Функция Delta в calendarView в календаре пользователя</span><span class="sxs-lookup"><span data-stu-id="c7880-149">Delta function on calendarView in a user calendar</span></span>
<span data-ttu-id="c7880-150">Примените функцию **Delta** к диапазону событий, разделенных на дату начала и окончания, в указанном календаре пользователя:</span><span class="sxs-lookup"><span data-stu-id="c7880-150">Apply the **delta** function on a range of events delimited by start and end date/times, in the specified user calendar:</span></span>

* <span data-ttu-id="c7880-151">Для получения добавочных изменений в представлении календаря _календаря пользователя по умолчанию_:</span><span class="sxs-lookup"><span data-stu-id="c7880-151">To get incremental changes in a calendar view of _the user's default calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

* <span data-ttu-id="c7880-152">Чтобы получить добавочные изменения в представлении календаря для _указанного календаря пользователя_:</span><span class="sxs-lookup"><span data-stu-id="c7880-152">To get incremental changes in a calendar view of _the specified user calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

### <a name="delta-function-on-calendarview-in-a-group-calendar"></a><span data-ttu-id="c7880-153">Функция Delta в calendarView в календаре группы</span><span class="sxs-lookup"><span data-stu-id="c7880-153">Delta function on calendarView in a group calendar</span></span>
* <span data-ttu-id="c7880-154">Чтобы получить добавочные изменения в представлении календаря _группы_, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="c7880-154">To get incremental changes in a calendar view of _a group's calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

## <a name="query-parameters"></a><span data-ttu-id="c7880-155">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="c7880-155">Query parameters</span></span>

<span data-ttu-id="c7880-156">Отслеживание изменений приводит к округлению одного или нескольких вызовов функции **Delta** .</span><span class="sxs-lookup"><span data-stu-id="c7880-156">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="c7880-157">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="c7880-157">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="c7880-158">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="c7880-158">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="c7880-159">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="c7880-159">You only need to specify any desired query parameters once upfront.</span></span>
<span data-ttu-id="c7880-160">При последующих запросах просто скопируйте и примените `nextLink` `deltaLink` URL-адрес из предыдущего ответа, так как этот URL-адрес уже включает закодированные, нужные параметры.</span><span class="sxs-lookup"><span data-stu-id="c7880-160">In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="c7880-161">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="c7880-161">Query parameter</span></span>      | <span data-ttu-id="c7880-162">Тип</span><span class="sxs-lookup"><span data-stu-id="c7880-162">Type</span></span>   |<span data-ttu-id="c7880-163">Описание</span><span class="sxs-lookup"><span data-stu-id="c7880-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7880-164">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c7880-164">startDateTime</span></span>|<span data-ttu-id="c7880-165">String</span><span class="sxs-lookup"><span data-stu-id="c7880-165">String</span></span>|<span data-ttu-id="c7880-166">The start date and time of the time range, represented in ISO 8601 format.</span><span class="sxs-lookup"><span data-stu-id="c7880-166">The start date and time of the time range, represented in ISO 8601 format.</span></span> <span data-ttu-id="c7880-167">For example, "2019-11-08T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="c7880-167">For example, "2019-11-08T19:00:00-08:00".</span></span> <br><span data-ttu-id="c7880-168">Часовой пояс указывается в части смещения TimeZone значения параметра и не влияет на `Prefer: outlook.timezone` заголовку, если он есть.</span><span class="sxs-lookup"><span data-stu-id="c7880-168">The timezone is specified in the timezone offset portion of the parameter value, and is not impacted by the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="c7880-169">Если в значении не указано смещение часового пояса, оно интерпретируется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c7880-169">If no timezone offset is included in the value, it is interpreted as UTC.</span></span><br><span data-ttu-id="c7880-170">Необязательно для **изменений** событий в календаре.</span><span class="sxs-lookup"><span data-stu-id="c7880-170">Optional for **delta** on events in a calendar.</span></span> <br><span data-ttu-id="c7880-171">Обязательный для **изменений** в **calendarView**.</span><span class="sxs-lookup"><span data-stu-id="c7880-171">Required for **delta** on **calendarView**.</span></span> |
|<span data-ttu-id="c7880-172">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c7880-172">endDateTime</span></span>|<span data-ttu-id="c7880-173">String</span><span class="sxs-lookup"><span data-stu-id="c7880-173">String</span></span>|<span data-ttu-id="c7880-174">The end date and time of the time range, represented in ISO 8601 format.</span><span class="sxs-lookup"><span data-stu-id="c7880-174">The end date and time of the time range, represented in ISO 8601 format.</span></span> <span data-ttu-id="c7880-175">For example, "2019-11-08T20:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="c7880-175">For example, "2019-11-08T20:00:00-08:00".</span></span> <br><span data-ttu-id="c7880-176">Часовой пояс указывается в части смещения TimeZone значения параметра и не влияет на `Prefer: outlook.timezone` заголовку, если он есть.</span><span class="sxs-lookup"><span data-stu-id="c7880-176">The timezone is specified in the timezone offset portion of the parameter value, and is not impacted by the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="c7880-177">Если в значении не указано смещение часового пояса, оно интерпретируется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c7880-177">If no timezone offset is included in the value, it is interpreted as UTC.</span></span><br><span data-ttu-id="c7880-178">_Не поддерживается_ в **Delta** для событий в календаре.</span><span class="sxs-lookup"><span data-stu-id="c7880-178">_Not supported_ by **delta** on events in a calendar.</span></span> <br><span data-ttu-id="c7880-179">Обязательный для **изменений** в **calendarView**.</span><span class="sxs-lookup"><span data-stu-id="c7880-179">Required for **delta** on **calendarView**.</span></span>|
| <span data-ttu-id="c7880-180">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="c7880-180">$deltatoken</span></span> | <span data-ttu-id="c7880-181">string</span><span class="sxs-lookup"><span data-stu-id="c7880-181">string</span></span> | <span data-ttu-id="c7880-182">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same calendar view, indicating the completion of that round of change tracking.</span><span class="sxs-lookup"><span data-stu-id="c7880-182">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same calendar view, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="c7880-183">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that calendar view.</span><span class="sxs-lookup"><span data-stu-id="c7880-183">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that calendar view.</span></span>|
| <span data-ttu-id="c7880-184">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="c7880-184">$skiptoken</span></span> | <span data-ttu-id="c7880-185">string</span><span class="sxs-lookup"><span data-stu-id="c7880-185">string</span></span> | <span data-ttu-id="c7880-186">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` при предыдущем вызове функции **delta** и указывает на то, что в представлении календаря остаются не отслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="c7880-186">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same calendar view.</span></span> |

<span data-ttu-id="c7880-187">Не поддерживает `$expand` , `$filter` ,, `$orderby` `$select` и `$search` .</span><span class="sxs-lookup"><span data-stu-id="c7880-187">Does not support `$expand`, `$filter`, `$orderby`, `$select`, and `$search`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="c7880-188">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7880-188">Request headers</span></span>
| <span data-ttu-id="c7880-189">Имя</span><span class="sxs-lookup"><span data-stu-id="c7880-189">Name</span></span>       | <span data-ttu-id="c7880-190">Тип</span><span class="sxs-lookup"><span data-stu-id="c7880-190">Type</span></span> | <span data-ttu-id="c7880-191">Описание</span><span class="sxs-lookup"><span data-stu-id="c7880-191">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="c7880-192">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7880-192">Authorization</span></span>  | <span data-ttu-id="c7880-193">string</span><span class="sxs-lookup"><span data-stu-id="c7880-193">string</span></span>  | <span data-ttu-id="c7880-194">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="c7880-194">Bearer {token}.</span></span> <span data-ttu-id="c7880-195">Required.</span><span class="sxs-lookup"><span data-stu-id="c7880-195">Required.</span></span> |
| <span data-ttu-id="c7880-196">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7880-196">Content-Type</span></span>  | <span data-ttu-id="c7880-197">string</span><span class="sxs-lookup"><span data-stu-id="c7880-197">string</span></span>  | <span data-ttu-id="c7880-198">application/json.</span><span class="sxs-lookup"><span data-stu-id="c7880-198">application/json.</span></span> <span data-ttu-id="c7880-199">Required.</span><span class="sxs-lookup"><span data-stu-id="c7880-199">Required.</span></span> |
| <span data-ttu-id="c7880-200">Prefer</span><span class="sxs-lookup"><span data-stu-id="c7880-200">Prefer</span></span> | <span data-ttu-id="c7880-201">string</span><span class="sxs-lookup"><span data-stu-id="c7880-201">string</span></span>  | <span data-ttu-id="c7880-202">odata.maxpagesize={x}.</span><span class="sxs-lookup"><span data-stu-id="c7880-202">odata.maxpagesize={x}.</span></span> <span data-ttu-id="c7880-203">Optional.</span><span class="sxs-lookup"><span data-stu-id="c7880-203">Optional.</span></span> |
| <span data-ttu-id="c7880-204">Prefer</span><span class="sxs-lookup"><span data-stu-id="c7880-204">Prefer</span></span> | <span data-ttu-id="c7880-205">string</span><span class="sxs-lookup"><span data-stu-id="c7880-205">string</span></span> | <span data-ttu-id="c7880-206">Outlook. TimeZone = {строка часового пояса}.</span><span class="sxs-lookup"><span data-stu-id="c7880-206">outlook.timezone={Time zone string}.</span></span> <span data-ttu-id="c7880-207">Необязательное, в формате UTC предполагается, что отсутствует.</span><span class="sxs-lookup"><span data-stu-id="c7880-207">Optional, UTC assumed if absent.</span></span>|

## <a name="response"></a><span data-ttu-id="c7880-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7880-208">Response</span></span>

### <a name="delta-function-on-events-preview"></a><span data-ttu-id="c7880-209">Функция Delta для событий (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="c7880-209">Delta function on events (preview)</span></span>
<span data-ttu-id="c7880-210">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию [событий](../resources/event.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7880-210">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) collection in the response body.</span></span> <span data-ttu-id="c7880-211">Каждое **событие** в ответе содержит только свойства **ID**, **Type**, **Start** и **End** для повышения производительности.</span><span class="sxs-lookup"><span data-stu-id="c7880-211">Each **event** in the response contains only the **id**, **type**, **start** and **end** properties for performance reasons.</span></span> <span data-ttu-id="c7880-212">Используйте `GET /events/{id}` последовательное, чтобы развернуть все события из отклика.</span><span class="sxs-lookup"><span data-stu-id="c7880-212">Use `GET /events/{id}` subsequently to expand any events from the response.</span></span>  

### <a name="delta-function-on-calendarview"></a><span data-ttu-id="c7880-213">Функция Delta в calendarView</span><span class="sxs-lookup"><span data-stu-id="c7880-213">Delta function on calendarView</span></span>
<span data-ttu-id="c7880-214">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию [событий](../resources/event.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7880-214">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) collection in the response body.</span></span>

<span data-ttu-id="c7880-215">Ожидается получение всех свойств, которые вы обычно получаете из `GET /calendarview` запроса.</span><span class="sxs-lookup"><span data-stu-id="c7880-215">Expect to get all the properties you'd normally get from a `GET /calendarview` request.</span></span> 

## <a name="examples"></a><span data-ttu-id="c7880-216">Примеры</span><span class="sxs-lookup"><span data-stu-id="c7880-216">Examples</span></span>

### <a name="example-1-delta-function-on-events-in-a-calendar-preview"></a><span data-ttu-id="c7880-217">Пример 1: функция Delta для событий в календаре (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="c7880-217">Example 1: Delta function on events in a calendar (preview)</span></span>
#### <a name="request"></a><span data-ttu-id="c7880-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7880-218">Request</span></span>
<span data-ttu-id="c7880-219">В следующем примере показан первоначальный запрос на синхронизацию для получения событий в календаре пользователя, вошедшего в систему по умолчанию, которые происходят в указанном параметре или после него `startDateTime` .</span><span class="sxs-lookup"><span data-stu-id="c7880-219">The following example shows the initial sync request to get events in the signed-in user's default calendar, that occur on or after the specified `startDateTime` parameter.</span></span> <span data-ttu-id="c7880-220">Исходный запрос не включает никаких маркеров состояния.</span><span class="sxs-lookup"><span data-stu-id="c7880-220">The initial request does not include any state token.</span></span> 

<span data-ttu-id="c7880-221">В запросе используется `Prefer: odata.maxpagesize` заголовок, чтобы ограничить максимальное количество событий в каждом ответе на 1.</span><span class="sxs-lookup"><span data-stu-id="c7880-221">The request uses the `Prefer: odata.maxpagesize` header to limit the maximum number of events in each response to 1.</span></span> <span data-ttu-id="c7880-222">Продолжайте вызывать `delta` функцию с помощью запроса, возвращенного в `@odata.nextLink` `@odata.deltaLink` ответе.</span><span class="sxs-lookup"><span data-stu-id="c7880-222">Continue calling the `delta` function by using the query returned in `@odata.nextLink` until you get a `@odata.deltaLink` in the response.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_delta_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar/events/delta?startDateTime=2020-06-12T00:00:00Z

Prefer: odata.maxpagesize=1
```

#### <a name="response"></a><span data-ttu-id="c7880-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7880-223">Response</span></span>

<span data-ttu-id="c7880-224">Если запрос выполнен успешно, ответ включает маркер состояния, который является либо _skipToken_ (в заголовке ответа _ \@ OData. NextLink_ ), либо _deltaToken_ (в заголовке ответа _ \@ OData. deltaLink_ ).</span><span class="sxs-lookup"><span data-stu-id="c7880-224">If the request is successful, the response includes a state token, which is either a _skipToken_ (in an _\@odata.nextLink_ response header) or a _deltaToken_ (in an _\@odata.deltaLink_ response header).</span></span>
<span data-ttu-id="c7880-225">В соответствии с этим они указывают, следует ли продолжать работу со циклом или вы завершили сбор всех изменений для этого цикла.</span><span class="sxs-lookup"><span data-stu-id="c7880-225">Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="c7880-226">Приведенный ниже ответ показывает _skipToken_ в заголовке ответа _ \@ OData. nextLink_ .</span><span class="sxs-lookup"><span data-stu-id="c7880-226">The response below shows a _skipToken_ in an _\@odata.nextLink_ response header.</span></span>

<!-- {
  "blockType": "response",
  "name": "event_delta_events",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/calendar/events/delta?$skiptoken=R0usmcdvmMu7jxWP8",
  "value": [
    { 
      "id": " AAMkADllMWMwNDkzLWJlY2EtNDIyOS1iZjAA=", 
      "type": "singleInstance", 
      "start": {  
             "DateTime": "2020-02-19T10:00:00.0000000",  
             "TimeZone": "UTC" 
         },  
       "end": {  
                "DateTime": "2020-02-19T11:00:00.0000000",  
                "TimeZone": "UTC"        
          }  
        } 
  ]
}
```


### <a name="example-2-delta-function-on-calendarview"></a><span data-ttu-id="c7880-227">Пример 2: функция Delta в calendarView</span><span class="sxs-lookup"><span data-stu-id="c7880-227">Example 2: Delta function on calendarView</span></span>
#### <a name="request"></a><span data-ttu-id="c7880-228">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7880-228">Request</span></span>

<span data-ttu-id="c7880-229">В приведенном ниже примере показан первоначальный запрос на синхронизацию для получения событий в указанном календаре вошедшего пользователя, в диапазоне дат, указанном с помощью **calendarView**.</span><span class="sxs-lookup"><span data-stu-id="c7880-229">The following example shows the initial sync request to get events in the specified calendar of the signed-in user, within the range of dates indicated by the **calendarView**.</span></span> <span data-ttu-id="c7880-230">Исходный запрос не включает никаких маркеров состояния.</span><span class="sxs-lookup"><span data-stu-id="c7880-230">The initial request does not include any state token.</span></span> 

<span data-ttu-id="c7880-231">В запросе используется `Prefer: odata.maxpagesize` заголовок, чтобы ограничить максимальное количество событий в каждом ответе на 2.</span><span class="sxs-lookup"><span data-stu-id="c7880-231">The request uses the `Prefer: odata.maxpagesize` header to limit the maximum number of events in each response to 2.</span></span> <span data-ttu-id="c7880-232">Продолжите вызов `delta` функции с помощью запроса, возвращенного, `@odata.nextLink` пока не будут получены все события в представлении календаря и `@odata.deltaLink` в ответе.</span><span class="sxs-lookup"><span data-stu-id="c7880-232">Continue calling the `delta` function by using the query returned in `@odata.nextLink` until you get all the events in that calendar view, and a `@odata.deltaLink` in the response.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7880-233">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7880-233">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADI5M1BbeAAA="],
  "name": "event_delta_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendars/AAMkADI5M1BbeAAA=/calendarview/delta?startDateTime=2020-06-01T00:00:00Z&endDateTime=2020-06-10T00:00:00Z

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="c7880-234">C#</span><span class="sxs-lookup"><span data-stu-id="c7880-234">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-delta-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7880-235">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7880-235">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-delta-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c7880-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7880-236">Response</span></span>

<span data-ttu-id="c7880-237">Если запрос выполнен успешно, ответ включает маркер состояния, который является либо _skipToken_ (в заголовке ответа _ \@ OData. NextLink_ ), либо _deltaToken_ (в заголовке ответа _ \@ OData. deltaLink_ ).</span><span class="sxs-lookup"><span data-stu-id="c7880-237">If the request is successful, the response includes a state token, which is either a _skipToken_ (in an _\@odata.nextLink_ response header) or a _deltaToken_ (in an _\@odata.deltaLink_ response header).</span></span>
<span data-ttu-id="c7880-238">В соответствии с этим они указывают, следует ли продолжать работу со циклом или вы завершили сбор всех изменений для этого цикла.</span><span class="sxs-lookup"><span data-stu-id="c7880-238">Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="c7880-239">Приведенный ниже ответ показывает _skipToken_ в заголовке ответа _ \@ OData. nextLink_ .</span><span class="sxs-lookup"><span data-stu-id="c7880-239">The response below shows a _skipToken_ in an _\@odata.nextLink_ response header.</span></span>

<span data-ttu-id="c7880-240">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c7880-240">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "name": "event_delta_calendarview",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(event)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/calendars/AAMkADI5M1BbeAAA=/calendarview/delta?$skiptoken=R0usmcdvmMu7jxWP8",
    "value": [
        {
            "@odata.type": "#microsoft.graph.event",
            "@odata.etag": "W/\"Jdsb3FEkPk2qoUHCdliYowACwixTgw==\"",
            "createdDateTime": "2020-06-16T04:05:43.8668791Z",
            "lastModifiedDateTime": "2020-06-16T04:08:27.354268Z",
            "changeKey": "Jdsb3FEkPk2qoUHCdliYowACwixTgw==",
            "categories": [],
            "transactionId": null,
            "originalStartTimeZone": "Pacific Standard Time",
            "originalEndTimeZone": "Pacific Standard Time",
            "uid": "040000008200E00074C5B7101A82E00800000000F088B8B95843D601000000000000000010000000165CD5547CFC9545B6492B261750B48C",
            "reminderMinutesBeforeStart": 15,
            "isReminderOn": false,
            "hasAttachments": false,
            "subject": "Summer party",
            "bodyPreview": "",
            "importance": "normal",
            "sensitivity": "normal",
            "isAllDay": false,
            "isCancelled": false,
            "isOrganizer": true,
            "IsRoomRequested": false,
            "AutoRoomBookingStatus": "None",
            "responseRequested": true,
            "seriesMasterId": null,
            "showAs": "busy",
            "type": "singleInstance",
            "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADI5MAAKkeE1QAAA%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl": null,
            "isOnlineMeeting": false,
            "onlineMeetingProvider": "unknown",
            "allowNewTimeProposals": true,
            "OccurrenceId": null,
            "isDraft": false,
            "recurrence": null,
            "AutoRoomBookingOptions": null,
            "onlineMeeting": null,
            "id": "AAMkADI5MAAKkeE1QAAA=",
            "responseStatus": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "body": {
                "contentType": "html",
                "content": "<html>\r\n<head></head>\r\n<body lang=\"EN-US\" link=\"#0563C1\" vlink=\"#954F72\" style=\"\">\r\n<div class=\"WordSection1\">\r\n<p class=\"MsoNormal\">&nbsp;</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
            },
            "start": {
                "dateTime": "2020-06-02T20:00:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2020-06-02T22:30:00.0000000",
                "timeZone": "UTC"
            },
            "location": {
                "displayName": "",
                "locationType": "default",
                "uniqueIdType": "unknown",
                "address": {
                    "type": "unknown"
                },
                "coordinates": {}
            },
            "locations": [],
            "attendees": [
                {
                    "type": "required",
                    "status": {
                        "response": "none",
                        "time": "0001-01-01T00:00:00Z"
                    },
                    "emailAddress": {
                        "name": "Samantha Booth",
                        "address": "samanthab@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer": {
                "emailAddress": {
                    "name": "Samantha Booth",
                    "address": "samanthab@contoso.onmicrosoft.com"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.event",
            "@odata.etag": "W/\"Jdsb3FEkPk2qoUHCdliYowACwixTfw==\"",
            "createdDateTime": "2020-06-16T04:06:18.386713Z",
            "lastModifiedDateTime": "2020-06-16T04:08:19.5694048Z",
            "changeKey": "Jdsb3FEkPk2qoUHCdliYowACwixTfw==",
            "categories": [],
            "transactionId": null,
            "originalStartTimeZone": "Pacific Standard Time",
            "originalEndTimeZone": "Pacific Standard Time",
            "uid": "040000008200E00074C5B7101A82E0080000000060074BC55843D6010000000000000000100000002D33A89F36B10D43A12FD990B62858B2",
            "reminderMinutesBeforeStart": 15,
            "isReminderOn": true,
            "hasAttachments": false,
            "subject": "Summer party part 2",
            "bodyPreview": "",
            "importance": "normal",
            "sensitivity": "normal",
            "isAllDay": false,
            "isCancelled": false,
            "isOrganizer": true,
            "IsRoomRequested": false,
            "AutoRoomBookingStatus": "None",
            "responseRequested": true,
            "seriesMasterId": null,
            "showAs": "busy",
            "type": "singleInstance",
            "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADI5MAAKkeE1RAAA%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl": null,
            "isOnlineMeeting": false,
            "onlineMeetingProvider": "unknown",
            "allowNewTimeProposals": true,
            "OccurrenceId": null,
            "isDraft": false,
            "recurrence": null,
            "AutoRoomBookingOptions": null,
            "onlineMeeting": null,
            "id": "AAMkADI5MAAKkeE1RAAA=",
            "responseStatus": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "body": {
                "contentType": "html",
                "content": "<html>\r\n<head></head>\r\n<body lang=\"EN-US\" link=\"#0563C1\" vlink=\"#954F72\" style=\"\">\r\n<div class=\"WordSection1\">\r\n<p class=\"MsoNormal\">&nbsp;</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
            },
            "start": {
                "dateTime": "2020-06-04T19:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2020-06-04T22:30:00.0000000",
                "timeZone": "UTC"
            },
            "location": {
                "displayName": "",
                "locationType": "default",
                "uniqueIdType": "unknown",
                "address": {
                    "type": "unknown"
                },
                "coordinates": {}
            },
            "locations": [],
            "attendees": [
                {
                    "type": "required",
                    "status": {
                        "response": "none",
                        "time": "0001-01-01T00:00:00Z"
                    },
                    "emailAddress": {
                        "name": "Samantha Booth",
                        "address": "samanthab@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer": {
                "emailAddress": {
                    "name": "Samantha Booth",
                    "address": "samanthab@contoso.onmicrosoft.com"
                }
            }
        }
    ]
}
```

### <a name="see-also"></a><span data-ttu-id="c7880-241">См. также</span><span class="sxs-lookup"><span data-stu-id="c7880-241">See also</span></span>

- [<span data-ttu-id="c7880-242">Запрос изменений Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c7880-242">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="c7880-243">Получение добавочных изменений для событий в папке</span><span class="sxs-lookup"><span data-stu-id="c7880-243">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
