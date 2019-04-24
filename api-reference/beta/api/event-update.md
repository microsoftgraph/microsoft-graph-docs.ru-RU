---
title: Обновление события
description: Обновление свойств объекта Event.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b3f101c14a69c6dc2b3687e9d4a1509e6ac7a531
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464036"
---
# <a name="update-event"></a><span data-ttu-id="f194b-103">Обновление события</span><span class="sxs-lookup"><span data-stu-id="f194b-103">Update event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f194b-104">Обновление свойств объекта [event](../resources/event.md) .</span><span class="sxs-lookup"><span data-stu-id="f194b-104">Update the properties of the [event](../resources/event.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f194b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f194b-105">Permissions</span></span>
<span data-ttu-id="f194b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f194b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f194b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f194b-108">Permission type</span></span>      | <span data-ttu-id="f194b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f194b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f194b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f194b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f194b-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f194b-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f194b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f194b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f194b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f194b-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f194b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f194b-114">Application</span></span> | <span data-ttu-id="f194b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f194b-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f194b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f194b-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="f194b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f194b-117">Request headers</span></span>
| <span data-ttu-id="f194b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f194b-118">Name</span></span>       | <span data-ttu-id="f194b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f194b-119">Type</span></span> | <span data-ttu-id="f194b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f194b-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f194b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f194b-121">Authorization</span></span>  | <span data-ttu-id="f194b-122">string</span><span class="sxs-lookup"><span data-stu-id="f194b-122">string</span></span>  | <span data-ttu-id="f194b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f194b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f194b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f194b-125">Request body</span></span>
<span data-ttu-id="f194b-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f194b-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f194b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f194b-129">Property</span></span>       | <span data-ttu-id="f194b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f194b-130">Type</span></span>    | <span data-ttu-id="f194b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f194b-131">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="f194b-132">attendees</span><span class="sxs-lookup"><span data-stu-id="f194b-132">attendees</span></span>|<span data-ttu-id="f194b-133">Участник</span><span class="sxs-lookup"><span data-stu-id="f194b-133">Attendee</span></span>|<span data-ttu-id="f194b-134">Коллекция участников события.</span><span class="sxs-lookup"><span data-stu-id="f194b-134">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="f194b-135">body</span><span class="sxs-lookup"><span data-stu-id="f194b-135">body</span></span>|<span data-ttu-id="f194b-136">ItemBody</span><span class="sxs-lookup"><span data-stu-id="f194b-136">ItemBody</span></span>|<span data-ttu-id="f194b-137">Текст сообщения, связанного с событием.</span><span class="sxs-lookup"><span data-stu-id="f194b-137">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="f194b-138">categories</span><span class="sxs-lookup"><span data-stu-id="f194b-138">categories</span></span>|<span data-ttu-id="f194b-139">String</span><span class="sxs-lookup"><span data-stu-id="f194b-139">String</span></span>|<span data-ttu-id="f194b-140">Категории, связанные с событием.</span><span class="sxs-lookup"><span data-stu-id="f194b-140">The categories associated with the event.</span></span>|
| <span data-ttu-id="f194b-141">end</span><span class="sxs-lookup"><span data-stu-id="f194b-141">end</span></span>|<span data-ttu-id="f194b-142">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f194b-142">DateTimeTimeZone</span></span>|<span data-ttu-id="f194b-143">Дата и время завершения события.</span><span class="sxs-lookup"><span data-stu-id="f194b-143">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="f194b-p104">По умолчанию время завершения указано в формате UTC. Можно дополнительно указать часовой пояс в элементе EndTimeZone, задать время завершения согласно этому часовому поясу и UTC-смещение. Обратите внимание, что если вы используете EndTimeZone, следует также указать значение StartTimeZone.</span><span class="sxs-lookup"><span data-stu-id="f194b-p104">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="f194b-147">Пример указания даты (25 февраля 2015 г., 21:34 по тихоокеанскому поясному времени): "2015-02-25T21:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="f194b-147">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
| <span data-ttu-id="f194b-148">importance</span><span class="sxs-lookup"><span data-stu-id="f194b-148">importance</span></span>|<span data-ttu-id="f194b-149">String</span><span class="sxs-lookup"><span data-stu-id="f194b-149">String</span></span>|<span data-ttu-id="f194b-150">Важность события.</span><span class="sxs-lookup"><span data-stu-id="f194b-150">The importance of the event.</span></span> <span data-ttu-id="f194b-151">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="f194b-151">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="f194b-152">isAllDay</span><span class="sxs-lookup"><span data-stu-id="f194b-152">isAllDay</span></span>|<span data-ttu-id="f194b-153">Логический</span><span class="sxs-lookup"><span data-stu-id="f194b-153">Boolean</span></span>|<span data-ttu-id="f194b-154">Задайте значение true, если событие длится весь день.</span><span class="sxs-lookup"><span data-stu-id="f194b-154">Set to true if the event lasts all day.</span></span>|
| <span data-ttu-id="f194b-155">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="f194b-155">isReminderOn</span></span>|<span data-ttu-id="f194b-156">Логический</span><span class="sxs-lookup"><span data-stu-id="f194b-156">Boolean</span></span>|<span data-ttu-id="f194b-157">Задайте значение true, если установлено напоминание пользователю о событии.</span><span class="sxs-lookup"><span data-stu-id="f194b-157">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="f194b-158">location</span><span class="sxs-lookup"><span data-stu-id="f194b-158">location</span></span>|<span data-ttu-id="f194b-159">Расположение</span><span class="sxs-lookup"><span data-stu-id="f194b-159">Location</span></span>|<span data-ttu-id="f194b-160">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="f194b-160">The location of the event.</span></span>|
|<span data-ttu-id="f194b-161">locations</span><span class="sxs-lookup"><span data-stu-id="f194b-161">locations</span></span>|<span data-ttu-id="f194b-162">Коллекция [Location](../resources/location.md)</span><span class="sxs-lookup"><span data-stu-id="f194b-162">[Location](../resources/location.md) collection</span></span>|<span data-ttu-id="f194b-163">Места проведения события или участия в нем.</span><span class="sxs-lookup"><span data-stu-id="f194b-163">The locations where the event is held or attended from.</span></span> <span data-ttu-id="f194b-164">Свойства **location** и **locations** всегда совпадают друг с другом.</span><span class="sxs-lookup"><span data-stu-id="f194b-164">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="f194b-165">Если вы обновите свойство **location**, предыдущие места в коллекции **locations** будут удалены и заменены новым значением **location**.</span><span class="sxs-lookup"><span data-stu-id="f194b-165">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
| <span data-ttu-id="f194b-166">recurrence</span><span class="sxs-lookup"><span data-stu-id="f194b-166">recurrence</span></span>|<span data-ttu-id="f194b-167">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="f194b-167">PatternedRecurrence</span></span>|<span data-ttu-id="f194b-168">Расписание повторения события.</span><span class="sxs-lookup"><span data-stu-id="f194b-168">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="f194b-169">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="f194b-169">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="f194b-170">Int32</span><span class="sxs-lookup"><span data-stu-id="f194b-170">Int32</span></span>|<span data-ttu-id="f194b-171">Позволяет указать, за сколько минут до начала события появляется напоминание.</span><span class="sxs-lookup"><span data-stu-id="f194b-171">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="f194b-172">responseRequested</span><span class="sxs-lookup"><span data-stu-id="f194b-172">responseRequested</span></span>|<span data-ttu-id="f194b-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="f194b-173">Boolean</span></span>|<span data-ttu-id="f194b-174">Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения.</span><span class="sxs-lookup"><span data-stu-id="f194b-174">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="f194b-175">sensitivity</span><span class="sxs-lookup"><span data-stu-id="f194b-175">sensitivity</span></span>|<span data-ttu-id="f194b-176">String</span><span class="sxs-lookup"><span data-stu-id="f194b-176">String</span></span>| <span data-ttu-id="f194b-177">Возможные значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="f194b-177">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="f194b-178">showAs</span><span class="sxs-lookup"><span data-stu-id="f194b-178">showAs</span></span>|<span data-ttu-id="f194b-179">String</span><span class="sxs-lookup"><span data-stu-id="f194b-179">String</span></span>|<span data-ttu-id="f194b-180">Отображаемое состояние.</span><span class="sxs-lookup"><span data-stu-id="f194b-180">The status to show.</span></span> <span data-ttu-id="f194b-181">Возможные `free` значения:, `tentative`, `busy`, `oof`, `workingElsewhere`,. `unknown`</span><span class="sxs-lookup"><span data-stu-id="f194b-181">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="f194b-182">start</span><span class="sxs-lookup"><span data-stu-id="f194b-182">start</span></span>|<span data-ttu-id="f194b-183">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f194b-183">DateTimeTimeZone</span></span>|<span data-ttu-id="f194b-184">Время начала события.</span><span class="sxs-lookup"><span data-stu-id="f194b-184">The start time of the event.</span></span> <br/><br/><span data-ttu-id="f194b-p108">По умолчанию время начала указано в формате UTC. Можно дополнительно указать часовой пояс в элементе StartTimeZone, задать время завершения согласно этому часовому поясу и UTC-смещение. Обратите внимание, что если вы используете StartTimeZone, следует также указать значение EndTimeZone.</span><span class="sxs-lookup"><span data-stu-id="f194b-p108">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="f194b-188">Пример указания даты (25 февраля 2015 г., 19:34 по тихоокеанскому поясному времени): "2015-02-25T19:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="f194b-188">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
| <span data-ttu-id="f194b-189">subject</span><span class="sxs-lookup"><span data-stu-id="f194b-189">subject</span></span>|<span data-ttu-id="f194b-190">String</span><span class="sxs-lookup"><span data-stu-id="f194b-190">String</span></span>|<span data-ttu-id="f194b-191">Текст в строке темы события.</span><span class="sxs-lookup"><span data-stu-id="f194b-191">The text of the event's subject line.</span></span>|

