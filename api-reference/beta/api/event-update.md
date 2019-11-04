---
title: Обновление события
description: Обновление свойств объекта event.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ef2b53a9b907146c91bb66e269c6f604c2b26d57
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938690"
---
# <a name="update-event"></a><span data-ttu-id="8d117-103">Обновление события</span><span class="sxs-lookup"><span data-stu-id="8d117-103">Update event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d117-104">Обновление свойств объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="8d117-104">Update the properties of the [event](../resources/event.md) object.</span></span>

<span data-ttu-id="8d117-105">При обновлении часового пояса начала или завершения события сначала [найдите поддерживаемые часовые пояса](outlookuser-supportedtimezones.md), чтобы устанавливать только часовые пояса, настроенные для сервера почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="8d117-105">When updating the time zone of the start or end time of an event, first [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8d117-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d117-106">Permissions</span></span>
<span data-ttu-id="8d117-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d117-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d117-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d117-109">Permission type</span></span>      | <span data-ttu-id="8d117-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d117-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d117-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d117-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8d117-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d117-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8d117-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d117-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d117-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d117-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8d117-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d117-115">Application</span></span> | <span data-ttu-id="8d117-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d117-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d117-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d117-117">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="8d117-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d117-118">Request headers</span></span>
| <span data-ttu-id="8d117-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8d117-119">Name</span></span>       | <span data-ttu-id="8d117-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8d117-120">Type</span></span> | <span data-ttu-id="8d117-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8d117-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8d117-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d117-122">Authorization</span></span>  | <span data-ttu-id="8d117-123">string</span><span class="sxs-lookup"><span data-stu-id="8d117-123">string</span></span>  | <span data-ttu-id="8d117-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d117-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d117-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d117-126">Request body</span></span>
<span data-ttu-id="8d117-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8d117-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8d117-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d117-130">Property</span></span>       | <span data-ttu-id="8d117-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8d117-131">Type</span></span>    | <span data-ttu-id="8d117-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8d117-132">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="8d117-133">attendees</span><span class="sxs-lookup"><span data-stu-id="8d117-133">attendees</span></span>|<span data-ttu-id="8d117-134">Attendee</span><span class="sxs-lookup"><span data-stu-id="8d117-134">Attendee</span></span>|<span data-ttu-id="8d117-135">Коллекция участников события.</span><span class="sxs-lookup"><span data-stu-id="8d117-135">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="8d117-136">body</span><span class="sxs-lookup"><span data-stu-id="8d117-136">body</span></span>|<span data-ttu-id="8d117-137">ItemBody</span><span class="sxs-lookup"><span data-stu-id="8d117-137">ItemBody</span></span>|<span data-ttu-id="8d117-138">Текст сообщения, связанного с событием.</span><span class="sxs-lookup"><span data-stu-id="8d117-138">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="8d117-139">categories</span><span class="sxs-lookup"><span data-stu-id="8d117-139">categories</span></span>|<span data-ttu-id="8d117-140">String</span><span class="sxs-lookup"><span data-stu-id="8d117-140">String</span></span>|<span data-ttu-id="8d117-141">Категории, связанные с событием.</span><span class="sxs-lookup"><span data-stu-id="8d117-141">The categories associated with the event.</span></span>|
| <span data-ttu-id="8d117-142">end</span><span class="sxs-lookup"><span data-stu-id="8d117-142">end</span></span>|<span data-ttu-id="8d117-143">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8d117-143">DateTimeTimeZone</span></span>|<span data-ttu-id="8d117-144">Дата, время и часовой пояс завершения события.</span><span class="sxs-lookup"><span data-stu-id="8d117-144">The date, time, and time zone that the event ends.</span></span> |
| <span data-ttu-id="8d117-145">importance</span><span class="sxs-lookup"><span data-stu-id="8d117-145">importance</span></span>|<span data-ttu-id="8d117-146">String</span><span class="sxs-lookup"><span data-stu-id="8d117-146">String</span></span>|<span data-ttu-id="8d117-147">Важность события.</span><span class="sxs-lookup"><span data-stu-id="8d117-147">The importance of the event.</span></span> <span data-ttu-id="8d117-148">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="8d117-148">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="8d117-149">isAllDay</span><span class="sxs-lookup"><span data-stu-id="8d117-149">isAllDay</span></span>|<span data-ttu-id="8d117-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d117-150">Boolean</span></span>|<span data-ttu-id="8d117-151">Задайте значение true, если событие длится весь день.</span><span class="sxs-lookup"><span data-stu-id="8d117-151">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="8d117-152">исонлинемитинг</span><span class="sxs-lookup"><span data-stu-id="8d117-152">isOnlineMeeting</span></span>|<span data-ttu-id="8d117-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d117-153">Boolean</span></span>| <span data-ttu-id="8d117-154">`True`, если это событие содержит сведения о собрании по сети, `false` в противном случае.</span><span class="sxs-lookup"><span data-stu-id="8d117-154">`True` if this event has online meeting information, `false` otherwise.</span></span> <span data-ttu-id="8d117-155">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="8d117-155">Default is false.</span></span> <span data-ttu-id="8d117-156">Необязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="8d117-156">Optional.</span></span>|
| <span data-ttu-id="8d117-157">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="8d117-157">isReminderOn</span></span>|<span data-ttu-id="8d117-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d117-158">Boolean</span></span>|<span data-ttu-id="8d117-159">Задайте значение true, если установлено напоминание пользователю о событии.</span><span class="sxs-lookup"><span data-stu-id="8d117-159">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="8d117-160">location</span><span class="sxs-lookup"><span data-stu-id="8d117-160">location</span></span>|<span data-ttu-id="8d117-161">Расположение</span><span class="sxs-lookup"><span data-stu-id="8d117-161">Location</span></span>|<span data-ttu-id="8d117-162">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="8d117-162">The location of the event.</span></span>|
|<span data-ttu-id="8d117-163">locations</span><span class="sxs-lookup"><span data-stu-id="8d117-163">locations</span></span>|<span data-ttu-id="8d117-164">Коллекция [Location](../resources/location.md)</span><span class="sxs-lookup"><span data-stu-id="8d117-164">[Location](../resources/location.md) collection</span></span>|<span data-ttu-id="8d117-165">Места проведения события или участия в нем.</span><span class="sxs-lookup"><span data-stu-id="8d117-165">The locations where the event is held or attended from.</span></span> <span data-ttu-id="8d117-166">Свойства **location** и **locations** всегда совпадают друг с другом.</span><span class="sxs-lookup"><span data-stu-id="8d117-166">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="8d117-167">Если вы обновите свойство **location**, предыдущие места в коллекции **locations** будут удалены и заменены новым значением **location**.</span><span class="sxs-lookup"><span data-stu-id="8d117-167">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="8d117-168">онлинемитингпровидер</span><span class="sxs-lookup"><span data-stu-id="8d117-168">onlineMeetingProvider</span></span>|<span data-ttu-id="8d117-169">онлинемитингпровидертипе</span><span class="sxs-lookup"><span data-stu-id="8d117-169">onlineMeetingProviderType</span></span>| <span data-ttu-id="8d117-170">Представляет поставщика службы собраний по сети.</span><span class="sxs-lookup"><span data-stu-id="8d117-170">Represents the online meeting service provider.</span></span> <span data-ttu-id="8d117-171">Возможные значения: `teamsForBusiness`, `skypeForBusiness`и. `skypeForConsumer`</span><span class="sxs-lookup"><span data-stu-id="8d117-171">The possible values are `teamsForBusiness`, `skypeForBusiness`, and `skypeForConsumer`.</span></span> <span data-ttu-id="8d117-172">Необязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="8d117-172">Optional.</span></span> |
| <span data-ttu-id="8d117-173">recurrence</span><span class="sxs-lookup"><span data-stu-id="8d117-173">recurrence</span></span>|<span data-ttu-id="8d117-174">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="8d117-174">PatternedRecurrence</span></span>|<span data-ttu-id="8d117-175">Расписание повторения события.</span><span class="sxs-lookup"><span data-stu-id="8d117-175">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="8d117-176">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="8d117-176">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="8d117-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8d117-177">Int32</span></span>|<span data-ttu-id="8d117-178">Позволяет указать, за сколько минут до начала события появляется напоминание.</span><span class="sxs-lookup"><span data-stu-id="8d117-178">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="8d117-179">responseRequested</span><span class="sxs-lookup"><span data-stu-id="8d117-179">responseRequested</span></span>|<span data-ttu-id="8d117-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d117-180">Boolean</span></span>|<span data-ttu-id="8d117-181">Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения.</span><span class="sxs-lookup"><span data-stu-id="8d117-181">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="8d117-182">sensitivity</span><span class="sxs-lookup"><span data-stu-id="8d117-182">sensitivity</span></span>|<span data-ttu-id="8d117-183">String</span><span class="sxs-lookup"><span data-stu-id="8d117-183">String</span></span>| <span data-ttu-id="8d117-184">Возможные значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="8d117-184">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="8d117-185">showAs</span><span class="sxs-lookup"><span data-stu-id="8d117-185">showAs</span></span>|<span data-ttu-id="8d117-186">String</span><span class="sxs-lookup"><span data-stu-id="8d117-186">String</span></span>|<span data-ttu-id="8d117-187">Отображаемое состояние.</span><span class="sxs-lookup"><span data-stu-id="8d117-187">The status to show.</span></span> <span data-ttu-id="8d117-188">Возможные `free` значения:, `tentative`, `busy`, `oof`, `workingElsewhere`,. `unknown`</span><span class="sxs-lookup"><span data-stu-id="8d117-188">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="8d117-189">начать</span><span class="sxs-lookup"><span data-stu-id="8d117-189">start</span></span>|<span data-ttu-id="8d117-190">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8d117-190">DateTimeTimeZone</span></span>|<span data-ttu-id="8d117-191">Дата, время и часовой пояс начала события.</span><span class="sxs-lookup"><span data-stu-id="8d117-191">The start date, time, and time zone of the event.</span></span> |
| <span data-ttu-id="8d117-192">subject</span><span class="sxs-lookup"><span data-stu-id="8d117-192">subject</span></span>|<span data-ttu-id="8d117-193">String</span><span class="sxs-lookup"><span data-stu-id="8d117-193">String</span></span>|<span data-ttu-id="8d117-194">Текст в строке темы сообщения о событии.</span><span class="sxs-lookup"><span data-stu-id="8d117-194">The text of the event's subject line.</span></span>|

<span data-ttu-id="8d117-195">Так как ресурс **event** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **event**.</span><span class="sxs-lookup"><span data-stu-id="8d117-195">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="8d117-196">Если обновляемый ресурс **event** является главным событием повторяющегося ряда, содержит несколько участников и экземпляры, обновленные отдельно, отправляется несколько сообщений электронной почты с уведомлениями: одно для главного ряда и по одному для каждого обновленного экземпляра.</span><span class="sxs-lookup"><span data-stu-id="8d117-196">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="8d117-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d117-197">Response</span></span>

<span data-ttu-id="8d117-198">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8d117-198">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="8d117-199">**Примечание.** Этот метод может вернуть отклик "HTTP 400 — ошибочный запрос" с кодом ошибки `ErrorOccurrenceCrossingBoundary` и следующим сообщением об ошибке: "Измененная копия пересекается со смежной копией или перекрывает ее".</span><span class="sxs-lookup"><span data-stu-id="8d117-199">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="8d117-200">Это означает, что обновление нарушает следующее ограничение Outlook для повторяющихся исключений: повторение нельзя перемещать на день предыдущего повторения или до него, а также на день следующего повторения или после него.</span><span class="sxs-lookup"><span data-stu-id="8d117-200">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="8d117-201">Пример</span><span class="sxs-lookup"><span data-stu-id="8d117-201">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8d117-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d117-202">Request</span></span>

<span data-ttu-id="8d117-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d117-203">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8d117-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d117-204">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8d117-205">C#</span><span class="sxs-lookup"><span data-stu-id="8d117-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8d117-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d117-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8d117-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d117-207">Response</span></span>
<span data-ttu-id="8d117-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8d117-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="8d117-211">См. также</span><span class="sxs-lookup"><span data-stu-id="8d117-211">See also</span></span>

- [<span data-ttu-id="8d117-212">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="8d117-212">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="8d117-213">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="8d117-213">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="8d117-214">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="8d117-214">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
