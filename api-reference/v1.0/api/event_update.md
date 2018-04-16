# <a name="update-event"></a><span data-ttu-id="a608d-101">Обновление события</span><span class="sxs-lookup"><span data-stu-id="a608d-101">Update event</span></span>

<span data-ttu-id="a608d-102">Обновление свойств, принадлежащих объекту события.</span><span class="sxs-lookup"><span data-stu-id="a608d-102">Update the properties of event object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a608d-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a608d-103">Permissions</span></span>
<span data-ttu-id="a608d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a608d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a608d-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a608d-106">Permission type</span></span>      | <span data-ttu-id="a608d-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a608d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a608d-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a608d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a608d-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a608d-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a608d-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a608d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a608d-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a608d-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a608d-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a608d-112">Application</span></span> | <span data-ttu-id="a608d-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a608d-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a608d-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a608d-114">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="a608d-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a608d-115">Request headers</span></span>
| <span data-ttu-id="a608d-116">Имя</span><span class="sxs-lookup"><span data-stu-id="a608d-116">Name</span></span>       | <span data-ttu-id="a608d-117">Тип</span><span class="sxs-lookup"><span data-stu-id="a608d-117">Type</span></span> | <span data-ttu-id="a608d-118">Описание</span><span class="sxs-lookup"><span data-stu-id="a608d-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a608d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a608d-119">Authorization</span></span>  | <span data-ttu-id="a608d-120">string</span><span class="sxs-lookup"><span data-stu-id="a608d-120">string</span></span>  | <span data-ttu-id="a608d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a608d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a608d-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a608d-123">Request body</span></span>
<span data-ttu-id="a608d-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a608d-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a608d-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="a608d-127">Property</span></span>     | <span data-ttu-id="a608d-128">Тип</span><span class="sxs-lookup"><span data-stu-id="a608d-128">Type</span></span>   |<span data-ttu-id="a608d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="a608d-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a608d-130">attendees</span><span class="sxs-lookup"><span data-stu-id="a608d-130">attendees</span></span>|[<span data-ttu-id="a608d-131">Attendee</span><span class="sxs-lookup"><span data-stu-id="a608d-131">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="a608d-132">Коллекция участников события.</span><span class="sxs-lookup"><span data-stu-id="a608d-132">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="a608d-133">body</span><span class="sxs-lookup"><span data-stu-id="a608d-133">body</span></span>|[<span data-ttu-id="a608d-134">ItemBody</span><span class="sxs-lookup"><span data-stu-id="a608d-134">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="a608d-135">Текст сообщения, связанного с событием.</span><span class="sxs-lookup"><span data-stu-id="a608d-135">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="a608d-136">categories</span><span class="sxs-lookup"><span data-stu-id="a608d-136">categories</span></span>|<span data-ttu-id="a608d-137">String</span><span class="sxs-lookup"><span data-stu-id="a608d-137">String</span></span>|<span data-ttu-id="a608d-138">Категории, связанные с событием.</span><span class="sxs-lookup"><span data-stu-id="a608d-138">The categories associated with the event.</span></span>|
|<span data-ttu-id="a608d-139">end</span><span class="sxs-lookup"><span data-stu-id="a608d-139">end</span></span>|[<span data-ttu-id="a608d-140">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a608d-140">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="a608d-141">Дата и время завершения события.</span><span class="sxs-lookup"><span data-stu-id="a608d-141">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="a608d-p104">По умолчанию время завершения указано в формате UTC. Можно дополнительно указать часовой пояс в элементе EndTimeZone, задать время завершения согласно этому часовому поясу и UTC-смещение. Обратите внимание, что если вы используете EndTimeZone, следует также указать значение StartTimeZone.</span><span class="sxs-lookup"><span data-stu-id="a608d-p104">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="a608d-145">Пример указания даты (25 февраля 2015 г., 21:34 по тихоокеанскому поясному времени): "2015-02-25T21:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="a608d-145">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
|<span data-ttu-id="a608d-146">importance</span><span class="sxs-lookup"><span data-stu-id="a608d-146">importance</span></span>|<span data-ttu-id="a608d-147">String</span><span class="sxs-lookup"><span data-stu-id="a608d-147">String</span></span>|<span data-ttu-id="a608d-148">Важность события.</span><span class="sxs-lookup"><span data-stu-id="a608d-148">The importance of the event.</span></span> <span data-ttu-id="a608d-149">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="a608d-149">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="a608d-150">isAllDay</span><span class="sxs-lookup"><span data-stu-id="a608d-150">isAllDay</span></span>|<span data-ttu-id="a608d-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="a608d-151">Boolean</span></span>|<span data-ttu-id="a608d-152">Задайте значение true, если событие длится весь день.</span><span class="sxs-lookup"><span data-stu-id="a608d-152">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="a608d-153">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="a608d-153">isReminderOn</span></span>|<span data-ttu-id="a608d-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="a608d-154">Boolean</span></span>|<span data-ttu-id="a608d-155">Задайте значение true, если установлено напоминание пользователю о событии.</span><span class="sxs-lookup"><span data-stu-id="a608d-155">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="a608d-156">location</span><span class="sxs-lookup"><span data-stu-id="a608d-156">location</span></span>|[<span data-ttu-id="a608d-157">Location</span><span class="sxs-lookup"><span data-stu-id="a608d-157">Location</span></span>](../resources/location.md)|<span data-ttu-id="a608d-158">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="a608d-158">The location of the event.</span></span>|
|<span data-ttu-id="a608d-159">locations</span><span class="sxs-lookup"><span data-stu-id="a608d-159">locations</span></span>|<span data-ttu-id="a608d-160">Коллекция [location](../resources/location.md)</span><span class="sxs-lookup"><span data-stu-id="a608d-160">[location](../resources/location.md) collection</span></span>|<span data-ttu-id="a608d-161">Места проведения мероприятия или участия в нем.</span><span class="sxs-lookup"><span data-stu-id="a608d-161">The locations where the event is held or attended from.</span></span> <span data-ttu-id="a608d-162">Свойства **location** и **locations** всегда совпадают друг с другом.</span><span class="sxs-lookup"><span data-stu-id="a608d-162">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="a608d-163">Если вы обновите свойство **location**, предыдущие места в коллекции **locations** будут удалены и заменены новым значением **location**.</span><span class="sxs-lookup"><span data-stu-id="a608d-163">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="a608d-164">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="a608d-164">onlineMeetingUrl</span></span>|<span data-ttu-id="a608d-165">String</span><span class="sxs-lookup"><span data-stu-id="a608d-165">String</span></span>|<span data-ttu-id="a608d-166">URL-адрес для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="a608d-166">A URL for an online meeting.</span></span>|
|<span data-ttu-id="a608d-167">recurrence</span><span class="sxs-lookup"><span data-stu-id="a608d-167">recurrence</span></span>|[<span data-ttu-id="a608d-168">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="a608d-168">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="a608d-169">Расписание повторения события.</span><span class="sxs-lookup"><span data-stu-id="a608d-169">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="a608d-170">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="a608d-170">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="a608d-171">Int32</span><span class="sxs-lookup"><span data-stu-id="a608d-171">Int32</span></span>|<span data-ttu-id="a608d-172">Позволяет указать, за сколько минут до начала события появляется напоминание.</span><span class="sxs-lookup"><span data-stu-id="a608d-172">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="a608d-173">responseRequested</span><span class="sxs-lookup"><span data-stu-id="a608d-173">responseRequested</span></span>|<span data-ttu-id="a608d-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="a608d-174">Boolean</span></span>|<span data-ttu-id="a608d-175">Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения.</span><span class="sxs-lookup"><span data-stu-id="a608d-175">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="a608d-176">sensitivity</span><span class="sxs-lookup"><span data-stu-id="a608d-176">sensitivity</span></span>|<span data-ttu-id="a608d-177">String</span><span class="sxs-lookup"><span data-stu-id="a608d-177">String</span></span>| <span data-ttu-id="a608d-178">Возможные значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="a608d-178">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="a608d-179">showAs</span><span class="sxs-lookup"><span data-stu-id="a608d-179">showAs</span></span>|<span data-ttu-id="a608d-180">String</span><span class="sxs-lookup"><span data-stu-id="a608d-180">String</span></span>|<span data-ttu-id="a608d-181">Отображаемое состояние.</span><span class="sxs-lookup"><span data-stu-id="a608d-181">The status to show.</span></span> <span data-ttu-id="a608d-182">Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a608d-182">Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="a608d-183">start</span><span class="sxs-lookup"><span data-stu-id="a608d-183">start</span></span>|[<span data-ttu-id="a608d-184">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a608d-184">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="a608d-185">Время начала события.</span><span class="sxs-lookup"><span data-stu-id="a608d-185">The start time of the event.</span></span> <br/><br/><span data-ttu-id="a608d-p108">По умолчанию время начала указано в формате UTC. Можно дополнительно указать часовой пояс в элементе StartTimeZone, задать время завершения согласно этому часовому поясу и UTC-смещение. Обратите внимание, что если вы используете StartTimeZone, следует также указать значение EndTimeZone.</span><span class="sxs-lookup"><span data-stu-id="a608d-p108">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="a608d-189">Пример указания даты (25 февраля 2015 г., 19:34 по тихоокеанскому поясному времени): "2015-02-25T19:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="a608d-189">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
|<span data-ttu-id="a608d-190">subject</span><span class="sxs-lookup"><span data-stu-id="a608d-190">subject</span></span>|<span data-ttu-id="a608d-191">String</span><span class="sxs-lookup"><span data-stu-id="a608d-191">String</span></span>|<span data-ttu-id="a608d-192">Текст в строке темы сообщения о событии.</span><span class="sxs-lookup"><span data-stu-id="a608d-192">The text of the event's subject line.</span></span>|

<span data-ttu-id="a608d-193">Так как ресурс **event** поддерживает [расширения](../../../concepts/extensibility_overview.md), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **event**.</span><span class="sxs-lookup"><span data-stu-id="a608d-193">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

## <a name="response"></a><span data-ttu-id="a608d-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="a608d-194">Response</span></span>

<span data-ttu-id="a608d-195">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a608d-195">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a608d-196">Пример</span><span class="sxs-lookup"><span data-stu-id="a608d-196">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a608d-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="a608d-197">Request</span></span>

<span data-ttu-id="a608d-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a608d-198">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a608d-199">Ответ</span><span class="sxs-lookup"><span data-stu-id="a608d-199">Response</span></span>

<span data-ttu-id="a608d-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a608d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="a608d-203">См. также</span><span class="sxs-lookup"><span data-stu-id="a608d-203">See also</span></span>

- [<span data-ttu-id="a608d-204">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="a608d-204">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="a608d-205">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="a608d-205">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="a608d-206">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="a608d-206">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
