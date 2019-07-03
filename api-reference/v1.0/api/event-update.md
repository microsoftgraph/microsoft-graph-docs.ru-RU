---
title: Обновление события
description: Обновление свойств объекта event.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: b8d767f406d9d635a3a76ba03120851917b91689
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444381"
---
# <a name="update-event"></a><span data-ttu-id="ad041-103">Обновление события</span><span class="sxs-lookup"><span data-stu-id="ad041-103">Update event</span></span>

<span data-ttu-id="ad041-104">Обновление свойств объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="ad041-104">Update the properties of the [event](../resources/event.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ad041-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad041-105">Permissions</span></span>
<span data-ttu-id="ad041-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad041-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad041-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad041-108">Permission type</span></span>      | <span data-ttu-id="ad041-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad041-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad041-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad041-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ad041-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad041-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ad041-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad041-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad041-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad041-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ad041-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad041-114">Application</span></span> | <span data-ttu-id="ad041-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad041-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad041-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad041-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/events/{id}
PATCH /users/{id | userPrincipalName}/events/{id}
PATCH /groups/{id}/events/{id}

PATCH /me/calendar/events/{id}
PATCH /users/{id | userPrincipalName}/calendar/events/{id}
PATCH /groups/{id}/calendar/events/{id}

PATCH /me/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}/events/{id}

PATCH /me/calendargroup/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

