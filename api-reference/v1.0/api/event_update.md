# <a name="update-event"></a><span data-ttu-id="d7617-101">Обновление события</span><span class="sxs-lookup"><span data-stu-id="d7617-101">Update event</span></span>

<span data-ttu-id="d7617-102">Обновление свойств, принадлежащих объекту события.</span><span class="sxs-lookup"><span data-stu-id="d7617-102">Update the properties of event object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7617-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7617-103">Permissions</span></span>
<span data-ttu-id="d7617-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d7617-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d7617-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7617-106">Permission type</span></span>      | <span data-ttu-id="d7617-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7617-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7617-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7617-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d7617-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7617-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d7617-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7617-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7617-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7617-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d7617-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7617-112">Application</span></span> | <span data-ttu-id="d7617-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7617-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7617-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7617-114">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="d7617-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7617-115">Request headers</span></span>
| <span data-ttu-id="d7617-116">Имя</span><span class="sxs-lookup"><span data-stu-id="d7617-116">Name</span></span>       | <span data-ttu-id="d7617-117">Тип</span><span class="sxs-lookup"><span data-stu-id="d7617-117">Type</span></span> | <span data-ttu-id="d7617-118">Описание</span><span class="sxs-lookup"><span data-stu-id="d7617-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d7617-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7617-119">Authorization</span></span>  | <span data-ttu-id="d7617-120">string</span><span class="sxs-lookup"><span data-stu-id="d7617-120">string</span></span>  | <span data-ttu-id="d7617-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7617-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7617-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7617-123">Request body</span></span>
<span data-ttu-id="d7617-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d7617-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d7617-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7617-127">Property</span></span>     | <span data-ttu-id="d7617-128">Тип</span><span class="sxs-lookup"><span data-stu-id="d7617-128">Type</span></span>   |<span data-ttu-id="d7617-129">Описание</span><span class="sxs-lookup"><span data-stu-id="d7617-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7617-130">attendees</span><span class="sxs-lookup"><span data-stu-id="d7617-130">attendees</span></span>|[<span data-ttu-id="d7617-131">Attendee</span><span class="sxs-lookup"><span data-stu-id="d7617-131">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="d7617-132">Коллекция участников события.</span><span class="sxs-lookup"><span data-stu-id="d7617-132">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="d7617-133">body</span><span class="sxs-lookup"><span data-stu-id="d7617-133">body</span></span>|[<span data-ttu-id="d7617-134">ItemBody</span><span class="sxs-lookup"><span data-stu-id="d7617-134">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="d7617-135">Текст сообщения, связанного с событием.</span><span class="sxs-lookup"><span data-stu-id="d7617-135">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="d7617-136">categories</span><span class="sxs-lookup"><span data-stu-id="d7617-136">categories</span></span>|<span data-ttu-id="d7617-137">String</span><span class="sxs-lookup"><span data-stu-id="d7617-137">String</span></span>|<span data-ttu-id="d7617-138">Категории, связанные с событием.</span><span class="sxs-lookup"><span data-stu-id="d7617-138">The categories associated with the event.</span></span>|
|<span data-ttu-id="d7617-139">end</span><span class="sxs-lookup"><span data-stu-id="d7617-139">end</span></span>|[<span data-ttu-id="d7617-140">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d7617-140">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="d7617-141">Дата и время завершения события.</span><span class="sxs-lookup"><span data-stu-id="d7617-141">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="d7617-p104">По умолчанию время завершения указано в формате UTC. Можно дополнительно указать часовой пояс в элементе EndTimeZone, задать время завершения согласно этому часовому поясу и UTC-смещение. Обратите внимание, что если вы используете EndTimeZone, следует также указать значение StartTimeZone.</span><span class="sxs-lookup"><span data-stu-id="d7617-p104">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="d7617-145">Пример указания даты (25 февраля 2015 г., 21:34 по тихоокеанскому поясному времени): "2015-02-25T21:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="d7617-145">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
|<span data-ttu-id="d7617-146">importance</span><span class="sxs-lookup"><span data-stu-id="d7617-146">importance</span></span>|<span data-ttu-id="d7617-147">String</span><span class="sxs-lookup"><span data-stu-id="d7617-147">String</span></span>|<span data-ttu-id="d7617-p105">Важность события. Low = 0, Normal = 1, High = 2. Возможные значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="d7617-p105">The importance of the event: Low = 0, Normal = 1, High = 2. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="d7617-150">isAllDay</span><span class="sxs-lookup"><span data-stu-id="d7617-150">isAllDay</span></span>|<span data-ttu-id="d7617-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7617-151">Boolean</span></span>|<span data-ttu-id="d7617-152">Задайте значение true, если событие длится весь день.</span><span class="sxs-lookup"><span data-stu-id="d7617-152">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="d7617-153">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="d7617-153">isReminderOn</span></span>|<span data-ttu-id="d7617-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7617-154">Boolean</span></span>|<span data-ttu-id="d7617-155">Задайте значение true, если установлено напоминание пользователю о событии.</span><span class="sxs-lookup"><span data-stu-id="d7617-155">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="d7617-156">location</span><span class="sxs-lookup"><span data-stu-id="d7617-156">location</span></span>|[<span data-ttu-id="d7617-157">Location</span><span class="sxs-lookup"><span data-stu-id="d7617-157">Location</span></span>](../resources/location.md)|<span data-ttu-id="d7617-158">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="d7617-158">The location of the event.</span></span>|
|<span data-ttu-id="d7617-159">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="d7617-159">onlineMeetingUrl</span></span>|<span data-ttu-id="d7617-160">String</span><span class="sxs-lookup"><span data-stu-id="d7617-160">String</span></span>|<span data-ttu-id="d7617-161">URL-адрес для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="d7617-161">A URL for an online meeting.</span></span>|
|<span data-ttu-id="d7617-162">recurrence</span><span class="sxs-lookup"><span data-stu-id="d7617-162">recurrence</span></span>|[<span data-ttu-id="d7617-163">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="d7617-163">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="d7617-164">Расписание повторения события.</span><span class="sxs-lookup"><span data-stu-id="d7617-164">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="d7617-165">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="d7617-165">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="d7617-166">Int32</span><span class="sxs-lookup"><span data-stu-id="d7617-166">Int32</span></span>|<span data-ttu-id="d7617-167">Позволяет указать, за сколько минут до начала события появляется напоминание.</span><span class="sxs-lookup"><span data-stu-id="d7617-167">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="d7617-168">responseRequested</span><span class="sxs-lookup"><span data-stu-id="d7617-168">responseRequested</span></span>|<span data-ttu-id="d7617-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7617-169">Boolean</span></span>|<span data-ttu-id="d7617-170">Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения.</span><span class="sxs-lookup"><span data-stu-id="d7617-170">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="d7617-171">sensitivity</span><span class="sxs-lookup"><span data-stu-id="d7617-171">sensitivity</span></span>|<span data-ttu-id="d7617-172">String</span><span class="sxs-lookup"><span data-stu-id="d7617-172">String</span></span>| <span data-ttu-id="d7617-173">Возможные значения: `Normal`, `Personal`, `Private`, `Confidential`.</span><span class="sxs-lookup"><span data-stu-id="d7617-173">Possible values are: `Normal`, `Personal`, `Private`, `Confidential`.</span></span>|
|<span data-ttu-id="d7617-174">showAs</span><span class="sxs-lookup"><span data-stu-id="d7617-174">showAs</span></span>|<span data-ttu-id="d7617-175">String</span><span class="sxs-lookup"><span data-stu-id="d7617-175">String</span></span>|<span data-ttu-id="d7617-176">Отображаемое состояние.</span><span class="sxs-lookup"><span data-stu-id="d7617-176">The status to show.</span></span> <span data-ttu-id="d7617-177">Возможные значения: `Free`, `Tentative`, `Busy`, `Oof`, `WorkingElsewhere`, `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="d7617-177">Possible values are: `Free`, `Tentative`, `Busy`, `Oof`, `WorkingElsewhere`.</span></span>|
|<span data-ttu-id="d7617-178">start</span><span class="sxs-lookup"><span data-stu-id="d7617-178">start</span></span>|[<span data-ttu-id="d7617-179">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d7617-179">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="d7617-180">Время начала события.</span><span class="sxs-lookup"><span data-stu-id="d7617-180">The start time of the event.</span></span> <br/><br/><span data-ttu-id="d7617-p107">По умолчанию время начала указано в формате UTC. Можно дополнительно указать часовой пояс в элементе StartTimeZone, задать время завершения согласно этому часовому поясу и UTC-смещение. Обратите внимание, что если вы используете StartTimeZone, следует также указать значение EndTimeZone.</span><span class="sxs-lookup"><span data-stu-id="d7617-p107">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="d7617-184">Пример указания даты (25 февраля 2015 г., 19:34 по тихоокеанскому поясному времени): "2015-02-25T19:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="d7617-184">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
|<span data-ttu-id="d7617-185">subject</span><span class="sxs-lookup"><span data-stu-id="d7617-185">subject</span></span>|<span data-ttu-id="d7617-186">String</span><span class="sxs-lookup"><span data-stu-id="d7617-186">String</span></span>|<span data-ttu-id="d7617-187">Текст в строке темы сообщения о событии.</span><span class="sxs-lookup"><span data-stu-id="d7617-187">The text of the event's subject line.</span></span>|

<span data-ttu-id="d7617-188">Так как ресурс **event** поддерживает [расширения](../../../concepts/extensibility_overview.md), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **event**.</span><span class="sxs-lookup"><span data-stu-id="d7617-188">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

## <a name="response"></a><span data-ttu-id="d7617-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7617-189">Response</span></span>

<span data-ttu-id="d7617-190">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d7617-190">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7617-191">Пример</span><span class="sxs-lookup"><span data-stu-id="d7617-191">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d7617-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7617-192">Request</span></span>

<span data-ttu-id="d7617-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7617-193">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d7617-194">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7617-194">Response</span></span>

<span data-ttu-id="d7617-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d7617-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d7617-198">См. также</span><span class="sxs-lookup"><span data-stu-id="d7617-198">See also</span></span>

- [<span data-ttu-id="d7617-199">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="d7617-199">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="d7617-200">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="d7617-200">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
