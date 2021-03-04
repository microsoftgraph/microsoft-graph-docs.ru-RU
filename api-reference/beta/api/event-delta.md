---
title: 'event: delta'
description: Получение списка событий, которые были добавлены в **calendarView** (диапазон событий), обновлены в нем или удалены из него
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: efa0768fbb8cae441afc3d1fd48baa2e2a3567da
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436248"
---
# <a name="event-delta"></a><span data-ttu-id="1bed0-103">event: delta</span><span class="sxs-lookup"><span data-stu-id="1bed0-103">event: delta</span></span>

<span data-ttu-id="1bed0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bed0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bed0-105">Получите набор ресурсов [событий,](../resources/event.md) которые были добавлены, удалены или обновлены в одном или более календарях.</span><span class="sxs-lookup"><span data-stu-id="1bed0-105">Get a set of [event](../resources/event.md) resources that have been added, deleted, or updated in one or more calendars.</span></span> 

<span data-ttu-id="1bed0-106">Вы можете получить определенные типы этих дополнительных изменений в событиях во всех календарях почтового ящика или в определенном календаре или в коллекции событий **calendarView** (диапазон событий, определенных датами начала и окончания) календаря.</span><span class="sxs-lookup"><span data-stu-id="1bed0-106">You can get specific types of these incremental changes in the events in all the calendars of a mailbox or in a specific calendar, or in an event collection of a **calendarView** (range of events defined by start and end dates) of a calendar.</span></span> <span data-ttu-id="1bed0-107">Календарь может быть календарем по умолчанию или другим указанным календарем пользователя.</span><span class="sxs-lookup"><span data-stu-id="1bed0-107">The calendar can be the default calendar or some other specified calendar of the user's.</span></span> <span data-ttu-id="1bed0-108">В случае получения дополнительных изменений **в calendarView** календарь также может быть групповым.</span><span class="sxs-lookup"><span data-stu-id="1bed0-108">In the case of getting incremental changes on **calendarView**, the calendar can be a group calendar as well.</span></span>

