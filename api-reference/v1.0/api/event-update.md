---
title: Обновление события
description: Обновление свойств объекта event.
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4c9db9213b6245cc3a0c07c0bb590f0543055cb9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448265"
---
# <a name="update-event"></a><span data-ttu-id="922b6-103">Обновление события</span><span class="sxs-lookup"><span data-stu-id="922b6-103">Update event</span></span>

<span data-ttu-id="922b6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="922b6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="922b6-105">Обновление свойств объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="922b6-105">Update the properties of the [event](../resources/event.md) object.</span></span>

<span data-ttu-id="922b6-106">При обновлении часового пояса начала или завершения события сначала [найдите поддерживаемые часовые пояса](outlookuser-supportedtimezones.md), чтобы устанавливать только часовые пояса, настроенные для сервера почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="922b6-106">When updating the time zone of the start or end time of an event, first [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

## <a name="permissions"></a><span data-ttu-id="922b6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="922b6-107">Permissions</span></span>
<span data-ttu-id="922b6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="922b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="922b6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="922b6-110">Permission type</span></span>      | <span data-ttu-id="922b6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="922b6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="922b6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="922b6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="922b6-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="922b6-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="922b6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="922b6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="922b6-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="922b6-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="922b6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="922b6-116">Application</span></span> | <span data-ttu-id="922b6-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="922b6-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="922b6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="922b6-118">HTTP request</span></span>
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

PATCH /me/calendargroups/{id}/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="922b6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="922b6-119">Request headers</span></span>
| <span data-ttu-id="922b6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="922b6-120">Name</span></span>       | <span data-ttu-id="922b6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="922b6-121">Type</span></span> | <span data-ttu-id="922b6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="922b6-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="922b6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="922b6-123">Authorization</span></span>  | <span data-ttu-id="922b6-124">string</span><span class="sxs-lookup"><span data-stu-id="922b6-124">string</span></span>  | <span data-ttu-id="922b6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="922b6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="922b6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="922b6-127">Request body</span></span>
<span data-ttu-id="922b6-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="922b6-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="922b6-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="922b6-131">Property</span></span>     | <span data-ttu-id="922b6-132">Тип</span><span class="sxs-lookup"><span data-stu-id="922b6-132">Type</span></span>   |<span data-ttu-id="922b6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="922b6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="922b6-134">attendees</span><span class="sxs-lookup"><span data-stu-id="922b6-134">attendees</span></span>|[<span data-ttu-id="922b6-135">Attendee</span><span class="sxs-lookup"><span data-stu-id="922b6-135">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="922b6-136">Коллекция участников события.</span><span class="sxs-lookup"><span data-stu-id="922b6-136">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="922b6-137">body</span><span class="sxs-lookup"><span data-stu-id="922b6-137">body</span></span>|[<span data-ttu-id="922b6-138">ItemBody</span><span class="sxs-lookup"><span data-stu-id="922b6-138">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="922b6-139">Текст сообщения, связанного с событием.</span><span class="sxs-lookup"><span data-stu-id="922b6-139">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="922b6-140">categories</span><span class="sxs-lookup"><span data-stu-id="922b6-140">categories</span></span>|<span data-ttu-id="922b6-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="922b6-141">String collection</span></span>|<span data-ttu-id="922b6-142">Категории, связанные с событием.</span><span class="sxs-lookup"><span data-stu-id="922b6-142">The categories associated with the event.</span></span>|
| <span data-ttu-id="922b6-143">end</span><span class="sxs-lookup"><span data-stu-id="922b6-143">end</span></span>|<span data-ttu-id="922b6-144">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="922b6-144">DateTimeTimeZone</span></span>|<span data-ttu-id="922b6-145">Дата, время и часовой пояс завершения события.</span><span class="sxs-lookup"><span data-stu-id="922b6-145">The date, time, and time zone that the event ends.</span></span>|
|<span data-ttu-id="922b6-146">hideAttendees</span><span class="sxs-lookup"><span data-stu-id="922b6-146">hideAttendees</span></span>|<span data-ttu-id="922b6-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b6-147">Boolean</span></span>|<span data-ttu-id="922b6-148">Если присвоено значение `true`, каждый участник видит только себя в приглашении на собрание и списке собрания **Отслеживание**.</span><span class="sxs-lookup"><span data-stu-id="922b6-148">When set to `true`, each attendee only sees themselves in the meeting request and meeting **Tracking** list.</span></span> <span data-ttu-id="922b6-149">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="922b6-149">Default is false.</span></span>|
|<span data-ttu-id="922b6-150">importance</span><span class="sxs-lookup"><span data-stu-id="922b6-150">importance</span></span>|<span data-ttu-id="922b6-151">String</span><span class="sxs-lookup"><span data-stu-id="922b6-151">String</span></span>|<span data-ttu-id="922b6-152">Важность события.</span><span class="sxs-lookup"><span data-stu-id="922b6-152">The importance of the event.</span></span> <span data-ttu-id="922b6-153">Допустимые значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="922b6-153">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="922b6-154">isAllDay</span><span class="sxs-lookup"><span data-stu-id="922b6-154">isAllDay</span></span>|<span data-ttu-id="922b6-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b6-155">Boolean</span></span>|<span data-ttu-id="922b6-156">Задайте значение true, если событие длится весь день.</span><span class="sxs-lookup"><span data-stu-id="922b6-156">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="922b6-157">isOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="922b6-157">isOnlineMeeting</span></span>|<span data-ttu-id="922b6-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b6-158">Boolean</span></span>| <span data-ttu-id="922b6-159">`True`, если это событие содержит информацию о собраниях по сети; в противном случае — `false`.</span><span class="sxs-lookup"><span data-stu-id="922b6-159">`True` if this event has online meeting information, `false` otherwise.</span></span> <span data-ttu-id="922b6-160">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="922b6-160">Default is false.</span></span> <span data-ttu-id="922b6-161">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="922b6-161">Optional.</span></span>|
|<span data-ttu-id="922b6-162">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="922b6-162">isReminderOn</span></span>|<span data-ttu-id="922b6-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b6-163">Boolean</span></span>|<span data-ttu-id="922b6-164">Задайте значение true, если установлено напоминание пользователю о событии.</span><span class="sxs-lookup"><span data-stu-id="922b6-164">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="922b6-165">location</span><span class="sxs-lookup"><span data-stu-id="922b6-165">location</span></span>|[<span data-ttu-id="922b6-166">Location</span><span class="sxs-lookup"><span data-stu-id="922b6-166">Location</span></span>](../resources/location.md)|<span data-ttu-id="922b6-167">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="922b6-167">The location of the event.</span></span>|
|<span data-ttu-id="922b6-168">locations</span><span class="sxs-lookup"><span data-stu-id="922b6-168">locations</span></span>|<span data-ttu-id="922b6-169">Коллекция [location](../resources/location.md)</span><span class="sxs-lookup"><span data-stu-id="922b6-169">[location](../resources/location.md) collection</span></span>|<span data-ttu-id="922b6-170">Места проведения мероприятия или участия в нем.</span><span class="sxs-lookup"><span data-stu-id="922b6-170">The locations where the event is held or attended from.</span></span> <span data-ttu-id="922b6-171">Свойства **location** и **locations** всегда совпадают друг с другом.</span><span class="sxs-lookup"><span data-stu-id="922b6-171">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="922b6-172">Если вы обновите свойство **location**, предыдущие места в коллекции **locations** будут удалены и заменены новым значением **location**.</span><span class="sxs-lookup"><span data-stu-id="922b6-172">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="922b6-173">onlineMeetingProvider</span><span class="sxs-lookup"><span data-stu-id="922b6-173">onlineMeetingProvider</span></span>|<span data-ttu-id="922b6-174">onlineMeetingProviderType</span><span class="sxs-lookup"><span data-stu-id="922b6-174">onlineMeetingProviderType</span></span>| <span data-ttu-id="922b6-175">Представляет поставщика службы собраний по сети.</span><span class="sxs-lookup"><span data-stu-id="922b6-175">Represents the online meeting service provider.</span></span> <span data-ttu-id="922b6-176">Возможные значения: `teamsForBusiness`, `skypeForBusiness` и `skypeForConsumer`.</span><span class="sxs-lookup"><span data-stu-id="922b6-176">The possible values are `teamsForBusiness`, `skypeForBusiness`, and `skypeForConsumer`.</span></span> <span data-ttu-id="922b6-177">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="922b6-177">Optional.</span></span> |
|<span data-ttu-id="922b6-178">recurrence</span><span class="sxs-lookup"><span data-stu-id="922b6-178">recurrence</span></span>|[<span data-ttu-id="922b6-179">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="922b6-179">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="922b6-180">Расписание повторения события.</span><span class="sxs-lookup"><span data-stu-id="922b6-180">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="922b6-181">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="922b6-181">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="922b6-182">Int32</span><span class="sxs-lookup"><span data-stu-id="922b6-182">Int32</span></span>|<span data-ttu-id="922b6-183">Позволяет указать, за сколько минут до начала события появляется напоминание.</span><span class="sxs-lookup"><span data-stu-id="922b6-183">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="922b6-184">responseRequested</span><span class="sxs-lookup"><span data-stu-id="922b6-184">responseRequested</span></span>|<span data-ttu-id="922b6-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b6-185">Boolean</span></span>|<span data-ttu-id="922b6-186">Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения.</span><span class="sxs-lookup"><span data-stu-id="922b6-186">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="922b6-187">sensitivity</span><span class="sxs-lookup"><span data-stu-id="922b6-187">sensitivity</span></span>|<span data-ttu-id="922b6-188">String</span><span class="sxs-lookup"><span data-stu-id="922b6-188">String</span></span>| <span data-ttu-id="922b6-189">Допустимые значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="922b6-189">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="922b6-190">showAs</span><span class="sxs-lookup"><span data-stu-id="922b6-190">showAs</span></span>|<span data-ttu-id="922b6-191">String</span><span class="sxs-lookup"><span data-stu-id="922b6-191">String</span></span>|<span data-ttu-id="922b6-192">Отображаемое состояние.</span><span class="sxs-lookup"><span data-stu-id="922b6-192">The status to show.</span></span> <span data-ttu-id="922b6-193">Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="922b6-193">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="922b6-194">начать</span><span class="sxs-lookup"><span data-stu-id="922b6-194">start</span></span>|<span data-ttu-id="922b6-195">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="922b6-195">DateTimeTimeZone</span></span>|<span data-ttu-id="922b6-196">Дата, время и часовой пояс начала события.</span><span class="sxs-lookup"><span data-stu-id="922b6-196">The start date, time, and time zone of the event.</span></span> |
|<span data-ttu-id="922b6-197">subject</span><span class="sxs-lookup"><span data-stu-id="922b6-197">subject</span></span>|<span data-ttu-id="922b6-198">String</span><span class="sxs-lookup"><span data-stu-id="922b6-198">String</span></span>|<span data-ttu-id="922b6-199">Текст в строке темы сообщения о событии.</span><span class="sxs-lookup"><span data-stu-id="922b6-199">The text of the event's subject line.</span></span>|

<span data-ttu-id="922b6-200">Так как ресурс **event** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **event**.</span><span class="sxs-lookup"><span data-stu-id="922b6-200">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>  
  
<span data-ttu-id="922b6-201">Если обновляемый ресурс **event** является главным событием повторяющегося ряда, содержит несколько участников и экземпляры, обновленные отдельно, отправляется несколько сообщений электронной почты с уведомлениями: одно для главного ряда и по одному для каждого обновленного экземпляра.</span><span class="sxs-lookup"><span data-stu-id="922b6-201">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>  

## <a name="response"></a><span data-ttu-id="922b6-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="922b6-202">Response</span></span>

<span data-ttu-id="922b6-203">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="922b6-203">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>  

><span data-ttu-id="922b6-204">**Примечание.** Этот метод может вернуть отклик "HTTP 400 — ошибочный запрос" с кодом ошибки `ErrorOccurrenceCrossingBoundary` и следующим сообщением об ошибке: "Измененная копия пересекается со смежной копией или перекрывает ее".</span><span class="sxs-lookup"><span data-stu-id="922b6-204">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="922b6-205">Это означает, что обновление нарушает следующее ограничение Outlook для повторяющихся исключений: повторение нельзя перемещать на день предыдущего повторения или до него, а также на день следующего повторения или после него.</span><span class="sxs-lookup"><span data-stu-id="922b6-205">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="922b6-206">Пример</span><span class="sxs-lookup"><span data-stu-id="922b6-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="922b6-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="922b6-207">Request</span></span>

<span data-ttu-id="922b6-208">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="922b6-208">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="922b6-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="922b6-209">HTTP</span></span>](#tab/http)
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
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness",
  "isReminderOn": true,
  "hideAttendees": false,
  "categories": ["Red category"]
}
```
# <a name="c"></a>[<span data-ttu-id="922b6-210">C#</span><span class="sxs-lookup"><span data-stu-id="922b6-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="922b6-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="922b6-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="922b6-212">Java</span><span class="sxs-lookup"><span data-stu-id="922b6-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="922b6-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="922b6-213">Response</span></span>

<span data-ttu-id="922b6-214">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="922b6-214">Here is an example of the response.</span></span> <span data-ttu-id="922b6-215">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="922b6-215">Note: The response object shown here may be truncated for brevity.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="922b6-216">См. также</span><span class="sxs-lookup"><span data-stu-id="922b6-216">See also</span></span>

- [<span data-ttu-id="922b6-217">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="922b6-217">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="922b6-218">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="922b6-218">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="922b6-219">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="922b6-219">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)



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