PATCH /me/calendargroups/{id}/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ad041-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad041-117">Request headers</span></span>
| <span data-ttu-id="ad041-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ad041-118">Name</span></span>       | <span data-ttu-id="ad041-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ad041-119">Type</span></span> | <span data-ttu-id="ad041-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ad041-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ad041-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad041-121">Authorization</span></span>  | <span data-ttu-id="ad041-122">string</span><span class="sxs-lookup"><span data-stu-id="ad041-122">string</span></span>  | <span data-ttu-id="ad041-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad041-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad041-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad041-125">Request body</span></span>
<span data-ttu-id="ad041-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ad041-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ad041-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad041-129">Property</span></span>     | <span data-ttu-id="ad041-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ad041-130">Type</span></span>   |<span data-ttu-id="ad041-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ad041-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad041-132">attendees</span><span class="sxs-lookup"><span data-stu-id="ad041-132">attendees</span></span>|[<span data-ttu-id="ad041-133">Attendee</span><span class="sxs-lookup"><span data-stu-id="ad041-133">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="ad041-134">Коллекция участников события.</span><span class="sxs-lookup"><span data-stu-id="ad041-134">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="ad041-135">body</span><span class="sxs-lookup"><span data-stu-id="ad041-135">body</span></span>|[<span data-ttu-id="ad041-136">ItemBody</span><span class="sxs-lookup"><span data-stu-id="ad041-136">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="ad041-137">Текст сообщения, связанного с событием.</span><span class="sxs-lookup"><span data-stu-id="ad041-137">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="ad041-138">categories</span><span class="sxs-lookup"><span data-stu-id="ad041-138">categories</span></span>|<span data-ttu-id="ad041-139">String</span><span class="sxs-lookup"><span data-stu-id="ad041-139">String</span></span>|<span data-ttu-id="ad041-140">Категории, связанные с событием.</span><span class="sxs-lookup"><span data-stu-id="ad041-140">The categories associated with the event.</span></span>|
|<span data-ttu-id="ad041-141">end</span><span class="sxs-lookup"><span data-stu-id="ad041-141">end</span></span>|[<span data-ttu-id="ad041-142">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ad041-142">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="ad041-143">Дата и время завершения события.</span><span class="sxs-lookup"><span data-stu-id="ad041-143">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="ad041-p104">По умолчанию время завершения указано в формате UTC. Можно дополнительно указать часовой пояс в элементе EndTimeZone, задать время завершения согласно этому часовому поясу и UTC-смещение. Обратите внимание, что если вы используете EndTimeZone, следует также указать значение StartTimeZone.</span><span class="sxs-lookup"><span data-stu-id="ad041-p104">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="ad041-147">Пример указания даты (25 февраля 2015 г., 21:34 по тихоокеанскому поясному времени): "2015-02-25T21:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="ad041-147">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
|<span data-ttu-id="ad041-148">importance</span><span class="sxs-lookup"><span data-stu-id="ad041-148">importance</span></span>|<span data-ttu-id="ad041-149">String</span><span class="sxs-lookup"><span data-stu-id="ad041-149">String</span></span>|<span data-ttu-id="ad041-150">Важность события.</span><span class="sxs-lookup"><span data-stu-id="ad041-150">The importance of the event.</span></span> <span data-ttu-id="ad041-151">Допустимые значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="ad041-151">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="ad041-152">isAllDay</span><span class="sxs-lookup"><span data-stu-id="ad041-152">isAllDay</span></span>|<span data-ttu-id="ad041-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad041-153">Boolean</span></span>|<span data-ttu-id="ad041-154">Задайте значение true, если событие длится весь день.</span><span class="sxs-lookup"><span data-stu-id="ad041-154">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="ad041-155">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="ad041-155">isReminderOn</span></span>|<span data-ttu-id="ad041-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad041-156">Boolean</span></span>|<span data-ttu-id="ad041-157">Задайте значение true, если установлено напоминание пользователю о событии.</span><span class="sxs-lookup"><span data-stu-id="ad041-157">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="ad041-158">location</span><span class="sxs-lookup"><span data-stu-id="ad041-158">location</span></span>|[<span data-ttu-id="ad041-159">Location</span><span class="sxs-lookup"><span data-stu-id="ad041-159">Location</span></span>](../resources/location.md)|<span data-ttu-id="ad041-160">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="ad041-160">The location of the event.</span></span>|
|<span data-ttu-id="ad041-161">locations</span><span class="sxs-lookup"><span data-stu-id="ad041-161">locations</span></span>|<span data-ttu-id="ad041-162">Коллекция [location](../resources/location.md)</span><span class="sxs-lookup"><span data-stu-id="ad041-162">[location](../resources/location.md) collection</span></span>|<span data-ttu-id="ad041-163">Места проведения мероприятия или участия в нем.</span><span class="sxs-lookup"><span data-stu-id="ad041-163">The locations where the event is held or attended from.</span></span> <span data-ttu-id="ad041-164">Свойства **location** и **locations** всегда совпадают друг с другом.</span><span class="sxs-lookup"><span data-stu-id="ad041-164">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="ad041-165">Если вы обновите свойство **location**, предыдущие места в коллекции **locations** будут удалены и заменены новым значением **location**.</span><span class="sxs-lookup"><span data-stu-id="ad041-165">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="ad041-166">recurrence</span><span class="sxs-lookup"><span data-stu-id="ad041-166">recurrence</span></span>|[<span data-ttu-id="ad041-167">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="ad041-167">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="ad041-168">Расписание повторения события.</span><span class="sxs-lookup"><span data-stu-id="ad041-168">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="ad041-169">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="ad041-169">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="ad041-170">Int32</span><span class="sxs-lookup"><span data-stu-id="ad041-170">Int32</span></span>|<span data-ttu-id="ad041-171">Позволяет указать, за сколько минут до начала события появляется напоминание.</span><span class="sxs-lookup"><span data-stu-id="ad041-171">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="ad041-172">responseRequested</span><span class="sxs-lookup"><span data-stu-id="ad041-172">responseRequested</span></span>|<span data-ttu-id="ad041-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad041-173">Boolean</span></span>|<span data-ttu-id="ad041-174">Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения.</span><span class="sxs-lookup"><span data-stu-id="ad041-174">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="ad041-175">sensitivity</span><span class="sxs-lookup"><span data-stu-id="ad041-175">sensitivity</span></span>|<span data-ttu-id="ad041-176">String</span><span class="sxs-lookup"><span data-stu-id="ad041-176">String</span></span>| <span data-ttu-id="ad041-177">Допустимые значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="ad041-177">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="ad041-178">showAs</span><span class="sxs-lookup"><span data-stu-id="ad041-178">showAs</span></span>|<span data-ttu-id="ad041-179">String</span><span class="sxs-lookup"><span data-stu-id="ad041-179">String</span></span>|<span data-ttu-id="ad041-180">Отображаемое состояние.</span><span class="sxs-lookup"><span data-stu-id="ad041-180">The status to show.</span></span> <span data-ttu-id="ad041-181">Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ad041-181">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="ad041-182">начать</span><span class="sxs-lookup"><span data-stu-id="ad041-182">start</span></span>|[<span data-ttu-id="ad041-183">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ad041-183">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="ad041-184">Время начала события.</span><span class="sxs-lookup"><span data-stu-id="ad041-184">The start time of the event.</span></span> <br/><br/><span data-ttu-id="ad041-p108">По умолчанию время начала указано в формате UTC. Можно дополнительно указать часовой пояс в элементе StartTimeZone, задать время завершения согласно этому часовому поясу и UTC-смещение. Обратите внимание, что если вы используете StartTimeZone, следует также указать значение EndTimeZone.</span><span class="sxs-lookup"><span data-stu-id="ad041-p108">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="ad041-188">Пример указания даты (25 февраля 2015 г., 19:34 по тихоокеанскому поясному времени): "2015-02-25T19:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="ad041-188">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
|<span data-ttu-id="ad041-189">subject</span><span class="sxs-lookup"><span data-stu-id="ad041-189">subject</span></span>|<span data-ttu-id="ad041-190">String</span><span class="sxs-lookup"><span data-stu-id="ad041-190">String</span></span>|<span data-ttu-id="ad041-191">Текст в строке темы сообщения о событии.</span><span class="sxs-lookup"><span data-stu-id="ad041-191">The text of the event's subject line.</span></span>|

<span data-ttu-id="ad041-192">Так как ресурс **event** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **event**.</span><span class="sxs-lookup"><span data-stu-id="ad041-192">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>  
  
<span data-ttu-id="ad041-193">Если обновляемый ресурс **event** является главным событием повторяющегося ряда, содержит несколько участников и экземпляры, обновленные отдельно, отправляется несколько сообщений электронной почты с уведомлениями: одно для главного ряда и по одному для каждого обновленного экземпляра.</span><span class="sxs-lookup"><span data-stu-id="ad041-193">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>  

## <a name="response"></a><span data-ttu-id="ad041-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad041-194">Response</span></span>

<span data-ttu-id="ad041-195">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ad041-195">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>  

><span data-ttu-id="ad041-196">**Примечание.** Этот метод может вернуть отклик "HTTP 400 — ошибочный запрос" с кодом ошибки `ErrorOccurrenceCrossingBoundary` и следующим сообщением об ошибке: "Измененная копия пересекается со смежной копией или перекрывает ее".</span><span class="sxs-lookup"><span data-stu-id="ad041-196">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="ad041-197">Это означает, что обновление нарушает следующее ограничение Outlook для повторяющихся исключений: повторение нельзя перемещать на день предыдущего повторения или до него, а также на день следующего повторения или после него.</span><span class="sxs-lookup"><span data-stu-id="ad041-197">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="ad041-198">Пример</span><span class="sxs-lookup"><span data-stu-id="ad041-198">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ad041-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad041-199">Request</span></span>

<span data-ttu-id="ad041-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad041-200">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ad041-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad041-201">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "recurrence": null,
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ad041-202">C#</span><span class="sxs-lookup"><span data-stu-id="ad041-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad041-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad041-203">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ad041-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad041-204">Response</span></span>

<span data-ttu-id="ad041-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ad041-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "recurrence": null,  
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

## <a name="see-also"></a><span data-ttu-id="ad041-208">См. также</span><span class="sxs-lookup"><span data-stu-id="ad041-208">See also</span></span>

- [<span data-ttu-id="ad041-209">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="ad041-209">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ad041-210">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="ad041-210">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="ad041-211">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="ad041-211">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
