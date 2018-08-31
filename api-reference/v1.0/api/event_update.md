# <a name="update-event"></a><span data-ttu-id="a99fe-101">Событие обновления</span><span class="sxs-lookup"><span data-stu-id="a99fe-101">Update event</span></span>

<span data-ttu-id="a99fe-102">Обновить свойства [событийного](../resources/event.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="a99fe-102">Update the properties of event object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a99fe-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a99fe-103">Permissions</span></span>
<span data-ttu-id="a99fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a99fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a99fe-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a99fe-106">Permission type</span></span>      | <span data-ttu-id="a99fe-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a99fe-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a99fe-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a99fe-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a99fe-109">Календари.ЧитатьПисать</span><span class="sxs-lookup"><span data-stu-id="a99fe-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a99fe-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a99fe-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a99fe-111">Календари.ЧитатьПисать</span><span class="sxs-lookup"><span data-stu-id="a99fe-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a99fe-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a99fe-112">Application</span></span> | <span data-ttu-id="a99fe-113">Календари.ЧитатьПисать</span><span class="sxs-lookup"><span data-stu-id="a99fe-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a99fe-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a99fe-114">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="a99fe-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a99fe-115">Request headers</span></span>
| <span data-ttu-id="a99fe-116">Имя</span><span class="sxs-lookup"><span data-stu-id="a99fe-116">Name</span></span>       | <span data-ttu-id="a99fe-117">Тип</span><span class="sxs-lookup"><span data-stu-id="a99fe-117">Type</span></span> | <span data-ttu-id="a99fe-118">Описание</span><span class="sxs-lookup"><span data-stu-id="a99fe-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a99fe-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a99fe-119">Authorization</span></span>  | <span data-ttu-id="a99fe-120">string</span><span class="sxs-lookup"><span data-stu-id="a99fe-120">string</span></span>  | <span data-ttu-id="a99fe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a99fe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a99fe-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a99fe-123">Request body</span></span>
<span data-ttu-id="a99fe-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a99fe-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a99fe-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="a99fe-127">Property</span></span>     | <span data-ttu-id="a99fe-128">Тип</span><span class="sxs-lookup"><span data-stu-id="a99fe-128">Type</span></span>   |<span data-ttu-id="a99fe-129">Описание</span><span class="sxs-lookup"><span data-stu-id="a99fe-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a99fe-130">участники</span><span class="sxs-lookup"><span data-stu-id="a99fe-130">attendees</span></span>|[<span data-ttu-id="a99fe-131">Участник</span><span class="sxs-lookup"><span data-stu-id="a99fe-131">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="a99fe-132">Коллекция участников события.</span><span class="sxs-lookup"><span data-stu-id="a99fe-132">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="a99fe-133">текст</span><span class="sxs-lookup"><span data-stu-id="a99fe-133">body</span></span>|[<span data-ttu-id="a99fe-134">ТекстЭлемента</span><span class="sxs-lookup"><span data-stu-id="a99fe-134">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="a99fe-135">Текст сообщения, связанного с событием.</span><span class="sxs-lookup"><span data-stu-id="a99fe-135">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="a99fe-136">категории</span><span class="sxs-lookup"><span data-stu-id="a99fe-136">categories</span></span>|<span data-ttu-id="a99fe-137">Строка</span><span class="sxs-lookup"><span data-stu-id="a99fe-137">String</span></span>|<span data-ttu-id="a99fe-138">Категории, связанные с событием.</span><span class="sxs-lookup"><span data-stu-id="a99fe-138">The categories associated with the event.</span></span>|
|<span data-ttu-id="a99fe-139">завершение</span><span class="sxs-lookup"><span data-stu-id="a99fe-139">end</span></span>|[<span data-ttu-id="a99fe-140">ДатаВремяЧасовойПояс</span><span class="sxs-lookup"><span data-stu-id="a99fe-140">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="a99fe-141">Дата и время завершения события.</span><span class="sxs-lookup"><span data-stu-id="a99fe-141">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="a99fe-p104">По умолчанию время завершения указано в формате UTC. Можно дополнительно указать часовой пояс в элементе EndTimeZone, задать время завершения согласно этому часовому поясу и UTC-смещение. Обратите внимание, что если вы используете EndTimeZone, следует также указать значение StartTimeZone.</span><span class="sxs-lookup"><span data-stu-id="a99fe-p104">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="a99fe-145">Пример указания даты (25 февраля 2015 г., 21:34 по тихоокеанскому поясному времени): "2015-02-25T21:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="a99fe-145">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
|<span data-ttu-id="a99fe-146">важность</span><span class="sxs-lookup"><span data-stu-id="a99fe-146">importance</span></span>|<span data-ttu-id="a99fe-147">Строка</span><span class="sxs-lookup"><span data-stu-id="a99fe-147">String</span></span>|<span data-ttu-id="a99fe-148">Важность события.</span><span class="sxs-lookup"><span data-stu-id="a99fe-148">The importance of the event.</span></span> <span data-ttu-id="a99fe-149">Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="a99fe-149">The possible values are `low`, `normal`, `high`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="a99fe-150">ВесьДень</span><span class="sxs-lookup"><span data-stu-id="a99fe-150">isAllDay</span></span>|<span data-ttu-id="a99fe-151">Булев</span><span class="sxs-lookup"><span data-stu-id="a99fe-151">Boolean</span></span>|<span data-ttu-id="a99fe-152">Задайте значение true, если событие длится весь день.</span><span class="sxs-lookup"><span data-stu-id="a99fe-152">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="a99fe-153">НапоминаниеВключено</span><span class="sxs-lookup"><span data-stu-id="a99fe-153">isReminderOn</span></span>|<span data-ttu-id="a99fe-154">Булев</span><span class="sxs-lookup"><span data-stu-id="a99fe-154">Boolean</span></span>|<span data-ttu-id="a99fe-155">Задайте значение true, если установлено напоминание пользователю о событии.</span><span class="sxs-lookup"><span data-stu-id="a99fe-155">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="a99fe-156">местоположение</span><span class="sxs-lookup"><span data-stu-id="a99fe-156">location</span></span>|[<span data-ttu-id="a99fe-157">Местоположение</span><span class="sxs-lookup"><span data-stu-id="a99fe-157">Location</span></span>](../resources/location.md)|<span data-ttu-id="a99fe-158">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="a99fe-158">The location of the event.</span></span>|
|<span data-ttu-id="a99fe-159">местоположения</span><span class="sxs-lookup"><span data-stu-id="a99fe-159">locations</span></span>|<span data-ttu-id="a99fe-160">Коллекция [location](../resources/location.md)</span><span class="sxs-lookup"><span data-stu-id="a99fe-160">[location](../resources/location.md) collection</span></span>|<span data-ttu-id="a99fe-161">Места проведения мероприятия или участия в нем.</span><span class="sxs-lookup"><span data-stu-id="a99fe-161">The locations where the event is held or attended from.</span></span> <span data-ttu-id="a99fe-162">Свойства **location** и **locations** всегда совпадают друг с другом.</span><span class="sxs-lookup"><span data-stu-id="a99fe-162">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="a99fe-163">Если вы обновите свойство **местоположения**, любые предыдущие местоположения в совокупности **местоположений** будут удалены и заменены новым значением **местоположения**.</span><span class="sxs-lookup"><span data-stu-id="a99fe-163">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="a99fe-164">повторение</span><span class="sxs-lookup"><span data-stu-id="a99fe-164">recurrence</span></span>|[<span data-ttu-id="a99fe-165">ШаблонноеПовторение</span><span class="sxs-lookup"><span data-stu-id="a99fe-165">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="a99fe-166">Расписание повторения события.</span><span class="sxs-lookup"><span data-stu-id="a99fe-166">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="a99fe-167">напоминаниеМинутыДоНачала</span><span class="sxs-lookup"><span data-stu-id="a99fe-167">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="a99fe-168">Int32</span><span class="sxs-lookup"><span data-stu-id="a99fe-168">Int32</span></span>|<span data-ttu-id="a99fe-169">Позволяет указать, за сколько минут до начала события появляется напоминание.</span><span class="sxs-lookup"><span data-stu-id="a99fe-169">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="a99fe-170">ответЗатребован</span><span class="sxs-lookup"><span data-stu-id="a99fe-170">responseRequested</span></span>|<span data-ttu-id="a99fe-171">Булев</span><span class="sxs-lookup"><span data-stu-id="a99fe-171">Boolean</span></span>|<span data-ttu-id="a99fe-172">Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения.</span><span class="sxs-lookup"><span data-stu-id="a99fe-172">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="a99fe-173">чувствительность</span><span class="sxs-lookup"><span data-stu-id="a99fe-173">sensitivity</span></span>|<span data-ttu-id="a99fe-174">Строка</span><span class="sxs-lookup"><span data-stu-id="a99fe-174">String</span></span>| <span data-ttu-id="a99fe-175">Возможные значения: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="a99fe-175">The possible values are `normal`, `personal`, `private`, `confidential`, , , , , , , , or .</span></span>|
|<span data-ttu-id="a99fe-176">показатьКак</span><span class="sxs-lookup"><span data-stu-id="a99fe-176">showAs</span></span>|<span data-ttu-id="a99fe-177">Строка</span><span class="sxs-lookup"><span data-stu-id="a99fe-177">String</span></span>|<span data-ttu-id="a99fe-178">Отображаемое состояние.</span><span class="sxs-lookup"><span data-stu-id="a99fe-178">The status to show.</span></span> <span data-ttu-id="a99fe-179">Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a99fe-179">The possible values are `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`, , , , , , or .</span></span>|
|<span data-ttu-id="a99fe-180">начать</span><span class="sxs-lookup"><span data-stu-id="a99fe-180">start</span></span>|[<span data-ttu-id="a99fe-181">ДатаВремяЧасовойПояс</span><span class="sxs-lookup"><span data-stu-id="a99fe-181">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="a99fe-182">Время начала события.</span><span class="sxs-lookup"><span data-stu-id="a99fe-182">The start time of the event.</span></span> <br/><br/><span data-ttu-id="a99fe-p108">По умолчанию время начала указано в формате UTC. Можно дополнительно указать часовой пояс в элементе StartTimeZone, задать время завершения согласно этому часовому поясу и UTC-смещение. Обратите внимание, что если вы используете StartTimeZone, следует также указать значение EndTimeZone.</span><span class="sxs-lookup"><span data-stu-id="a99fe-p108">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="a99fe-186">Пример указания даты (25 февраля 2015 г., 19:34 по тихоокеанскому поясному времени): "2015-02-25T19:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="a99fe-186">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
|<span data-ttu-id="a99fe-187">тема</span><span class="sxs-lookup"><span data-stu-id="a99fe-187">subject</span></span>|<span data-ttu-id="a99fe-188">String</span><span class="sxs-lookup"><span data-stu-id="a99fe-188">String</span></span>|<span data-ttu-id="a99fe-189">Текст в строке темы события.</span><span class="sxs-lookup"><span data-stu-id="a99fe-189">The text of the event's subject line.</span></span>|

<span data-ttu-id="a99fe-190">Так как ресурс **события** поддерживает [расширения](../../../concepts/extensibility_overview.md), вы можете использовать эту `PATCH` операцию для добавления, обновления или удаления ваших собственных данных, касающихся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **события**.</span><span class="sxs-lookup"><span data-stu-id="a99fe-190">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>  
  
<span data-ttu-id="a99fe-191">Если **событие**, которое вы обновляете, является главным событием повторяющейся серии, содержащим несколько участников и экземпляры, которые были обновлены отдельно, будет отправлено несколько уведомлений по электронной почте: одно для главной серии и по одному для каждого экземпляра, который был обновлен.</span><span class="sxs-lookup"><span data-stu-id="a99fe-191">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>  

## <a name="response"></a><span data-ttu-id="a99fe-192">Ответ</span><span class="sxs-lookup"><span data-stu-id="a99fe-192">Response</span></span>

<span data-ttu-id="a99fe-193">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [события](../resources/event.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a99fe-193">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>  

><span data-ttu-id="a99fe-194">**Примечание:** Этот метод может вернуть ответ "Неверный запрос HTTP 400" с кодом ошибки `ErrorOccurrenceCrossingBoundary` и следующее сообщение об ошибке: "Измененная копия пересекается со смежной копией или перекрывает ее".</span><span class="sxs-lookup"><span data-stu-id="a99fe-194">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="a99fe-195">Это указывает на то, что обновление нарушает следующее ограничение Outlook для исключения повторений: копия не может быть перемещена на день или перед днем предыдущей копии, а также на день или после дня следующей копии.</span><span class="sxs-lookup"><span data-stu-id="a99fe-195">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="a99fe-196">Пример</span><span class="sxs-lookup"><span data-stu-id="a99fe-196">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a99fe-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="a99fe-197">Request</span></span>

<span data-ttu-id="a99fe-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a99fe-198">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a99fe-199">Ответ</span><span class="sxs-lookup"><span data-stu-id="a99fe-199">Response</span></span>

<span data-ttu-id="a99fe-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a99fe-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="a99fe-203">См. также</span><span class="sxs-lookup"><span data-stu-id="a99fe-203">See also</span></span>

- [<span data-ttu-id="a99fe-204">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="a99fe-204">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="a99fe-205">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="a99fe-205">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="a99fe-206">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="a99fe-206">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