<span data-ttu-id="1bed0-109">Вызов  функции дельты похож на запрос или запрос указанного календаря, за исключением того, что, надлежащим образом применяя маркеры состояния в одном или несколько из этих вызовов, можно запрашивать дополнительные изменения событий в этом `GET /events` календаре. `GET /calendarview` [](/graph/delta-query-overview#state-tokens)</span><span class="sxs-lookup"><span data-stu-id="1bed0-109">A **delta** function call is similar to a `GET /events` or `GET /calendarview` request for the specified calendar, except that by appropriately applying [state tokens](/graph/delta-query-overview#state-tokens) in one or more of these calls, you can query for incremental changes of events in that calender.</span></span> <span data-ttu-id="1bed0-110">Это позволяет поддерживать и синхронизировать локальный магазин событий в указанном календаре, не извлекая все события календаря с сервера каждый раз.</span><span class="sxs-lookup"><span data-stu-id="1bed0-110">This allows you to maintain and synchronize a local store of events in the specified calendar, without having to fetch all the events of that calendar from the server every time.</span></span>

<span data-ttu-id="1bed0-111">В следующей таблице перечислены различия между функцией **дельты** событий и функцией дельты в **calendarView** в календаре. </span><span class="sxs-lookup"><span data-stu-id="1bed0-111">The following table lists the differences between the **delta** function on events and the **delta** function on a **calendarView** in a calendar.</span></span>

| <span data-ttu-id="1bed0-112">Функция Delta в событиях</span><span class="sxs-lookup"><span data-stu-id="1bed0-112">Delta function on events</span></span>  | <span data-ttu-id="1bed0-113">Функция Delta в calendarView</span><span class="sxs-lookup"><span data-stu-id="1bed0-113">Delta function on calendarView</span></span>  |
|:--------------------------|:---------------------------------------------------------|
| <span data-ttu-id="1bed0-114">Получает дополнительные изменения всех событий в календаре, не ограниченных диапазоном даты начала и окончания.</span><span class="sxs-lookup"><span data-stu-id="1bed0-114">Gets incremental changes of all the events in a calendar not bounded by a start and end date range.</span></span> <span data-ttu-id="1bed0-115">Кроме того, можно получить дополнительные изменения событий в календаре, ограниченных временем начала, начиная с этой даты или после нее.</span><span class="sxs-lookup"><span data-stu-id="1bed0-115">Alternatively, you can get incremental changes of the events in a calendar bounded by a start time, starting on or after that date/time.</span></span> | <span data-ttu-id="1bed0-116">Получает дополнительные изменения событий в начале и конце **календаря.**</span><span class="sxs-lookup"><span data-stu-id="1bed0-116">Gets incremental changes of events within the start and end date/time of the **calendarView**.</span></span> |
| <span data-ttu-id="1bed0-117">Возвращает только ограниченный набор **свойств событий** по соображениям производительности.</span><span class="sxs-lookup"><span data-stu-id="1bed0-117">Returns only a limited set of **event** properties for performance reasons.</span></span> <span data-ttu-id="1bed0-118">Клиент для последующего использования `GET /events/{id}` для расширения любых событий.</span><span class="sxs-lookup"><span data-stu-id="1bed0-118">Client to subsequently use `GET /events/{id}` to expand any events.</span></span> | <span data-ttu-id="1bed0-119">Расширение на стороне сервера возвращает более полный набор **свойств** событий.</span><span class="sxs-lookup"><span data-stu-id="1bed0-119">Server-side expansion returns a fuller set of **event** properties.</span></span> |
| <span data-ttu-id="1bed0-120">Ответ включает в себя отдельные экземпляры и повторяющийся мастер серии.</span><span class="sxs-lookup"><span data-stu-id="1bed0-120">Response includes single instances and recurring series master.</span></span> | <span data-ttu-id="1bed0-121">Ответ включает в себя отдельные экземпляры, а также случаи и исключения повторяющихся серий.</span><span class="sxs-lookup"><span data-stu-id="1bed0-121">Response includes single instances, and occurrences and exceptions of recurring series.</span></span> |
| <span data-ttu-id="1bed0-122">Применяется к событиям в календарях пользователей, но не к групповым календарям.</span><span class="sxs-lookup"><span data-stu-id="1bed0-122">Applies to events in user calendars but not group calendars.</span></span> | <span data-ttu-id="1bed0-123">Применяется к событиям в пользовательском и групповом календарях.</span><span class="sxs-lookup"><span data-stu-id="1bed0-123">Applies to events in user and group calendars.</span></span> |
| <span data-ttu-id="1bed0-124">В настоящее время доступно только в бета-версии.</span><span class="sxs-lookup"><span data-stu-id="1bed0-124">Currently available only in the beta version.</span></span> | <span data-ttu-id="1bed0-125">Доступно в версиях v1.0 и бета-версии.</span><span class="sxs-lookup"><span data-stu-id="1bed0-125">Available in the v1.0 and beta versions.</span></span> |

## <a name="permissions"></a><span data-ttu-id="1bed0-126">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1bed0-126">Permissions</span></span>
<span data-ttu-id="1bed0-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bed0-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bed0-129">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bed0-129">Permission type</span></span>      | <span data-ttu-id="1bed0-130">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bed0-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bed0-131">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bed0-131">Delegated (work or school account)</span></span> | <span data-ttu-id="1bed0-132">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1bed0-132">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="1bed0-133">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bed0-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bed0-134">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1bed0-134">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="1bed0-135">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1bed0-135">Application</span></span> | <span data-ttu-id="1bed0-136">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1bed0-136">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bed0-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bed0-137">HTTP request</span></span>

<span data-ttu-id="1bed0-138">В этом разделе показан синтаксис  http-запроса для начального вызова функции дельты для запуска полной синхронизации, которая извлекает все события в заданном представлении календаря или календаря.</span><span class="sxs-lookup"><span data-stu-id="1bed0-138">This section shows the HTTP request syntax for the initial **delta** function call to start a full synchronization that retrieves all the events in the specified calendar or calendar view.</span></span> <span data-ttu-id="1bed0-139">Этот синтаксис не содержит никаких [маркеров состояния.](/graph/delta-query-overview#state-tokens)</span><span class="sxs-lookup"><span data-stu-id="1bed0-139">This syntax does not contain any [state tokens](/graph/delta-query-overview#state-tokens).</span></span> 

<span data-ttu-id="1bed0-140">URL-адрес запроса, возвращенный в успешном ответе, включает `nextLink` `deltaLink` маркер состояния.</span><span class="sxs-lookup"><span data-stu-id="1bed0-140">The query URL returned in a `nextLink` or `deltaLink` of a successful response includes a state token.</span></span> <span data-ttu-id="1bed0-141">Для любого последующего **вызова функции дельты** используйте URL-адрес запроса в предшествующего `nextLink` или `deltaLink` предшествующего вызова.</span><span class="sxs-lookup"><span data-stu-id="1bed0-141">For any subsequent **delta** function call, use the query URL in a `nextLink` or `deltaLink` preceding it.</span></span>

### <a name="delta-function-on-events-in-a-user-calendar-preview"></a><span data-ttu-id="1bed0-142">Функция Delta в событиях в пользовательском календаре (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="1bed0-142">Delta function on events in a user calendar (preview)</span></span>
<span data-ttu-id="1bed0-143">Применение **функции дельты** для всех событий или событий, начиная с определенной даты или времени в указанном пользовательском календаре (s):</span><span class="sxs-lookup"><span data-stu-id="1bed0-143">Apply the **delta** function on all the events or events starting on or after a specific date/time, in the specified user calendar(s):</span></span>

* <span data-ttu-id="1bed0-144">Чтобы получить дополнительные изменения всех событий или событий, начиная с указанной даты или времени в почтовом ящике _пользователя:_</span><span class="sxs-lookup"><span data-stu-id="1bed0-144">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the user's mailbox_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/events/delta 
  GET /users/{id | userPrincipalName}/events/delta 

  GET /me/events/delta?startDateTime={start_datetime}
  GET /users/{id | userPrincipalName}/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="1bed0-145">Чтобы получить дополнительные изменения всех событий или событий, начиная с указанной даты или времени в календаре по умолчанию _пользователя:_</span><span class="sxs-lookup"><span data-stu-id="1bed0-145">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the user's default calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendar/events/delta 
  GET /users/{id | userPrincipalName}/calendar/events/delta 

  GET /me/calendar/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendar/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="1bed0-146">Чтобы получить дополнительные изменения всех событий или событий, начиная с указанной даты или времени в указанном пользовательском календаре:</span><span class="sxs-lookup"><span data-stu-id="1bed0-146">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the specified user calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta 

  GET /me/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="1bed0-147">Чтобы получить дополнительные изменения всех событий или событий, начиная с указанной даты или времени в указанной группе календаря и _календаре:_</span><span class="sxs-lookup"><span data-stu-id="1bed0-147">To get incremental changes all the events, or of events starting on or after the specified date/time _in the specified calendar group and calendar_:</span></span>
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

### <a name="delta-function-on-calendarview-in-a-user-calendar"></a><span data-ttu-id="1bed0-148">Функция Delta в calendarView в пользовательском календаре</span><span class="sxs-lookup"><span data-stu-id="1bed0-148">Delta function on calendarView in a user calendar</span></span>
<span data-ttu-id="1bed0-149">Применение **функции дельты** для ряда событий, делимитированные по дате начала и окончания/времени, в указанном пользовательском календаре:</span><span class="sxs-lookup"><span data-stu-id="1bed0-149">Apply the **delta** function on a range of events delimited by start and end date/times, in the specified user calendar:</span></span>

* <span data-ttu-id="1bed0-150">Чтобы получить дополнительные изменения в представлении календаря календаря пользователя по _умолчанию:_</span><span class="sxs-lookup"><span data-stu-id="1bed0-150">To get incremental changes in a calendar view of _the user's default calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

* <span data-ttu-id="1bed0-151">Чтобы получить дополнительные изменения в представлении календаря указанного _пользовательского календаря:_</span><span class="sxs-lookup"><span data-stu-id="1bed0-151">To get incremental changes in a calendar view of _the specified user calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

### <a name="delta-function-on-calendarview-in-a-group-calendar"></a><span data-ttu-id="1bed0-152">Функция Delta в calendarView в групповом календаре</span><span class="sxs-lookup"><span data-stu-id="1bed0-152">Delta function on calendarView in a group calendar</span></span>
* <span data-ttu-id="1bed0-153">Чтобы получить дополнительные изменения в представлении календаря календаря _группы:_</span><span class="sxs-lookup"><span data-stu-id="1bed0-153">To get incremental changes in a calendar view of _a group's calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

## <a name="query-parameters"></a><span data-ttu-id="1bed0-154">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="1bed0-154">Query parameters</span></span>

<span data-ttu-id="1bed0-155">Отслеживание изменений вызывает один или несколько вызовов функции **дельты.**</span><span class="sxs-lookup"><span data-stu-id="1bed0-155">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="1bed0-156">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="1bed0-156">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="1bed0-157">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="1bed0-157">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="1bed0-158">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="1bed0-158">You only need to specify any desired query parameters once upfront.</span></span>
<span data-ttu-id="1bed0-159">В последующих запросах просто скопируйте и примените URL-адрес из предыдущего ответа, так как этот URL-адрес уже содержит закодированные `nextLink` `deltaLink` и нужные параметры.</span><span class="sxs-lookup"><span data-stu-id="1bed0-159">In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="1bed0-160">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="1bed0-160">Query parameter</span></span>      | <span data-ttu-id="1bed0-161">Тип</span><span class="sxs-lookup"><span data-stu-id="1bed0-161">Type</span></span>   |<span data-ttu-id="1bed0-162">Описание</span><span class="sxs-lookup"><span data-stu-id="1bed0-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1bed0-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1bed0-163">startDateTime</span></span>|<span data-ttu-id="1bed0-164">String</span><span class="sxs-lookup"><span data-stu-id="1bed0-164">String</span></span>|<span data-ttu-id="1bed0-p109">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2019-11-08T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="1bed0-p109">The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00". </span></span><br><span data-ttu-id="1bed0-167">Часовой пояс указывается в смещенной части часового пояса значения параметра и при этом не влияет на `Prefer: outlook.timezone` заглавный заглавный.</span><span class="sxs-lookup"><span data-stu-id="1bed0-167">The timezone is specified in the timezone offset portion of the parameter value, and is not impacted by the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="1bed0-168">Если в значении не указано смещение часового пояса, оно интерпретируется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="1bed0-168">If no timezone offset is included in the value, it is interpreted as UTC.</span></span><br><span data-ttu-id="1bed0-169">Необязательный **для дельты** событий в календаре.</span><span class="sxs-lookup"><span data-stu-id="1bed0-169">Optional for **delta** on events in a calendar.</span></span> <br><span data-ttu-id="1bed0-170">Необходимый для **дельты** **в calendarView**.</span><span class="sxs-lookup"><span data-stu-id="1bed0-170">Required for **delta** on **calendarView**.</span></span> |
|<span data-ttu-id="1bed0-171">endDateTime</span><span class="sxs-lookup"><span data-stu-id="1bed0-171">endDateTime</span></span>|<span data-ttu-id="1bed0-172">String</span><span class="sxs-lookup"><span data-stu-id="1bed0-172">String</span></span>|<span data-ttu-id="1bed0-p111">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2019-11-08T20:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="1bed0-p111">The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00". </span></span><br><span data-ttu-id="1bed0-175">Часовой пояс указывается в смещенной части часового пояса значения параметра и при этом не влияет на `Prefer: outlook.timezone` заглавный заглавный.</span><span class="sxs-lookup"><span data-stu-id="1bed0-175">The timezone is specified in the timezone offset portion of the parameter value, and is not impacted by the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="1bed0-176">Если в значении не указано смещение часового пояса, оно интерпретируется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="1bed0-176">If no timezone offset is included in the value, it is interpreted as UTC.</span></span><br><span data-ttu-id="1bed0-177">_Не поддерживается_ **дельта** на событиях в календаре.</span><span class="sxs-lookup"><span data-stu-id="1bed0-177">_Not supported_ by **delta** on events in a calendar.</span></span> <br><span data-ttu-id="1bed0-178">Необходимый для **дельты** **в calendarView**.</span><span class="sxs-lookup"><span data-stu-id="1bed0-178">Required for **delta** on **calendarView**.</span></span>|
| <span data-ttu-id="1bed0-179">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="1bed0-179">$deltatoken</span></span> | <span data-ttu-id="1bed0-180">string</span><span class="sxs-lookup"><span data-stu-id="1bed0-180">string</span></span> | <span data-ttu-id="1bed0-p113">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` при предыдущем вызове функции **delta** для этого же представления календаря и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этого представления календаря.</span><span class="sxs-lookup"><span data-stu-id="1bed0-p113">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same calendar view, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that calendar view.</span></span>|
| <span data-ttu-id="1bed0-183">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="1bed0-183">$skiptoken</span></span> | <span data-ttu-id="1bed0-184">string</span><span class="sxs-lookup"><span data-stu-id="1bed0-184">string</span></span> | <span data-ttu-id="1bed0-185">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` при предыдущем вызове функции **delta** и указывает на то, что в представлении календаря остаются не отслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="1bed0-185">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same calendar view.</span></span> |

<span data-ttu-id="1bed0-186">Не поддерживает `$expand` `$filter` , , , и `$orderby` `$select` `$search` .</span><span class="sxs-lookup"><span data-stu-id="1bed0-186">Does not support `$expand`, `$filter`, `$orderby`, `$select`, and `$search`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="1bed0-187">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bed0-187">Request headers</span></span>
| <span data-ttu-id="1bed0-188">Имя</span><span class="sxs-lookup"><span data-stu-id="1bed0-188">Name</span></span>       | <span data-ttu-id="1bed0-189">Тип</span><span class="sxs-lookup"><span data-stu-id="1bed0-189">Type</span></span> | <span data-ttu-id="1bed0-190">Описание</span><span class="sxs-lookup"><span data-stu-id="1bed0-190">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="1bed0-191">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bed0-191">Authorization</span></span>  | <span data-ttu-id="1bed0-192">string</span><span class="sxs-lookup"><span data-stu-id="1bed0-192">string</span></span>  | <span data-ttu-id="1bed0-p114">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bed0-p114">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1bed0-195">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1bed0-195">Content-Type</span></span>  | <span data-ttu-id="1bed0-196">string</span><span class="sxs-lookup"><span data-stu-id="1bed0-196">string</span></span>  | <span data-ttu-id="1bed0-p115">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bed0-p115">application/json. Required.</span></span> |
| <span data-ttu-id="1bed0-199">Prefer</span><span class="sxs-lookup"><span data-stu-id="1bed0-199">Prefer</span></span> | <span data-ttu-id="1bed0-200">string</span><span class="sxs-lookup"><span data-stu-id="1bed0-200">string</span></span>  | <span data-ttu-id="1bed0-p116">odata.maxpagesize={x}. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="1bed0-p116">odata.maxpagesize={x}. Optional.</span></span> |
| <span data-ttu-id="1bed0-203">Prefer</span><span class="sxs-lookup"><span data-stu-id="1bed0-203">Prefer</span></span> | <span data-ttu-id="1bed0-204">string</span><span class="sxs-lookup"><span data-stu-id="1bed0-204">string</span></span> | <span data-ttu-id="1bed0-205">outlook.timezone={Time zone string}.</span><span class="sxs-lookup"><span data-stu-id="1bed0-205">outlook.timezone={Time zone string}.</span></span> <span data-ttu-id="1bed0-206">Необязательный, UTC предполагается, если отсутствует.</span><span class="sxs-lookup"><span data-stu-id="1bed0-206">Optional, UTC assumed if absent.</span></span>|

## <a name="response"></a><span data-ttu-id="1bed0-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bed0-207">Response</span></span>

### <a name="delta-function-on-events-preview"></a><span data-ttu-id="1bed0-208">Функция Delta в событиях (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="1bed0-208">Delta function on events (preview)</span></span>
<span data-ttu-id="1bed0-209">В случае успешной работы этот метод возвращает код отклика и коллекцию событий `200 OK` в тексте [](../resources/event.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="1bed0-209">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) collection in the response body.</span></span> <span data-ttu-id="1bed0-210">**Каждое** событие в ответе содержит только свойства **id,** **type,** **start** и **end** по соображениям производительности.</span><span class="sxs-lookup"><span data-stu-id="1bed0-210">Each **event** in the response contains only the **id**, **type**, **start** and **end** properties for performance reasons.</span></span> <span data-ttu-id="1bed0-211">Используйте `GET /events/{id}` впоследствии для расширения любых событий из ответа.</span><span class="sxs-lookup"><span data-stu-id="1bed0-211">Use `GET /events/{id}` subsequently to expand any events from the response.</span></span>  

### <a name="delta-function-on-calendarview"></a><span data-ttu-id="1bed0-212">Функция Delta в calendarView</span><span class="sxs-lookup"><span data-stu-id="1bed0-212">Delta function on calendarView</span></span>
<span data-ttu-id="1bed0-213">В случае успешной работы этот метод возвращает код отклика и коллекцию событий `200 OK` в тексте [](../resources/event.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="1bed0-213">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) collection in the response body.</span></span>

<span data-ttu-id="1bed0-214">Ожидайте получения всех свойств, которые обычно получаются из `GET /calendarview` запроса.</span><span class="sxs-lookup"><span data-stu-id="1bed0-214">Expect to get all the properties you'd normally get from a `GET /calendarview` request.</span></span> 

## <a name="examples"></a><span data-ttu-id="1bed0-215">Примеры</span><span class="sxs-lookup"><span data-stu-id="1bed0-215">Examples</span></span>

### <a name="example-1-delta-function-on-events-in-a-calendar-preview"></a><span data-ttu-id="1bed0-216">Пример 1. Функция Delta для событий в календаре (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="1bed0-216">Example 1: Delta function on events in a calendar (preview)</span></span>
#### <a name="request"></a><span data-ttu-id="1bed0-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bed0-217">Request</span></span>
<span data-ttu-id="1bed0-218">В следующем примере показан начальный запрос на синхронизацию для получения событий в календаре по умолчанию пользователя, которые происходят в указанном параметре или после `startDateTime` него.</span><span class="sxs-lookup"><span data-stu-id="1bed0-218">The following example shows the initial sync request to get events in the signed-in user's default calendar, that occur on or after the specified `startDateTime` parameter.</span></span> <span data-ttu-id="1bed0-219">Начальный запрос не включает какой-либо маркер состояния.</span><span class="sxs-lookup"><span data-stu-id="1bed0-219">The initial request does not include any state token.</span></span> 

<span data-ttu-id="1bed0-220">Запрос использует заглавную для ограничения максимального количества событий в `Prefer: odata.maxpagesize` каждом ответе до 1.</span><span class="sxs-lookup"><span data-stu-id="1bed0-220">The request uses the `Prefer: odata.maxpagesize` header to limit the maximum number of events in each response to 1.</span></span> <span data-ttu-id="1bed0-221">Продолжайте вызывать функцию с помощью возвращенного запроса, `delta` `@odata.nextLink` пока не получите `@odata.deltaLink` ответ.</span><span class="sxs-lookup"><span data-stu-id="1bed0-221">Continue calling the `delta` function by using the query returned in `@odata.nextLink` until you get a `@odata.deltaLink` in the response.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_delta_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar/events/delta?startDateTime=2020-06-12T00:00:00Z

Prefer: odata.maxpagesize=1
```

#### <a name="response"></a><span data-ttu-id="1bed0-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bed0-222">Response</span></span>

<span data-ttu-id="1bed0-223">Если запрос является успешным, в ответ включается маркер состояния, который является либо _skipToken_ (в загоне ответа _\@ odata.nextLink)_ или _deltaToken_ (в загоне ответа _\@ odata.deltaLink)._</span><span class="sxs-lookup"><span data-stu-id="1bed0-223">If the request is successful, the response includes a state token, which is either a _skipToken_ (in an _\@odata.nextLink_ response header) or a _deltaToken_ (in an _\@odata.deltaLink_ response header).</span></span>
<span data-ttu-id="1bed0-224">Соответственно, они указывают, следует ли продолжить раунд или вы завершили получение всех изменений для этого раунда.</span><span class="sxs-lookup"><span data-stu-id="1bed0-224">Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="1bed0-225">В ответе ниже показан _skipToken_ в _\@ загоне ответа odata.nextLink._</span><span class="sxs-lookup"><span data-stu-id="1bed0-225">The response below shows a _skipToken_ in an _\@odata.nextLink_ response header.</span></span>

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


### <a name="example-2-delta-function-on-calendarview"></a><span data-ttu-id="1bed0-226">Пример 2. Функция Delta в calendarView</span><span class="sxs-lookup"><span data-stu-id="1bed0-226">Example 2: Delta function on calendarView</span></span>
#### <a name="request"></a><span data-ttu-id="1bed0-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bed0-227">Request</span></span>

<span data-ttu-id="1bed0-228">В следующем примере показан начальный запрос на синхронизацию для получения событий в заданном календаре подписанного пользователя в диапазоне дат, указанных **в calendarView.**</span><span class="sxs-lookup"><span data-stu-id="1bed0-228">The following example shows the initial sync request to get events in the specified calendar of the signed-in user, within the range of dates indicated by the **calendarView**.</span></span> <span data-ttu-id="1bed0-229">Начальный запрос не включает какой-либо маркер состояния.</span><span class="sxs-lookup"><span data-stu-id="1bed0-229">The initial request does not include any state token.</span></span> 

<span data-ttu-id="1bed0-230">Запрос использует `Prefer: odata.maxpagesize` заглавную для ограничения максимального количества событий в каждом ответе до 2.</span><span class="sxs-lookup"><span data-stu-id="1bed0-230">The request uses the `Prefer: odata.maxpagesize` header to limit the maximum number of events in each response to 2.</span></span> <span data-ttu-id="1bed0-231">Продолжайте вызывать функцию с помощью возвращенного запроса, пока не получите все события в этом представлении календаря `delta` `@odata.nextLink` и `@odata.deltaLink` ответ.</span><span class="sxs-lookup"><span data-stu-id="1bed0-231">Continue calling the `delta` function by using the query returned in `@odata.nextLink` until you get all the events in that calendar view, and a `@odata.deltaLink` in the response.</span></span>

# <a name="http"></a>[<span data-ttu-id="1bed0-232">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bed0-232">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADI5M1BbeAAA="],
  "name": "event_delta_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendars/AAMkADI5M1BbeAAA=/calendarview/delta?startDateTime=2020-06-01T00:00:00Z&endDateTime=2020-06-10T00:00:00Z

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="1bed0-233">C#</span><span class="sxs-lookup"><span data-stu-id="1bed0-233">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-delta-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1bed0-234">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1bed0-234">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-delta-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1bed0-235">Java</span><span class="sxs-lookup"><span data-stu-id="1bed0-235">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-delta-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1bed0-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bed0-236">Response</span></span>

<span data-ttu-id="1bed0-237">Если запрос является успешным, в ответ включается маркер состояния, который является либо _skipToken_ (в загоне ответа _\@ odata.nextLink)_ или _deltaToken_ (в загоне ответа _\@ odata.deltaLink)._</span><span class="sxs-lookup"><span data-stu-id="1bed0-237">If the request is successful, the response includes a state token, which is either a _skipToken_ (in an _\@odata.nextLink_ response header) or a _deltaToken_ (in an _\@odata.deltaLink_ response header).</span></span>
<span data-ttu-id="1bed0-238">Соответственно, они указывают, следует ли продолжить раунд или вы завершили получение всех изменений для этого раунда.</span><span class="sxs-lookup"><span data-stu-id="1bed0-238">Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="1bed0-239">В ответе ниже показан _skipToken_ в _\@ загоне ответа odata.nextLink._</span><span class="sxs-lookup"><span data-stu-id="1bed0-239">The response below shows a _skipToken_ in an _\@odata.nextLink_ response header.</span></span>

<span data-ttu-id="1bed0-240">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="1bed0-240">Note: The response object shown here may be truncated for brevity.</span></span> 
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

## <a name="see-also"></a><span data-ttu-id="1bed0-241">См. также</span><span class="sxs-lookup"><span data-stu-id="1bed0-241">See also</span></span>

- [<span data-ttu-id="1bed0-242">Запрос изменений Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1bed0-242">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="1bed0-243">Получение добавочных изменений для событий в папке</span><span class="sxs-lookup"><span data-stu-id="1bed0-243">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)

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


