---
title: Обновление события
description: Обновление свойства объекта события.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 50711c6e2533f7a99e742542b1376faf78fff8e9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956579"
---
# <a name="update-event"></a><span data-ttu-id="ce1c9-103">Обновление события</span><span class="sxs-lookup"><span data-stu-id="ce1c9-103">Update event</span></span>

> <span data-ttu-id="ce1c9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce1c9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ce1c9-106">Обновление свойства объекта [события](../resources/event.md) .</span><span class="sxs-lookup"><span data-stu-id="ce1c9-106">Update the properties of the [event](../resources/event.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ce1c9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce1c9-107">Permissions</span></span>
<span data-ttu-id="ce1c9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce1c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce1c9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce1c9-110">Permission type</span></span>      | <span data-ttu-id="ce1c9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce1c9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce1c9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce1c9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ce1c9-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce1c9-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ce1c9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce1c9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce1c9-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce1c9-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ce1c9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce1c9-116">Application</span></span> | <span data-ttu-id="ce1c9-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce1c9-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce1c9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce1c9-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="ce1c9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce1c9-119">Request headers</span></span>
| <span data-ttu-id="ce1c9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ce1c9-120">Name</span></span>       | <span data-ttu-id="ce1c9-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ce1c9-121">Type</span></span> | <span data-ttu-id="ce1c9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ce1c9-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ce1c9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce1c9-123">Authorization</span></span>  | <span data-ttu-id="ce1c9-124">string</span><span class="sxs-lookup"><span data-stu-id="ce1c9-124">string</span></span>  | <span data-ttu-id="ce1c9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce1c9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ce1c9-127">Request body</span></span>
<span data-ttu-id="ce1c9-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ce1c9-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce1c9-131">Property</span></span>       | <span data-ttu-id="ce1c9-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ce1c9-132">Type</span></span>    | <span data-ttu-id="ce1c9-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ce1c9-133">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="ce1c9-134">attendees</span><span class="sxs-lookup"><span data-stu-id="ce1c9-134">attendees</span></span>|<span data-ttu-id="ce1c9-135">Attendee</span><span class="sxs-lookup"><span data-stu-id="ce1c9-135">Attendee</span></span>|<span data-ttu-id="ce1c9-136">Коллекция участников события.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-136">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="ce1c9-137">Основной текст</span><span class="sxs-lookup"><span data-stu-id="ce1c9-137">body</span></span>|<span data-ttu-id="ce1c9-138">ItemBody</span><span class="sxs-lookup"><span data-stu-id="ce1c9-138">ItemBody</span></span>|<span data-ttu-id="ce1c9-139">Текст сообщения, связанного с событием.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-139">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="ce1c9-140">categories</span><span class="sxs-lookup"><span data-stu-id="ce1c9-140">categories</span></span>|<span data-ttu-id="ce1c9-141">String</span><span class="sxs-lookup"><span data-stu-id="ce1c9-141">String</span></span>|<span data-ttu-id="ce1c9-142">Категории, связанные с событием.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-142">The categories associated with the event.</span></span>|
| <span data-ttu-id="ce1c9-143">end</span><span class="sxs-lookup"><span data-stu-id="ce1c9-143">end</span></span>|<span data-ttu-id="ce1c9-144">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ce1c9-144">DateTimeTimeZone</span></span>|<span data-ttu-id="ce1c9-145">Дата и время завершения события.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-145">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="ce1c9-p105">По умолчанию время завершения указано в формате UTC. Можно дополнительно указать часовой пояс в элементе EndTimeZone, задать время завершения согласно этому часовому поясу и UTC-смещение. Обратите внимание, что если вы используете EndTimeZone, следует также указать значение StartTimeZone.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-p105">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="ce1c9-149">Пример указания даты (25 февраля 2015 г., 21:34 по тихоокеанскому поясному времени): "2015-02-25T21:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="ce1c9-149">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
| <span data-ttu-id="ce1c9-150">importance</span><span class="sxs-lookup"><span data-stu-id="ce1c9-150">importance</span></span>|<span data-ttu-id="ce1c9-151">String</span><span class="sxs-lookup"><span data-stu-id="ce1c9-151">String</span></span>|<span data-ttu-id="ce1c9-152">Важность события.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-152">The importance of the event.</span></span> <span data-ttu-id="ce1c9-153">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-153">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="ce1c9-154">isAllDay</span><span class="sxs-lookup"><span data-stu-id="ce1c9-154">isAllDay</span></span>|<span data-ttu-id="ce1c9-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce1c9-155">Boolean</span></span>|<span data-ttu-id="ce1c9-156">Задайте значение true, если событие длится весь день.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-156">Set to true if the event lasts all day.</span></span>|
| <span data-ttu-id="ce1c9-157">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="ce1c9-157">isReminderOn</span></span>|<span data-ttu-id="ce1c9-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce1c9-158">Boolean</span></span>|<span data-ttu-id="ce1c9-159">Задайте значение true, если установлено напоминание пользователю о событии.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-159">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="ce1c9-160">location</span><span class="sxs-lookup"><span data-stu-id="ce1c9-160">location</span></span>|<span data-ttu-id="ce1c9-161">Location</span><span class="sxs-lookup"><span data-stu-id="ce1c9-161">Location</span></span>|<span data-ttu-id="ce1c9-162">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-162">The location of the event.</span></span>|
|<span data-ttu-id="ce1c9-163">locations</span><span class="sxs-lookup"><span data-stu-id="ce1c9-163">locations</span></span>|<span data-ttu-id="ce1c9-164">[Расположение](../resources/location.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="ce1c9-164">[Location](../resources/location.md) collection</span></span>|<span data-ttu-id="ce1c9-165">Места проведения мероприятия или участия в нем.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-165">The locations where the event is held or attended from.</span></span> <span data-ttu-id="ce1c9-166">Свойства **location** и **locations** всегда совпадают друг с другом.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-166">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="ce1c9-167">Если вы обновите свойство **location**, предыдущие места в коллекции **locations** будут удалены и заменены новым значением **location**.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-167">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
| <span data-ttu-id="ce1c9-168">recurrence</span><span class="sxs-lookup"><span data-stu-id="ce1c9-168">recurrence</span></span>|<span data-ttu-id="ce1c9-169">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="ce1c9-169">PatternedRecurrence</span></span>|<span data-ttu-id="ce1c9-170">Расписание повторения события.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-170">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="ce1c9-171">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="ce1c9-171">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="ce1c9-172">Int32</span><span class="sxs-lookup"><span data-stu-id="ce1c9-172">Int32</span></span>|<span data-ttu-id="ce1c9-173">Позволяет указать, за сколько минут до начала события появляется напоминание.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-173">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="ce1c9-174">responseRequested</span><span class="sxs-lookup"><span data-stu-id="ce1c9-174">responseRequested</span></span>|<span data-ttu-id="ce1c9-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce1c9-175">Boolean</span></span>|<span data-ttu-id="ce1c9-176">Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-176">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="ce1c9-177">sensitivity</span><span class="sxs-lookup"><span data-stu-id="ce1c9-177">sensitivity</span></span>|<span data-ttu-id="ce1c9-178">String</span><span class="sxs-lookup"><span data-stu-id="ce1c9-178">String</span></span>| <span data-ttu-id="ce1c9-179">Возможные значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-179">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="ce1c9-180">showAs</span><span class="sxs-lookup"><span data-stu-id="ce1c9-180">showAs</span></span>|<span data-ttu-id="ce1c9-181">String</span><span class="sxs-lookup"><span data-stu-id="ce1c9-181">String</span></span>|<span data-ttu-id="ce1c9-182">Отображаемое состояние.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-182">The status to show.</span></span> <span data-ttu-id="ce1c9-183">Возможные значения: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-183">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="ce1c9-184">start</span><span class="sxs-lookup"><span data-stu-id="ce1c9-184">start</span></span>|<span data-ttu-id="ce1c9-185">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ce1c9-185">DateTimeTimeZone</span></span>|<span data-ttu-id="ce1c9-186">Время начала события.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-186">The start time of the event.</span></span> <br/><br/><span data-ttu-id="ce1c9-p109">По умолчанию время начала указано в формате UTC. Можно дополнительно указать часовой пояс в элементе StartTimeZone, задать время завершения согласно этому часовому поясу и UTC-смещение. Обратите внимание, что если вы используете StartTimeZone, следует также указать значение EndTimeZone.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-p109">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="ce1c9-190">Пример указания даты (25 февраля 2015 г., 19:34 по тихоокеанскому поясному времени): "2015-02-25T19:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="ce1c9-190">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
| <span data-ttu-id="ce1c9-191">subject</span><span class="sxs-lookup"><span data-stu-id="ce1c9-191">subject</span></span>|<span data-ttu-id="ce1c9-192">String</span><span class="sxs-lookup"><span data-stu-id="ce1c9-192">String</span></span>|<span data-ttu-id="ce1c9-193">Текст в строке темы сообщения о событии.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-193">The text of the event's subject line.</span></span>|

<span data-ttu-id="ce1c9-194">Так как ресурс **событие** поддерживает [расширений](/graph/extensibility-overview), можно использовать `PATCH` операции для добавления, обновления или удаления данных конкретного приложения в настраиваемых свойств расширения в существующий экземпляр **события** .</span><span class="sxs-lookup"><span data-stu-id="ce1c9-194">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="ce1c9-195">Если **события** , для обновления — главной встречи, содержащий несколько участников и экземпляры, которые были обновлены отдельно, несколько уведомлений по электронной почте будут отправлены: один для главной серии и один для каждого экземпляра, который имеет были обновлены.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-195">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="ce1c9-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce1c9-196">Response</span></span>

<span data-ttu-id="ce1c9-197">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-197">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="ce1c9-198">**Примечание:** Этот метод может вернуть ответ HTTP 400 Bad Request с кодом ошибки из `ErrorOccurrenceCrossingBoundary` и следующее сообщение об ошибке: пересечение или перекрывающиеся рядом с вхождение измененная копия.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-198">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="ce1c9-199">Это указывает на то, что обновление нарушает следующие ограничения Outlook для повторяющихся исключений: вхождения или до день предыдущего события, нельзя перемещать и нельзя перемещать или после день следующие вхождение.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-199">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="ce1c9-200">Пример</span><span class="sxs-lookup"><span data-stu-id="ce1c9-200">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ce1c9-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce1c9-201">Request</span></span>

<span data-ttu-id="ce1c9-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-202">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ce1c9-203">Ответ</span><span class="sxs-lookup"><span data-stu-id="ce1c9-203">Response</span></span>
<span data-ttu-id="ce1c9-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ce1c9-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="ce1c9-207">См. также</span><span class="sxs-lookup"><span data-stu-id="ce1c9-207">See also</span></span>

- [<span data-ttu-id="ce1c9-208">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="ce1c9-208">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ce1c9-209">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="ce1c9-209">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="ce1c9-210">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="ce1c9-210">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
