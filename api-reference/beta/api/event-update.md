---
title: Обновление события
description: Обновление свойств объекта event.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 847bb4f25cfdadecc3983ac7365eff8146200094
ms.sourcegitcommit: 6144934d4f6cf8c9797aa19e62285217220c7f45
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268386"
---
# <a name="update-event"></a><span data-ttu-id="7a962-103">Обновление события</span><span class="sxs-lookup"><span data-stu-id="7a962-103">Update event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a962-104">Обновление свойств объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="7a962-104">Update the properties of the [event](../resources/event.md) object.</span></span>

<span data-ttu-id="7a962-105">При обновлении часового пояса начала или завершения события сначала [найдите поддерживаемые часовые пояса](outlookuser-supportedtimezones.md), чтобы устанавливать только часовые пояса, настроенные для сервера почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="7a962-105">When updating the time zone of the start or end time of an event, first [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7a962-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7a962-106">Permissions</span></span>
<span data-ttu-id="7a962-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a962-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a962-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a962-109">Permission type</span></span>      | <span data-ttu-id="7a962-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a962-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a962-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a962-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7a962-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a962-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7a962-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a962-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a962-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a962-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7a962-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a962-115">Application</span></span> | <span data-ttu-id="7a962-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a962-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a962-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a962-117">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="7a962-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a962-118">Request headers</span></span>
| <span data-ttu-id="7a962-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7a962-119">Name</span></span>       | <span data-ttu-id="7a962-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7a962-120">Type</span></span> | <span data-ttu-id="7a962-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7a962-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7a962-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a962-122">Authorization</span></span>  | <span data-ttu-id="7a962-123">string</span><span class="sxs-lookup"><span data-stu-id="7a962-123">string</span></span>  | <span data-ttu-id="7a962-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a962-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a962-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a962-126">Request body</span></span>
<span data-ttu-id="7a962-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7a962-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7a962-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a962-130">Property</span></span>       | <span data-ttu-id="7a962-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7a962-131">Type</span></span>    | <span data-ttu-id="7a962-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7a962-132">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="7a962-133">attendees</span><span class="sxs-lookup"><span data-stu-id="7a962-133">attendees</span></span>|<span data-ttu-id="7a962-134">Attendee</span><span class="sxs-lookup"><span data-stu-id="7a962-134">Attendee</span></span>|<span data-ttu-id="7a962-135">Коллекция участников события.</span><span class="sxs-lookup"><span data-stu-id="7a962-135">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="7a962-136">body</span><span class="sxs-lookup"><span data-stu-id="7a962-136">body</span></span>|<span data-ttu-id="7a962-137">ItemBody</span><span class="sxs-lookup"><span data-stu-id="7a962-137">ItemBody</span></span>|<span data-ttu-id="7a962-138">Текст сообщения, связанного с событием.</span><span class="sxs-lookup"><span data-stu-id="7a962-138">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="7a962-139">categories</span><span class="sxs-lookup"><span data-stu-id="7a962-139">categories</span></span>|<span data-ttu-id="7a962-140">String</span><span class="sxs-lookup"><span data-stu-id="7a962-140">String</span></span>|<span data-ttu-id="7a962-141">Категории, связанные с событием.</span><span class="sxs-lookup"><span data-stu-id="7a962-141">The categories associated with the event.</span></span>|
| <span data-ttu-id="7a962-142">end</span><span class="sxs-lookup"><span data-stu-id="7a962-142">end</span></span>|<span data-ttu-id="7a962-143">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="7a962-143">DateTimeTimeZone</span></span>|<span data-ttu-id="7a962-144">Дата, время и часовой пояс завершения события.</span><span class="sxs-lookup"><span data-stu-id="7a962-144">The date, time, and time zone that the event ends.</span></span> |
| <span data-ttu-id="7a962-145">importance</span><span class="sxs-lookup"><span data-stu-id="7a962-145">importance</span></span>|<span data-ttu-id="7a962-146">String</span><span class="sxs-lookup"><span data-stu-id="7a962-146">String</span></span>|<span data-ttu-id="7a962-147">Важность события.</span><span class="sxs-lookup"><span data-stu-id="7a962-147">The importance of the event.</span></span> <span data-ttu-id="7a962-148">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="7a962-148">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="7a962-149">isAllDay</span><span class="sxs-lookup"><span data-stu-id="7a962-149">isAllDay</span></span>|<span data-ttu-id="7a962-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a962-150">Boolean</span></span>|<span data-ttu-id="7a962-151">Задайте значение true, если событие длится весь день.</span><span class="sxs-lookup"><span data-stu-id="7a962-151">Set to true if the event lasts all day.</span></span> <span data-ttu-id="7a962-152">Если задано значение true, независимо от того, является ли событие одним или несколькими днями, время начала и окончания должно быть равно полночи и находиться в одном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="7a962-152">If true, regardless of whether it's a single-day or multi-day event, start and end time must be set to midnight and be in the same time zone.</span></span>|
|<span data-ttu-id="7a962-153">isOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="7a962-153">isOnlineMeeting</span></span>|<span data-ttu-id="7a962-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a962-154">Boolean</span></span>| <span data-ttu-id="7a962-155">`True`, если это событие содержит информацию о собраниях по сети; в противном случае — `false`.</span><span class="sxs-lookup"><span data-stu-id="7a962-155">`True` if this event has online meeting information, `false` otherwise.</span></span> <span data-ttu-id="7a962-156">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="7a962-156">Default is false.</span></span> <span data-ttu-id="7a962-157">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="7a962-157">Optional.</span></span>|
| <span data-ttu-id="7a962-158">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="7a962-158">isReminderOn</span></span>|<span data-ttu-id="7a962-159">Логический</span><span class="sxs-lookup"><span data-stu-id="7a962-159">Boolean</span></span>|<span data-ttu-id="7a962-160">Задайте значение true, если установлено напоминание пользователю о событии.</span><span class="sxs-lookup"><span data-stu-id="7a962-160">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="7a962-161">location</span><span class="sxs-lookup"><span data-stu-id="7a962-161">location</span></span>|<span data-ttu-id="7a962-162">Расположение</span><span class="sxs-lookup"><span data-stu-id="7a962-162">Location</span></span>|<span data-ttu-id="7a962-163">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="7a962-163">The location of the event.</span></span>|
|<span data-ttu-id="7a962-164">locations</span><span class="sxs-lookup"><span data-stu-id="7a962-164">locations</span></span>|<span data-ttu-id="7a962-165">Коллекция [Location](../resources/location.md)</span><span class="sxs-lookup"><span data-stu-id="7a962-165">[Location](../resources/location.md) collection</span></span>|<span data-ttu-id="7a962-166">Места проведения события или участия в нем.</span><span class="sxs-lookup"><span data-stu-id="7a962-166">The locations where the event is held or attended from.</span></span> <span data-ttu-id="7a962-167">Свойства **location** и **locations** всегда совпадают друг с другом.</span><span class="sxs-lookup"><span data-stu-id="7a962-167">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="7a962-168">Если вы обновите свойство **location**, предыдущие места в коллекции **locations** будут удалены и заменены новым значением **location**.</span><span class="sxs-lookup"><span data-stu-id="7a962-168">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="7a962-169">onlineMeetingProvider</span><span class="sxs-lookup"><span data-stu-id="7a962-169">onlineMeetingProvider</span></span>|<span data-ttu-id="7a962-170">onlineMeetingProviderType</span><span class="sxs-lookup"><span data-stu-id="7a962-170">onlineMeetingProviderType</span></span>| <span data-ttu-id="7a962-171">Представляет поставщика службы собраний по сети.</span><span class="sxs-lookup"><span data-stu-id="7a962-171">Represents the online meeting service provider.</span></span> <span data-ttu-id="7a962-172">Возможные значения: `teamsForBusiness`, `skypeForBusiness` и `skypeForConsumer`.</span><span class="sxs-lookup"><span data-stu-id="7a962-172">The possible values are `teamsForBusiness`, `skypeForBusiness`, and `skypeForConsumer`.</span></span> <span data-ttu-id="7a962-173">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="7a962-173">Optional.</span></span> |
| <span data-ttu-id="7a962-174">recurrence</span><span class="sxs-lookup"><span data-stu-id="7a962-174">recurrence</span></span>|<span data-ttu-id="7a962-175">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="7a962-175">PatternedRecurrence</span></span>|<span data-ttu-id="7a962-176">Расписание повторения события.</span><span class="sxs-lookup"><span data-stu-id="7a962-176">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="7a962-177">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="7a962-177">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="7a962-178">Int32</span><span class="sxs-lookup"><span data-stu-id="7a962-178">Int32</span></span>|<span data-ttu-id="7a962-179">Позволяет указать, за сколько минут до начала события появляется напоминание.</span><span class="sxs-lookup"><span data-stu-id="7a962-179">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="7a962-180">responseRequested</span><span class="sxs-lookup"><span data-stu-id="7a962-180">responseRequested</span></span>|<span data-ttu-id="7a962-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a962-181">Boolean</span></span>|<span data-ttu-id="7a962-182">Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения.</span><span class="sxs-lookup"><span data-stu-id="7a962-182">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="7a962-183">sensitivity</span><span class="sxs-lookup"><span data-stu-id="7a962-183">sensitivity</span></span>|<span data-ttu-id="7a962-184">String</span><span class="sxs-lookup"><span data-stu-id="7a962-184">String</span></span>| <span data-ttu-id="7a962-185">Возможные значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="7a962-185">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="7a962-186">showAs</span><span class="sxs-lookup"><span data-stu-id="7a962-186">showAs</span></span>|<span data-ttu-id="7a962-187">String</span><span class="sxs-lookup"><span data-stu-id="7a962-187">String</span></span>|<span data-ttu-id="7a962-188">Отображаемое состояние.</span><span class="sxs-lookup"><span data-stu-id="7a962-188">The status to show.</span></span> <span data-ttu-id="7a962-189">Возможные `free` значения:, `tentative`, `busy`, `oof`, `workingElsewhere`,. `unknown`</span><span class="sxs-lookup"><span data-stu-id="7a962-189">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="7a962-190">начать</span><span class="sxs-lookup"><span data-stu-id="7a962-190">start</span></span>|<span data-ttu-id="7a962-191">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="7a962-191">DateTimeTimeZone</span></span>|<span data-ttu-id="7a962-192">Дата, время и часовой пояс начала события.</span><span class="sxs-lookup"><span data-stu-id="7a962-192">The start date, time, and time zone of the event.</span></span> |
| <span data-ttu-id="7a962-193">subject</span><span class="sxs-lookup"><span data-stu-id="7a962-193">subject</span></span>|<span data-ttu-id="7a962-194">String</span><span class="sxs-lookup"><span data-stu-id="7a962-194">String</span></span>|<span data-ttu-id="7a962-195">Текст в строке темы сообщения о событии.</span><span class="sxs-lookup"><span data-stu-id="7a962-195">The text of the event's subject line.</span></span>|

<span data-ttu-id="7a962-196">Так как ресурс **event** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **event**.</span><span class="sxs-lookup"><span data-stu-id="7a962-196">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="7a962-197">Если обновляемый ресурс **event** является главным событием повторяющегося ряда, содержит несколько участников и экземпляры, обновленные отдельно, отправляется несколько сообщений электронной почты с уведомлениями: одно для главного ряда и по одному для каждого обновленного экземпляра.</span><span class="sxs-lookup"><span data-stu-id="7a962-197">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="7a962-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a962-198">Response</span></span>

<span data-ttu-id="7a962-199">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7a962-199">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="7a962-200">**Примечание.** Этот метод может вернуть отклик "HTTP 400 — ошибочный запрос" с кодом ошибки `ErrorOccurrenceCrossingBoundary` и следующим сообщением об ошибке: "Измененная копия пересекается со смежной копией или перекрывает ее".</span><span class="sxs-lookup"><span data-stu-id="7a962-200">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="7a962-201">Это означает, что обновление нарушает следующее ограничение Outlook для повторяющихся исключений: повторение нельзя перемещать на день предыдущего повторения или до него, а также на день следующего повторения или после него.</span><span class="sxs-lookup"><span data-stu-id="7a962-201">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="7a962-202">Пример</span><span class="sxs-lookup"><span data-stu-id="7a962-202">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7a962-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a962-203">Request</span></span>

<span data-ttu-id="7a962-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a962-204">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7a962-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a962-205">HTTP</span></span>](#tab/http)
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
  "isReminderOn": true
}
```
# <a name="c"></a>[<span data-ttu-id="7a962-206">C#</span><span class="sxs-lookup"><span data-stu-id="7a962-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a962-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a962-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7a962-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a962-208">Response</span></span>
<span data-ttu-id="7a962-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7a962-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NzIyNzhlMGEtM2YyZC00ZmY0LTlhNzUtZmZjNWFmZGNlNzE2%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22bc55b173-cff6-457d-b7a1-64bda7d7581a%22%7d",
        "conferenceId": "177513992",
        "tollNumber": "+91 22 6241 6885"
    }
}
```


## <a name="see-also"></a><span data-ttu-id="7a962-212">См. также</span><span class="sxs-lookup"><span data-stu-id="7a962-212">See also</span></span>

- [<span data-ttu-id="7a962-213">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="7a962-213">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7a962-214">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="7a962-214">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="7a962-215">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="7a962-215">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
