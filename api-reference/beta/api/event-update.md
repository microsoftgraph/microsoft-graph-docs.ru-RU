---
title: Обновление события
description: Обновление свойств объекта event.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 36f7c643bd843f20488304dbc365455c01877354
ms.sourcegitcommit: 6fe086e6a9396a71a82179853547cb7b5e22d980
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/20/2019
ms.locfileid: "35805069"
---
# <a name="update-event"></a><span data-ttu-id="8fba6-103">Обновление события</span><span class="sxs-lookup"><span data-stu-id="8fba6-103">Update event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fba6-104">Обновление свойств объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="8fba6-104">Update the properties of the [event](../resources/event.md) object.</span></span>

<span data-ttu-id="8fba6-105">При обновлении часового пояса времени начала или окончания события сначала [найдите поддерживаемые Часовые пояса](outlookuser-supportedtimezones.md) , чтобы убедиться, что настроены только Часовые пояса, настроенные для сервера почтовых ящиков пользователя.</span><span class="sxs-lookup"><span data-stu-id="8fba6-105">When updating the time zone of the start or end time of an event, first [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8fba6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8fba6-106">Permissions</span></span>
<span data-ttu-id="8fba6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fba6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fba6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fba6-109">Permission type</span></span>      | <span data-ttu-id="8fba6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fba6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fba6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fba6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8fba6-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8fba6-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8fba6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fba6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fba6-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8fba6-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8fba6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8fba6-115">Application</span></span> | <span data-ttu-id="8fba6-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8fba6-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8fba6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fba6-117">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="8fba6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8fba6-118">Request headers</span></span>
| <span data-ttu-id="8fba6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8fba6-119">Name</span></span>       | <span data-ttu-id="8fba6-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8fba6-120">Type</span></span> | <span data-ttu-id="8fba6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8fba6-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8fba6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fba6-122">Authorization</span></span>  | <span data-ttu-id="8fba6-123">string</span><span class="sxs-lookup"><span data-stu-id="8fba6-123">string</span></span>  | <span data-ttu-id="8fba6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fba6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8fba6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8fba6-126">Request body</span></span>
<span data-ttu-id="8fba6-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8fba6-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8fba6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8fba6-130">Property</span></span>       | <span data-ttu-id="8fba6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8fba6-131">Type</span></span>    | <span data-ttu-id="8fba6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8fba6-132">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="8fba6-133">attendees</span><span class="sxs-lookup"><span data-stu-id="8fba6-133">attendees</span></span>|<span data-ttu-id="8fba6-134">Attendee</span><span class="sxs-lookup"><span data-stu-id="8fba6-134">Attendee</span></span>|<span data-ttu-id="8fba6-135">Коллекция участников события.</span><span class="sxs-lookup"><span data-stu-id="8fba6-135">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="8fba6-136">body</span><span class="sxs-lookup"><span data-stu-id="8fba6-136">body</span></span>|<span data-ttu-id="8fba6-137">ItemBody</span><span class="sxs-lookup"><span data-stu-id="8fba6-137">ItemBody</span></span>|<span data-ttu-id="8fba6-138">Текст сообщения, связанного с событием.</span><span class="sxs-lookup"><span data-stu-id="8fba6-138">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="8fba6-139">categories</span><span class="sxs-lookup"><span data-stu-id="8fba6-139">categories</span></span>|<span data-ttu-id="8fba6-140">String</span><span class="sxs-lookup"><span data-stu-id="8fba6-140">String</span></span>|<span data-ttu-id="8fba6-141">Категории, связанные с событием.</span><span class="sxs-lookup"><span data-stu-id="8fba6-141">The categories associated with the event.</span></span>|
| <span data-ttu-id="8fba6-142">end</span><span class="sxs-lookup"><span data-stu-id="8fba6-142">end</span></span>|<span data-ttu-id="8fba6-143">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8fba6-143">DateTimeTimeZone</span></span>|<span data-ttu-id="8fba6-144">Дата, время и часовой пояс завершения события.</span><span class="sxs-lookup"><span data-stu-id="8fba6-144">The date, time, and time zone that the event ends.</span></span> |
| <span data-ttu-id="8fba6-145">importance</span><span class="sxs-lookup"><span data-stu-id="8fba6-145">importance</span></span>|<span data-ttu-id="8fba6-146">String</span><span class="sxs-lookup"><span data-stu-id="8fba6-146">String</span></span>|<span data-ttu-id="8fba6-147">Важность события.</span><span class="sxs-lookup"><span data-stu-id="8fba6-147">The importance of the event.</span></span> <span data-ttu-id="8fba6-148">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="8fba6-148">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="8fba6-149">isAllDay</span><span class="sxs-lookup"><span data-stu-id="8fba6-149">isAllDay</span></span>|<span data-ttu-id="8fba6-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fba6-150">Boolean</span></span>|<span data-ttu-id="8fba6-151">Задайте значение true, если событие длится весь день.</span><span class="sxs-lookup"><span data-stu-id="8fba6-151">Set to true if the event lasts all day.</span></span>|
| <span data-ttu-id="8fba6-152">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="8fba6-152">isReminderOn</span></span>|<span data-ttu-id="8fba6-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fba6-153">Boolean</span></span>|<span data-ttu-id="8fba6-154">Задайте значение true, если установлено напоминание пользователю о событии.</span><span class="sxs-lookup"><span data-stu-id="8fba6-154">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="8fba6-155">location</span><span class="sxs-lookup"><span data-stu-id="8fba6-155">location</span></span>|<span data-ttu-id="8fba6-156">Расположение</span><span class="sxs-lookup"><span data-stu-id="8fba6-156">Location</span></span>|<span data-ttu-id="8fba6-157">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="8fba6-157">The location of the event.</span></span>|
|<span data-ttu-id="8fba6-158">locations</span><span class="sxs-lookup"><span data-stu-id="8fba6-158">locations</span></span>|<span data-ttu-id="8fba6-159">Коллекция [Location](../resources/location.md)</span><span class="sxs-lookup"><span data-stu-id="8fba6-159">[Location](../resources/location.md) collection</span></span>|<span data-ttu-id="8fba6-160">Места проведения события или участия в нем.</span><span class="sxs-lookup"><span data-stu-id="8fba6-160">The locations where the event is held or attended from.</span></span> <span data-ttu-id="8fba6-161">Свойства **location** и **locations** всегда совпадают друг с другом.</span><span class="sxs-lookup"><span data-stu-id="8fba6-161">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="8fba6-162">Если вы обновите свойство **location**, предыдущие места в коллекции **locations** будут удалены и заменены новым значением **location**.</span><span class="sxs-lookup"><span data-stu-id="8fba6-162">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
| <span data-ttu-id="8fba6-163">recurrence</span><span class="sxs-lookup"><span data-stu-id="8fba6-163">recurrence</span></span>|<span data-ttu-id="8fba6-164">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="8fba6-164">PatternedRecurrence</span></span>|<span data-ttu-id="8fba6-165">Расписание повторения события.</span><span class="sxs-lookup"><span data-stu-id="8fba6-165">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="8fba6-166">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="8fba6-166">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="8fba6-167">Int32</span><span class="sxs-lookup"><span data-stu-id="8fba6-167">Int32</span></span>|<span data-ttu-id="8fba6-168">Позволяет указать, за сколько минут до начала события появляется напоминание.</span><span class="sxs-lookup"><span data-stu-id="8fba6-168">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="8fba6-169">responseRequested</span><span class="sxs-lookup"><span data-stu-id="8fba6-169">responseRequested</span></span>|<span data-ttu-id="8fba6-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fba6-170">Boolean</span></span>|<span data-ttu-id="8fba6-171">Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения.</span><span class="sxs-lookup"><span data-stu-id="8fba6-171">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="8fba6-172">sensitivity</span><span class="sxs-lookup"><span data-stu-id="8fba6-172">sensitivity</span></span>|<span data-ttu-id="8fba6-173">String</span><span class="sxs-lookup"><span data-stu-id="8fba6-173">String</span></span>| <span data-ttu-id="8fba6-174">Возможные значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="8fba6-174">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="8fba6-175">showAs</span><span class="sxs-lookup"><span data-stu-id="8fba6-175">showAs</span></span>|<span data-ttu-id="8fba6-176">String</span><span class="sxs-lookup"><span data-stu-id="8fba6-176">String</span></span>|<span data-ttu-id="8fba6-177">Отображаемое состояние.</span><span class="sxs-lookup"><span data-stu-id="8fba6-177">The status to show.</span></span> <span data-ttu-id="8fba6-178">Возможные `free` значения:, `tentative`, `busy`, `oof`, `workingElsewhere`,. `unknown`</span><span class="sxs-lookup"><span data-stu-id="8fba6-178">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="8fba6-179">начать</span><span class="sxs-lookup"><span data-stu-id="8fba6-179">start</span></span>|<span data-ttu-id="8fba6-180">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8fba6-180">DateTimeTimeZone</span></span>|<span data-ttu-id="8fba6-181">Дата и время начала, время и часовой пояс события.</span><span class="sxs-lookup"><span data-stu-id="8fba6-181">The start date, time, and time zone of the event.</span></span> |
| <span data-ttu-id="8fba6-182">subject</span><span class="sxs-lookup"><span data-stu-id="8fba6-182">subject</span></span>|<span data-ttu-id="8fba6-183">String</span><span class="sxs-lookup"><span data-stu-id="8fba6-183">String</span></span>|<span data-ttu-id="8fba6-184">Текст в строке темы сообщения о событии.</span><span class="sxs-lookup"><span data-stu-id="8fba6-184">The text of the event's subject line.</span></span>|

<span data-ttu-id="8fba6-185">Так как ресурс **event** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **event**.</span><span class="sxs-lookup"><span data-stu-id="8fba6-185">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="8fba6-186">Если обновляемый ресурс **event** является главным событием повторяющегося ряда, содержит несколько участников и экземпляры, обновленные отдельно, отправляется несколько сообщений электронной почты с уведомлениями: одно для главного ряда и по одному для каждого обновленного экземпляра.</span><span class="sxs-lookup"><span data-stu-id="8fba6-186">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="8fba6-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fba6-187">Response</span></span>

<span data-ttu-id="8fba6-188">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8fba6-188">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="8fba6-189">**Примечание.** Этот метод может вернуть отклик "HTTP 400 — ошибочный запрос" с кодом ошибки `ErrorOccurrenceCrossingBoundary` и следующим сообщением об ошибке: "Измененная копия пересекается со смежной копией или перекрывает ее".</span><span class="sxs-lookup"><span data-stu-id="8fba6-189">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="8fba6-190">Это означает, что обновление нарушает следующее ограничение Outlook для повторяющихся исключений: повторение нельзя перемещать на день предыдущего повторения или до него, а также на день следующего повторения или после него.</span><span class="sxs-lookup"><span data-stu-id="8fba6-190">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="8fba6-191">Пример</span><span class="sxs-lookup"><span data-stu-id="8fba6-191">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8fba6-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fba6-192">Request</span></span>

<span data-ttu-id="8fba6-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8fba6-193">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8fba6-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="8fba6-194">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8fba6-195">C#</span><span class="sxs-lookup"><span data-stu-id="8fba6-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8fba6-196">Javascript</span><span class="sxs-lookup"><span data-stu-id="8fba6-196">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8fba6-197">Ответ</span><span class="sxs-lookup"><span data-stu-id="8fba6-197">Response</span></span>
<span data-ttu-id="8fba6-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8fba6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="8fba6-201">См. также</span><span class="sxs-lookup"><span data-stu-id="8fba6-201">See also</span></span>

- [<span data-ttu-id="8fba6-202">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="8fba6-202">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="8fba6-203">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="8fba6-203">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="8fba6-204">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="8fba6-204">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
