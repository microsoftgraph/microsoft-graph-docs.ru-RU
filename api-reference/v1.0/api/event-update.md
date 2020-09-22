---
title: Обновление события
description: Обновление свойств объекта event.
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3491288db2480c24440ad33e209236125c570426
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038769"
---
# <a name="update-event"></a><span data-ttu-id="d47e7-103">Обновление события</span><span class="sxs-lookup"><span data-stu-id="d47e7-103">Update event</span></span>

<span data-ttu-id="d47e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d47e7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d47e7-105">Обновление свойств объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="d47e7-105">Update the properties of the [event](../resources/event.md) object.</span></span>

<span data-ttu-id="d47e7-106">При обновлении часового пояса начала или завершения события сначала [найдите поддерживаемые часовые пояса](outlookuser-supportedtimezones.md), чтобы устанавливать только часовые пояса, настроенные для сервера почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="d47e7-106">When updating the time zone of the start or end time of an event, first [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d47e7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d47e7-107">Permissions</span></span>
<span data-ttu-id="d47e7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d47e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d47e7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d47e7-110">Permission type</span></span>      | <span data-ttu-id="d47e7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d47e7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d47e7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d47e7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d47e7-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d47e7-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d47e7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d47e7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d47e7-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d47e7-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d47e7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d47e7-116">Application</span></span> | <span data-ttu-id="d47e7-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d47e7-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d47e7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d47e7-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="d47e7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d47e7-119">Request headers</span></span>
| <span data-ttu-id="d47e7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d47e7-120">Name</span></span>       | <span data-ttu-id="d47e7-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d47e7-121">Type</span></span> | <span data-ttu-id="d47e7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d47e7-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d47e7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d47e7-123">Authorization</span></span>  | <span data-ttu-id="d47e7-124">string</span><span class="sxs-lookup"><span data-stu-id="d47e7-124">string</span></span>  | <span data-ttu-id="d47e7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d47e7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d47e7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d47e7-127">Request body</span></span>
<span data-ttu-id="d47e7-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d47e7-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d47e7-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="d47e7-131">Property</span></span>     | <span data-ttu-id="d47e7-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d47e7-132">Type</span></span>   |<span data-ttu-id="d47e7-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d47e7-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d47e7-134">attendees</span><span class="sxs-lookup"><span data-stu-id="d47e7-134">attendees</span></span>|[<span data-ttu-id="d47e7-135">Attendee</span><span class="sxs-lookup"><span data-stu-id="d47e7-135">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="d47e7-136">Коллекция участников события.</span><span class="sxs-lookup"><span data-stu-id="d47e7-136">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="d47e7-137">body</span><span class="sxs-lookup"><span data-stu-id="d47e7-137">body</span></span>|[<span data-ttu-id="d47e7-138">ItemBody</span><span class="sxs-lookup"><span data-stu-id="d47e7-138">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="d47e7-139">Текст сообщения, связанного с событием.</span><span class="sxs-lookup"><span data-stu-id="d47e7-139">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="d47e7-140">categories</span><span class="sxs-lookup"><span data-stu-id="d47e7-140">categories</span></span>|<span data-ttu-id="d47e7-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d47e7-141">String collection</span></span>|<span data-ttu-id="d47e7-142">Категории, связанные с событием.</span><span class="sxs-lookup"><span data-stu-id="d47e7-142">The categories associated with the event.</span></span>|
| <span data-ttu-id="d47e7-143">end</span><span class="sxs-lookup"><span data-stu-id="d47e7-143">end</span></span>|<span data-ttu-id="d47e7-144">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d47e7-144">DateTimeTimeZone</span></span>|<span data-ttu-id="d47e7-145">Дата, время и часовой пояс завершения события.</span><span class="sxs-lookup"><span data-stu-id="d47e7-145">The date, time, and time zone that the event ends.</span></span>|
|<span data-ttu-id="d47e7-146">importance</span><span class="sxs-lookup"><span data-stu-id="d47e7-146">importance</span></span>|<span data-ttu-id="d47e7-147">String</span><span class="sxs-lookup"><span data-stu-id="d47e7-147">String</span></span>|<span data-ttu-id="d47e7-148">Важность события.</span><span class="sxs-lookup"><span data-stu-id="d47e7-148">The importance of the event.</span></span> <span data-ttu-id="d47e7-149">Допустимые значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="d47e7-149">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="d47e7-150">isAllDay</span><span class="sxs-lookup"><span data-stu-id="d47e7-150">isAllDay</span></span>|<span data-ttu-id="d47e7-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="d47e7-151">Boolean</span></span>|<span data-ttu-id="d47e7-152">Задайте значение true, если событие длится весь день.</span><span class="sxs-lookup"><span data-stu-id="d47e7-152">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="d47e7-153">isOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="d47e7-153">isOnlineMeeting</span></span>|<span data-ttu-id="d47e7-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="d47e7-154">Boolean</span></span>| <span data-ttu-id="d47e7-155">`True`, если это событие содержит информацию о собраниях по сети; в противном случае — `false`.</span><span class="sxs-lookup"><span data-stu-id="d47e7-155">`True` if this event has online meeting information, `false` otherwise.</span></span> <span data-ttu-id="d47e7-156">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="d47e7-156">Default is false.</span></span> <span data-ttu-id="d47e7-157">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d47e7-157">Optional.</span></span>|
|<span data-ttu-id="d47e7-158">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="d47e7-158">isReminderOn</span></span>|<span data-ttu-id="d47e7-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="d47e7-159">Boolean</span></span>|<span data-ttu-id="d47e7-160">Задайте значение true, если установлено напоминание пользователю о событии.</span><span class="sxs-lookup"><span data-stu-id="d47e7-160">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="d47e7-161">location</span><span class="sxs-lookup"><span data-stu-id="d47e7-161">location</span></span>|[<span data-ttu-id="d47e7-162">Location</span><span class="sxs-lookup"><span data-stu-id="d47e7-162">Location</span></span>](../resources/location.md)|<span data-ttu-id="d47e7-163">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="d47e7-163">The location of the event.</span></span>|
|<span data-ttu-id="d47e7-164">locations</span><span class="sxs-lookup"><span data-stu-id="d47e7-164">locations</span></span>|<span data-ttu-id="d47e7-165">Коллекция [location](../resources/location.md)</span><span class="sxs-lookup"><span data-stu-id="d47e7-165">[location](../resources/location.md) collection</span></span>|<span data-ttu-id="d47e7-166">Места проведения мероприятия или участия в нем.</span><span class="sxs-lookup"><span data-stu-id="d47e7-166">The locations where the event is held or attended from.</span></span> <span data-ttu-id="d47e7-167">Свойства **location** и **locations** всегда совпадают друг с другом.</span><span class="sxs-lookup"><span data-stu-id="d47e7-167">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="d47e7-168">Если вы обновите свойство **location**, предыдущие места в коллекции **locations** будут удалены и заменены новым значением **location**.</span><span class="sxs-lookup"><span data-stu-id="d47e7-168">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="d47e7-169">onlineMeetingProvider</span><span class="sxs-lookup"><span data-stu-id="d47e7-169">onlineMeetingProvider</span></span>|<span data-ttu-id="d47e7-170">onlineMeetingProviderType</span><span class="sxs-lookup"><span data-stu-id="d47e7-170">onlineMeetingProviderType</span></span>| <span data-ttu-id="d47e7-171">Представляет поставщика службы собраний по сети.</span><span class="sxs-lookup"><span data-stu-id="d47e7-171">Represents the online meeting service provider.</span></span> <span data-ttu-id="d47e7-172">Возможные значения: `teamsForBusiness`, `skypeForBusiness` и `skypeForConsumer`.</span><span class="sxs-lookup"><span data-stu-id="d47e7-172">The possible values are `teamsForBusiness`, `skypeForBusiness`, and `skypeForConsumer`.</span></span> <span data-ttu-id="d47e7-173">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d47e7-173">Optional.</span></span> |
|<span data-ttu-id="d47e7-174">recurrence</span><span class="sxs-lookup"><span data-stu-id="d47e7-174">recurrence</span></span>|[<span data-ttu-id="d47e7-175">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="d47e7-175">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="d47e7-176">Расписание повторения события.</span><span class="sxs-lookup"><span data-stu-id="d47e7-176">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="d47e7-177">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="d47e7-177">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="d47e7-178">Int32</span><span class="sxs-lookup"><span data-stu-id="d47e7-178">Int32</span></span>|<span data-ttu-id="d47e7-179">Позволяет указать, за сколько минут до начала события появляется напоминание.</span><span class="sxs-lookup"><span data-stu-id="d47e7-179">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="d47e7-180">responseRequested</span><span class="sxs-lookup"><span data-stu-id="d47e7-180">responseRequested</span></span>|<span data-ttu-id="d47e7-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="d47e7-181">Boolean</span></span>|<span data-ttu-id="d47e7-182">Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения.</span><span class="sxs-lookup"><span data-stu-id="d47e7-182">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="d47e7-183">sensitivity</span><span class="sxs-lookup"><span data-stu-id="d47e7-183">sensitivity</span></span>|<span data-ttu-id="d47e7-184">String</span><span class="sxs-lookup"><span data-stu-id="d47e7-184">String</span></span>| <span data-ttu-id="d47e7-185">Допустимые значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="d47e7-185">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="d47e7-186">showAs</span><span class="sxs-lookup"><span data-stu-id="d47e7-186">showAs</span></span>|<span data-ttu-id="d47e7-187">String</span><span class="sxs-lookup"><span data-stu-id="d47e7-187">String</span></span>|<span data-ttu-id="d47e7-188">Отображаемое состояние.</span><span class="sxs-lookup"><span data-stu-id="d47e7-188">The status to show.</span></span> <span data-ttu-id="d47e7-189">Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d47e7-189">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="d47e7-190">начать</span><span class="sxs-lookup"><span data-stu-id="d47e7-190">start</span></span>|<span data-ttu-id="d47e7-191">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d47e7-191">DateTimeTimeZone</span></span>|<span data-ttu-id="d47e7-192">Дата, время и часовой пояс начала события.</span><span class="sxs-lookup"><span data-stu-id="d47e7-192">The start date, time, and time zone of the event.</span></span> |
|<span data-ttu-id="d47e7-193">subject</span><span class="sxs-lookup"><span data-stu-id="d47e7-193">subject</span></span>|<span data-ttu-id="d47e7-194">String</span><span class="sxs-lookup"><span data-stu-id="d47e7-194">String</span></span>|<span data-ttu-id="d47e7-195">Текст в строке темы сообщения о событии.</span><span class="sxs-lookup"><span data-stu-id="d47e7-195">The text of the event's subject line.</span></span>|

<span data-ttu-id="d47e7-196">Так как ресурс **event** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **event**.</span><span class="sxs-lookup"><span data-stu-id="d47e7-196">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>  
  
<span data-ttu-id="d47e7-197">Если обновляемый ресурс **event** является главным событием повторяющегося ряда, содержит несколько участников и экземпляры, обновленные отдельно, отправляется несколько сообщений электронной почты с уведомлениями: одно для главного ряда и по одному для каждого обновленного экземпляра.</span><span class="sxs-lookup"><span data-stu-id="d47e7-197">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>  

## <a name="response"></a><span data-ttu-id="d47e7-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="d47e7-198">Response</span></span>

<span data-ttu-id="d47e7-199">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d47e7-199">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>  

><span data-ttu-id="d47e7-200">**Примечание.** Этот метод может вернуть отклик "HTTP 400 — ошибочный запрос" с кодом ошибки `ErrorOccurrenceCrossingBoundary` и следующим сообщением об ошибке: "Измененная копия пересекается со смежной копией или перекрывает ее".</span><span class="sxs-lookup"><span data-stu-id="d47e7-200">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="d47e7-201">Это означает, что обновление нарушает следующее ограничение Outlook для повторяющихся исключений: повторение нельзя перемещать на день предыдущего повторения или до него, а также на день следующего повторения или после него.</span><span class="sxs-lookup"><span data-stu-id="d47e7-201">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="d47e7-202">Пример</span><span class="sxs-lookup"><span data-stu-id="d47e7-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="d47e7-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="d47e7-203">Request</span></span>

<span data-ttu-id="d47e7-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d47e7-204">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d47e7-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="d47e7-205">HTTP</span></span>](#tab/http)
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
  "categories": ["Red category"]
}
```
# <a name="c"></a>[<span data-ttu-id="d47e7-206">C#</span><span class="sxs-lookup"><span data-stu-id="d47e7-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d47e7-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d47e7-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d47e7-208">Java</span><span class="sxs-lookup"><span data-stu-id="d47e7-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d47e7-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="d47e7-209">Response</span></span>

<span data-ttu-id="d47e7-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d47e7-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NzIyNzhlMGEtM2YyZC00ZmY0LTlhNzUtZmZjNWFmZGNlNzE2%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22bc55b173-cff6-457d-b7a1-64bda7d7581a%22%7d",
        "conferenceId": "177513992",
        "tollNumber": "+91 22 6241 6885"
  }
}
```

## <a name="see-also"></a><span data-ttu-id="d47e7-213">См. также</span><span class="sxs-lookup"><span data-stu-id="d47e7-213">See also</span></span>

- [<span data-ttu-id="d47e7-214">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="d47e7-214">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d47e7-215">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="d47e7-215">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="d47e7-216">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="d47e7-216">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)



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