<span data-ttu-id="f194b-192">Так как ресурс **event** поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, зависящие от приложения, в пользовательских свойствах расширения в существующем экземпляре **события** .</span><span class="sxs-lookup"><span data-stu-id="f194b-192">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="f194b-193">Если обновляемое **событие** является главным событием повторяющейся серии, содержит несколько участников и содержит экземпляры, которые были обновлены отдельно, будет отправлено несколько сообщений с уведомлениями: один для основных рядов и один для каждого экземпляра обновлены.</span><span class="sxs-lookup"><span data-stu-id="f194b-193">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="f194b-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="f194b-194">Response</span></span>

<span data-ttu-id="f194b-195">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f194b-195">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="f194b-196">**Примечание:** Этот метод может возвращать ответ на ошибочный запрос HTTP 400 с кодом ошибки `ErrorOccurrenceCrossingBoundary` и следующим сообщением об ошибке: "измененное вхождение" пересекает или перекрывает смежное вхождение.</span><span class="sxs-lookup"><span data-stu-id="f194b-196">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="f194b-197">Это указывает на то, что обновление нарушает следующее ограничение Outlook на количество исключений повторения: событие не может быть перемещено до или до дня предыдущего события и не может быть перемещено в следующий день или после него.</span><span class="sxs-lookup"><span data-stu-id="f194b-197">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="f194b-198">Пример</span><span class="sxs-lookup"><span data-stu-id="f194b-198">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f194b-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="f194b-199">Request</span></span>

<span data-ttu-id="f194b-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f194b-200">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f194b-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="f194b-201">Response</span></span>
<span data-ttu-id="f194b-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f194b-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="f194b-205">См. также</span><span class="sxs-lookup"><span data-stu-id="f194b-205">See also</span></span>

- [<span data-ttu-id="f194b-206">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="f194b-206">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f194b-207">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="f194b-207">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="f194b-208">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="f194b-208">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/event-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
