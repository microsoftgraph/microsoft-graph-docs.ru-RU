---
title: Обновление события
description: Обновление свойств объекта event.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5532a950a44b2524501d387c249c88e5d4f4efd4
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719673"
---
# <a name="update-event"></a><span data-ttu-id="fc5bd-103">Обновление события</span><span class="sxs-lookup"><span data-stu-id="fc5bd-103">Update event</span></span>

<span data-ttu-id="fc5bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc5bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc5bd-105">Обновление свойств объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="fc5bd-105">Update the properties of the [event](../resources/event.md) object.</span></span>

<span data-ttu-id="fc5bd-106">При обновлении часового пояса начала или завершения события сначала [найдите поддерживаемые часовые пояса](outlookuser-supportedtimezones.md), чтобы устанавливать только часовые пояса, настроенные для сервера почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-106">When updating the time zone of the start or end time of an event, first [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

## <a name="permissions"></a><span data-ttu-id="fc5bd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc5bd-107">Permissions</span></span>
<span data-ttu-id="fc5bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc5bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc5bd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc5bd-110">Permission type</span></span>      | <span data-ttu-id="fc5bd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc5bd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc5bd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc5bd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fc5bd-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc5bd-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fc5bd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc5bd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc5bd-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc5bd-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fc5bd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc5bd-116">Application</span></span> | <span data-ttu-id="fc5bd-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc5bd-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc5bd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc5bd-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="fc5bd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc5bd-119">Request headers</span></span>
| <span data-ttu-id="fc5bd-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fc5bd-120">Name</span></span>       | <span data-ttu-id="fc5bd-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fc5bd-121">Type</span></span> | <span data-ttu-id="fc5bd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fc5bd-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fc5bd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc5bd-123">Authorization</span></span>  | <span data-ttu-id="fc5bd-124">string</span><span class="sxs-lookup"><span data-stu-id="fc5bd-124">string</span></span>  | <span data-ttu-id="fc5bd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc5bd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc5bd-127">Request body</span></span>
<span data-ttu-id="fc5bd-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fc5bd-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc5bd-131">Property</span></span>       | <span data-ttu-id="fc5bd-132">Тип</span><span class="sxs-lookup"><span data-stu-id="fc5bd-132">Type</span></span>    | <span data-ttu-id="fc5bd-133">Описание</span><span class="sxs-lookup"><span data-stu-id="fc5bd-133">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="fc5bd-134">attendees</span><span class="sxs-lookup"><span data-stu-id="fc5bd-134">attendees</span></span>|<span data-ttu-id="fc5bd-135">Attendee</span><span class="sxs-lookup"><span data-stu-id="fc5bd-135">Attendee</span></span>|<span data-ttu-id="fc5bd-136">Коллекция участников события.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-136">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="fc5bd-137">body</span><span class="sxs-lookup"><span data-stu-id="fc5bd-137">body</span></span>|<span data-ttu-id="fc5bd-138">ItemBody</span><span class="sxs-lookup"><span data-stu-id="fc5bd-138">ItemBody</span></span>|<span data-ttu-id="fc5bd-139">Текст сообщения, связанного с событием.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-139">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="fc5bd-140">categories</span><span class="sxs-lookup"><span data-stu-id="fc5bd-140">categories</span></span>|<span data-ttu-id="fc5bd-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc5bd-141">String collection</span></span>|<span data-ttu-id="fc5bd-142">Категории, связанные с событием.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-142">The categories associated with the event.</span></span>|
| <span data-ttu-id="fc5bd-143">end</span><span class="sxs-lookup"><span data-stu-id="fc5bd-143">end</span></span>|<span data-ttu-id="fc5bd-144">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="fc5bd-144">DateTimeTimeZone</span></span>|<span data-ttu-id="fc5bd-145">Дата, время и часовой пояс завершения события.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-145">The date, time, and time zone that the event ends.</span></span> |
|<span data-ttu-id="fc5bd-146">hideAttendees</span><span class="sxs-lookup"><span data-stu-id="fc5bd-146">hideAttendees</span></span>|<span data-ttu-id="fc5bd-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc5bd-147">Boolean</span></span>|<span data-ttu-id="fc5bd-148">Если за установлено, каждый участник видит себя только в запросе на собрание `true` и в списке **отслеживания** собраний.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-148">When set to `true`, each attendee only sees themselves in the meeting request and meeting **Tracking** list.</span></span> <span data-ttu-id="fc5bd-149">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-149">Default is false.</span></span>|
| <span data-ttu-id="fc5bd-150">importance</span><span class="sxs-lookup"><span data-stu-id="fc5bd-150">importance</span></span>|<span data-ttu-id="fc5bd-151">String</span><span class="sxs-lookup"><span data-stu-id="fc5bd-151">String</span></span>|<span data-ttu-id="fc5bd-152">Важность события.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-152">The importance of the event.</span></span> <span data-ttu-id="fc5bd-153">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-153">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="fc5bd-154">isAllDay</span><span class="sxs-lookup"><span data-stu-id="fc5bd-154">isAllDay</span></span>|<span data-ttu-id="fc5bd-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc5bd-155">Boolean</span></span>|<span data-ttu-id="fc5bd-156">Задайте значение true, если событие длится весь день.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-156">Set to true if the event lasts all day.</span></span> <span data-ttu-id="fc5bd-157">Если значение равно true, то независимо от того, один или несколько дней длится событие, время его начала и окончания должно быть установлено на полночь в одном и том же часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-157">If true, regardless of whether it's a single-day or multi-day event, start and end time must be set to midnight and be in the same time zone.</span></span>|
|<span data-ttu-id="fc5bd-158">isOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="fc5bd-158">isOnlineMeeting</span></span>|<span data-ttu-id="fc5bd-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc5bd-159">Boolean</span></span>| <span data-ttu-id="fc5bd-160">`True`, если это событие содержит информацию о собраниях по сети; в противном случае — `false`.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-160">`True` if this event has online meeting information, `false` otherwise.</span></span> <span data-ttu-id="fc5bd-161">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-161">Default is false.</span></span> <span data-ttu-id="fc5bd-162">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-162">Optional.</span></span>|
| <span data-ttu-id="fc5bd-163">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="fc5bd-163">isReminderOn</span></span>|<span data-ttu-id="fc5bd-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc5bd-164">Boolean</span></span>|<span data-ttu-id="fc5bd-165">Задайте значение true, если установлено напоминание пользователю о событии.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-165">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="fc5bd-166">location</span><span class="sxs-lookup"><span data-stu-id="fc5bd-166">location</span></span>|<span data-ttu-id="fc5bd-167">Расположение</span><span class="sxs-lookup"><span data-stu-id="fc5bd-167">Location</span></span>|<span data-ttu-id="fc5bd-168">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-168">The location of the event.</span></span>|
|<span data-ttu-id="fc5bd-169">locations</span><span class="sxs-lookup"><span data-stu-id="fc5bd-169">locations</span></span>|<span data-ttu-id="fc5bd-170">Коллекция [Location](../resources/location.md)</span><span class="sxs-lookup"><span data-stu-id="fc5bd-170">[Location](../resources/location.md) collection</span></span>|<span data-ttu-id="fc5bd-171">Места проведения события или участия в нем.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-171">The locations where the event is held or attended from.</span></span> <span data-ttu-id="fc5bd-172">Свойства **location** и **locations** всегда совпадают друг с другом.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-172">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="fc5bd-173">Если вы обновите свойство **location**, предыдущие места в коллекции **locations** будут удалены и заменены новым значением **location**.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-173">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="fc5bd-174">onlineMeetingProvider</span><span class="sxs-lookup"><span data-stu-id="fc5bd-174">onlineMeetingProvider</span></span>|<span data-ttu-id="fc5bd-175">onlineMeetingProviderType</span><span class="sxs-lookup"><span data-stu-id="fc5bd-175">onlineMeetingProviderType</span></span>| <span data-ttu-id="fc5bd-176">Представляет поставщика службы собраний по сети.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-176">Represents the online meeting service provider.</span></span> <span data-ttu-id="fc5bd-177">Возможные значения: `teamsForBusiness`, `skypeForBusiness` и `skypeForConsumer`.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-177">The possible values are `teamsForBusiness`, `skypeForBusiness`, and `skypeForConsumer`.</span></span> <span data-ttu-id="fc5bd-178">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-178">Optional.</span></span> |
| <span data-ttu-id="fc5bd-179">recurrence</span><span class="sxs-lookup"><span data-stu-id="fc5bd-179">recurrence</span></span>|<span data-ttu-id="fc5bd-180">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="fc5bd-180">PatternedRecurrence</span></span>|<span data-ttu-id="fc5bd-181">Расписание повторения события.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-181">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="fc5bd-182">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="fc5bd-182">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="fc5bd-183">Int32</span><span class="sxs-lookup"><span data-stu-id="fc5bd-183">Int32</span></span>|<span data-ttu-id="fc5bd-184">Позволяет указать, за сколько минут до начала события появляется напоминание.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-184">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="fc5bd-185">responseRequested</span><span class="sxs-lookup"><span data-stu-id="fc5bd-185">responseRequested</span></span>|<span data-ttu-id="fc5bd-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc5bd-186">Boolean</span></span>|<span data-ttu-id="fc5bd-187">Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-187">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="fc5bd-188">sensitivity</span><span class="sxs-lookup"><span data-stu-id="fc5bd-188">sensitivity</span></span>|<span data-ttu-id="fc5bd-189">String</span><span class="sxs-lookup"><span data-stu-id="fc5bd-189">String</span></span>| <span data-ttu-id="fc5bd-190">Возможные значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-190">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="fc5bd-191">showAs</span><span class="sxs-lookup"><span data-stu-id="fc5bd-191">showAs</span></span>|<span data-ttu-id="fc5bd-192">String</span><span class="sxs-lookup"><span data-stu-id="fc5bd-192">String</span></span>|<span data-ttu-id="fc5bd-193">Отображаемое состояние.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-193">The status to show.</span></span> <span data-ttu-id="fc5bd-194">Возможные значения: `free` , , , , `tentative` `busy` `oof` `workingElsewhere` `unknown` .</span><span class="sxs-lookup"><span data-stu-id="fc5bd-194">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="fc5bd-195">начать</span><span class="sxs-lookup"><span data-stu-id="fc5bd-195">start</span></span>|<span data-ttu-id="fc5bd-196">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="fc5bd-196">DateTimeTimeZone</span></span>|<span data-ttu-id="fc5bd-197">Дата, время и часовой пояс начала события.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-197">The start date, time, and time zone of the event.</span></span> |
| <span data-ttu-id="fc5bd-198">subject</span><span class="sxs-lookup"><span data-stu-id="fc5bd-198">subject</span></span>|<span data-ttu-id="fc5bd-199">String</span><span class="sxs-lookup"><span data-stu-id="fc5bd-199">String</span></span>|<span data-ttu-id="fc5bd-200">Текст в строке темы сообщения о событии.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-200">The text of the event's subject line.</span></span>|

