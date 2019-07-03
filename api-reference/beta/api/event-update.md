---
title: Обновление события
description: Обновление свойств объекта event.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 911f15257ce10e628cb63db2ca4ee9517b5cbe81
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440941"
---
# <a name="update-event"></a><span data-ttu-id="5105c-103">Обновление события</span><span class="sxs-lookup"><span data-stu-id="5105c-103">Update event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5105c-104">Обновление свойств объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="5105c-104">Update the properties of the [event](../resources/event.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5105c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5105c-105">Permissions</span></span>
<span data-ttu-id="5105c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5105c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5105c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5105c-108">Permission type</span></span>      | <span data-ttu-id="5105c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5105c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5105c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5105c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5105c-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5105c-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5105c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5105c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5105c-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5105c-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5105c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5105c-114">Application</span></span> | <span data-ttu-id="5105c-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5105c-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5105c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5105c-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="5105c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5105c-117">Request headers</span></span>
| <span data-ttu-id="5105c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5105c-118">Name</span></span>       | <span data-ttu-id="5105c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5105c-119">Type</span></span> | <span data-ttu-id="5105c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5105c-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5105c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5105c-121">Authorization</span></span>  | <span data-ttu-id="5105c-122">string</span><span class="sxs-lookup"><span data-stu-id="5105c-122">string</span></span>  | <span data-ttu-id="5105c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5105c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5105c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5105c-125">Request body</span></span>
<span data-ttu-id="5105c-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5105c-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5105c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5105c-129">Property</span></span>       | <span data-ttu-id="5105c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5105c-130">Type</span></span>    | <span data-ttu-id="5105c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5105c-131">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="5105c-132">attendees</span><span class="sxs-lookup"><span data-stu-id="5105c-132">attendees</span></span>|<span data-ttu-id="5105c-133">Attendee</span><span class="sxs-lookup"><span data-stu-id="5105c-133">Attendee</span></span>|<span data-ttu-id="5105c-134">Коллекция участников события.</span><span class="sxs-lookup"><span data-stu-id="5105c-134">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="5105c-135">body</span><span class="sxs-lookup"><span data-stu-id="5105c-135">body</span></span>|<span data-ttu-id="5105c-136">ItemBody</span><span class="sxs-lookup"><span data-stu-id="5105c-136">ItemBody</span></span>|<span data-ttu-id="5105c-137">Текст сообщения, связанного с событием.</span><span class="sxs-lookup"><span data-stu-id="5105c-137">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="5105c-138">categories</span><span class="sxs-lookup"><span data-stu-id="5105c-138">categories</span></span>|<span data-ttu-id="5105c-139">String</span><span class="sxs-lookup"><span data-stu-id="5105c-139">String</span></span>|<span data-ttu-id="5105c-140">Категории, связанные с событием.</span><span class="sxs-lookup"><span data-stu-id="5105c-140">The categories associated with the event.</span></span>|
| <span data-ttu-id="5105c-141">end</span><span class="sxs-lookup"><span data-stu-id="5105c-141">end</span></span>|<span data-ttu-id="5105c-142">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5105c-142">DateTimeTimeZone</span></span>|<span data-ttu-id="5105c-143">Дата и время завершения события.</span><span class="sxs-lookup"><span data-stu-id="5105c-143">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="5105c-p104">По умолчанию время завершения указано в формате UTC. Можно дополнительно указать часовой пояс в элементе EndTimeZone, задать время завершения согласно этому часовому поясу и UTC-смещение. Обратите внимание, что если вы используете EndTimeZone, следует также указать значение StartTimeZone.</span><span class="sxs-lookup"><span data-stu-id="5105c-p104">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="5105c-147">Пример указания даты (25 февраля 2015 г., 21:34 по тихоокеанскому поясному времени): "2015-02-25T21:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="5105c-147">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
| <span data-ttu-id="5105c-148">importance</span><span class="sxs-lookup"><span data-stu-id="5105c-148">importance</span></span>|<span data-ttu-id="5105c-149">String</span><span class="sxs-lookup"><span data-stu-id="5105c-149">String</span></span>|<span data-ttu-id="5105c-150">Важность события.</span><span class="sxs-lookup"><span data-stu-id="5105c-150">The importance of the event.</span></span> <span data-ttu-id="5105c-151">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="5105c-151">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="5105c-152">isAllDay</span><span class="sxs-lookup"><span data-stu-id="5105c-152">isAllDay</span></span>|<span data-ttu-id="5105c-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="5105c-153">Boolean</span></span>|<span data-ttu-id="5105c-154">Задайте значение true, если событие длится весь день.</span><span class="sxs-lookup"><span data-stu-id="5105c-154">Set to true if the event lasts all day.</span></span>|
| <span data-ttu-id="5105c-155">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="5105c-155">isReminderOn</span></span>|<span data-ttu-id="5105c-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="5105c-156">Boolean</span></span>|<span data-ttu-id="5105c-157">Задайте значение true, если установлено напоминание пользователю о событии.</span><span class="sxs-lookup"><span data-stu-id="5105c-157">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="5105c-158">location</span><span class="sxs-lookup"><span data-stu-id="5105c-158">location</span></span>|<span data-ttu-id="5105c-159">Расположение</span><span class="sxs-lookup"><span data-stu-id="5105c-159">Location</span></span>|<span data-ttu-id="5105c-160">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="5105c-160">The location of the event.</span></span>|
|<span data-ttu-id="5105c-161">locations</span><span class="sxs-lookup"><span data-stu-id="5105c-161">locations</span></span>|<span data-ttu-id="5105c-162">Коллекция [Location](../resources/location.md)</span><span class="sxs-lookup"><span data-stu-id="5105c-162">[Location](../resources/location.md) collection</span></span>|<span data-ttu-id="5105c-163">Места проведения мероприятия или участия в нем.</span><span class="sxs-lookup"><span data-stu-id="5105c-163">The locations where the event is held or attended from.</span></span> <span data-ttu-id="5105c-164">Свойства **location** и **locations** всегда совпадают друг с другом.</span><span class="sxs-lookup"><span data-stu-id="5105c-164">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="5105c-165">Если вы обновите свойство **location**, предыдущие места в коллекции **locations** будут удалены и заменены новым значением **location**.</span><span class="sxs-lookup"><span data-stu-id="5105c-165">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
| <span data-ttu-id="5105c-166">recurrence</span><span class="sxs-lookup"><span data-stu-id="5105c-166">recurrence</span></span>|<span data-ttu-id="5105c-167">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="5105c-167">PatternedRecurrence</span></span>|<span data-ttu-id="5105c-168">Расписание повторения события.</span><span class="sxs-lookup"><span data-stu-id="5105c-168">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="5105c-169">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="5105c-169">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="5105c-170">Int32</span><span class="sxs-lookup"><span data-stu-id="5105c-170">Int32</span></span>|<span data-ttu-id="5105c-171">Позволяет указать, за сколько минут до начала события появляется напоминание.</span><span class="sxs-lookup"><span data-stu-id="5105c-171">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="5105c-172">responseRequested</span><span class="sxs-lookup"><span data-stu-id="5105c-172">responseRequested</span></span>|<span data-ttu-id="5105c-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="5105c-173">Boolean</span></span>|<span data-ttu-id="5105c-174">Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения.</span><span class="sxs-lookup"><span data-stu-id="5105c-174">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="5105c-175">sensitivity</span><span class="sxs-lookup"><span data-stu-id="5105c-175">sensitivity</span></span>|<span data-ttu-id="5105c-176">String</span><span class="sxs-lookup"><span data-stu-id="5105c-176">String</span></span>| <span data-ttu-id="5105c-177">Возможные значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="5105c-177">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="5105c-178">showAs</span><span class="sxs-lookup"><span data-stu-id="5105c-178">showAs</span></span>|<span data-ttu-id="5105c-179">String</span><span class="sxs-lookup"><span data-stu-id="5105c-179">String</span></span>|<span data-ttu-id="5105c-180">Отображаемое состояние.</span><span class="sxs-lookup"><span data-stu-id="5105c-180">The status to show.</span></span> <span data-ttu-id="5105c-181">Возможные `free` значения:, `tentative`, `busy`, `oof`, `workingElsewhere`,. `unknown`</span><span class="sxs-lookup"><span data-stu-id="5105c-181">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="5105c-182">начать</span><span class="sxs-lookup"><span data-stu-id="5105c-182">start</span></span>|<span data-ttu-id="5105c-183">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5105c-183">DateTimeTimeZone</span></span>|<span data-ttu-id="5105c-184">Время начала события.</span><span class="sxs-lookup"><span data-stu-id="5105c-184">The start time of the event.</span></span> <br/><br/><span data-ttu-id="5105c-p108">По умолчанию время начала указано в формате UTC. Можно дополнительно указать часовой пояс в элементе StartTimeZone, задать время завершения согласно этому часовому поясу и UTC-смещение. Обратите внимание, что если вы используете StartTimeZone, следует также указать значение EndTimeZone.</span><span class="sxs-lookup"><span data-stu-id="5105c-p108">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="5105c-188">Пример указания даты (25 февраля 2015 г., 19:34 по тихоокеанскому поясному времени): "2015-02-25T19:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="5105c-188">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
| <span data-ttu-id="5105c-189">subject</span><span class="sxs-lookup"><span data-stu-id="5105c-189">subject</span></span>|<span data-ttu-id="5105c-190">String</span><span class="sxs-lookup"><span data-stu-id="5105c-190">String</span></span>|<span data-ttu-id="5105c-191">Текст в строке темы сообщения о событии.</span><span class="sxs-lookup"><span data-stu-id="5105c-191">The text of the event's subject line.</span></span>|