<span data-ttu-id="fc5bd-201">Так как ресурс **event** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **event**.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-201">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="fc5bd-202">Если обновляемый ресурс **event** является главным событием повторяющегося ряда, содержит несколько участников и экземпляры, обновленные отдельно, отправляется несколько сообщений электронной почты с уведомлениями: одно для главного ряда и по одному для каждого обновленного экземпляра.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-202">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="fc5bd-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc5bd-203">Response</span></span>

<span data-ttu-id="fc5bd-204">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-204">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="fc5bd-205">**Примечание.** Этот метод может вернуть отклик "HTTP 400 — ошибочный запрос" с кодом ошибки `ErrorOccurrenceCrossingBoundary` и следующим сообщением об ошибке: "Измененная копия пересекается со смежной копией или перекрывает ее".</span><span class="sxs-lookup"><span data-stu-id="fc5bd-205">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="fc5bd-206">Это означает, что обновление нарушает следующее ограничение Outlook для повторяющихся исключений: повторение нельзя перемещать на день предыдущего повторения или до него, а также на день следующего повторения или после него.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-206">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="fc5bd-207">Пример</span><span class="sxs-lookup"><span data-stu-id="fc5bd-207">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fc5bd-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc5bd-208">Request</span></span>

<span data-ttu-id="fc5bd-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-209">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fc5bd-210">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc5bd-210">HTTP</span></span>](#tab/http)
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
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness",
  "isReminderOn": true,
  "hideAttendees": false,
  "categories": ["Red category"]
}
```
# <a name="c"></a>[<span data-ttu-id="fc5bd-211">C#</span><span class="sxs-lookup"><span data-stu-id="fc5bd-211">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc5bd-212">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc5bd-212">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc5bd-213">Java</span><span class="sxs-lookup"><span data-stu-id="fc5bd-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fc5bd-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc5bd-214">Response</span></span>

<span data-ttu-id="fc5bd-215">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-215">Here is an example of the response.</span></span> <span data-ttu-id="fc5bd-216">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="fc5bd-216">Note: The response object shown here may be truncated for brevity.</span></span>

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
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness",
  "isReminderOn": true,
  "hideAttendees": false,
  "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NzIyNzhlMGEtM2YyZC00ZmY0LTlhNzUtZmZjNWFmZGNlNzE2%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22bc55b173-cff6-457d-b7a1-64bda7d7581a%22%7d",
        "conferenceId": "177513992",
        "tollNumber": "+91 22 6241 6885"
    }
}
```


## <a name="see-also"></a><span data-ttu-id="fc5bd-217">См. также</span><span class="sxs-lookup"><span data-stu-id="fc5bd-217">See also</span></span>

- [<span data-ttu-id="fc5bd-218">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="fc5bd-218">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fc5bd-219">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="fc5bd-219">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="fc5bd-220">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="fc5bd-220">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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