<span data-ttu-id="5105c-192">Так как ресурс **event** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **event**.</span><span class="sxs-lookup"><span data-stu-id="5105c-192">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="5105c-193">Если обновляемый ресурс **event** является главным событием повторяющегося ряда, содержит несколько участников и экземпляры, обновленные отдельно, отправляется несколько сообщений электронной почты с уведомлениями: одно для главного ряда и по одному для каждого обновленного экземпляра.</span><span class="sxs-lookup"><span data-stu-id="5105c-193">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="5105c-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="5105c-194">Response</span></span>

<span data-ttu-id="5105c-195">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5105c-195">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="5105c-196">**Примечание.** Этот метод может вернуть отклик "HTTP 400 — ошибочный запрос" с кодом ошибки `ErrorOccurrenceCrossingBoundary` и следующим сообщением об ошибке: "Измененная копия пересекается со смежной копией или перекрывает ее".</span><span class="sxs-lookup"><span data-stu-id="5105c-196">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="5105c-197">Это означает, что обновление нарушает следующее ограничение Outlook для повторяющихся исключений: повторение нельзя перемещать на день предыдущего повторения или до него, а также на день следующего повторения или после него.</span><span class="sxs-lookup"><span data-stu-id="5105c-197">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="5105c-198">Пример</span><span class="sxs-lookup"><span data-stu-id="5105c-198">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5105c-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="5105c-199">Request</span></span>

<span data-ttu-id="5105c-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5105c-200">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5105c-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="5105c-201">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5105c-202">C#</span><span class="sxs-lookup"><span data-stu-id="5105c-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5105c-203">Javascript</span><span class="sxs-lookup"><span data-stu-id="5105c-203">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5105c-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="5105c-204">Response</span></span>
<span data-ttu-id="5105c-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5105c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```


## <a name="see-also"></a><span data-ttu-id="5105c-208">Дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="5105c-208">See also</span></span>

- [<span data-ttu-id="5105c-209">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="5105c-209">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5105c-210">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5105c-210">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="5105c-211">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5105c-211">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
