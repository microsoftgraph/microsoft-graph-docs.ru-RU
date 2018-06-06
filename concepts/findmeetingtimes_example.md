# <a name="find-possible-meeting-times-on-the-outlook-calendar"></a><span data-ttu-id="bc4e5-101">Поиск времени для проведения собрания в календаре Outlook</span><span class="sxs-lookup"><span data-stu-id="bc4e5-101">Find possible meeting times on the Outlook calendar</span></span>

<span data-ttu-id="bc4e5-p101">В организации или учебном заведении поиск времени и места для проведения собрания часто влечет за собой дополнительные расходы. Приложения Microsoft Graph могут находить интервалы времени для проведения собраний, удовлетворяющие указанным ограничениям, используя действие [findMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md).</span><span class="sxs-lookup"><span data-stu-id="bc4e5-p101">In a workplace or school, looking for a common time and place to meet often incurs overhead. Microsoft Graph applications can use [findMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) to identify any possible meeting times that satisfy time, location, and other constraints.</span></span>   

<span data-ttu-id="bc4e5-p102">Действие **findMeetingTimes** позволяет указать такие условия, как диапазон времени, продолжительность, обязательные и необязательные участники, а также тип мероприятия (**activityDomain**). Действие учитывает рабочие графики и сведения о доступности участников и организатора и предлагает интервалы времени, которые подходят для участников и типа мероприятия. Например, мероприятия, связанные с работой, всегда предлагается проводить в рабочее время организатора и участников, а собрания, на которых могут присутствовать обязательные участники, располагаются в списке выше.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-p102">The **findMeetingTimes** action lets you specify conditions such as the meeting date/time range, duration, optional or required attendees, and nature of the activity (**activityDomain**). The action takes into account the attendees' and organizer's normal work schedules and free/busy status, and suggests times that are appropriate for the participants and type of activity. For instance, suggestions for a work-related activity always occur during the work hours of the organizer and attendees, and suggestions where required attendees are available are ordered higher up in the suggested list.</span></span>

<span data-ttu-id="bc4e5-p103">В Office 365 рабочее время и часовые пояса настраиваются для каждого почтового ящика. Действие **findMeetingTimes** учитывает разницу между часовыми поясами организатора и участников. По умолчанию действие **findMeetingTimes** возвращает предложения в формате UTC. Вы можете использовать следующий заголовок запроса, чтобы действие **findMeetingTimes** показывало предложения в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-p103">In Office 365, work hours and time zones are configurable per mailbox. The **findMeetingTimes** action handles time zone variations among the organizer and attendees. By default, **findMeetingTimes** returns suggestions in UTC. You can use the following request header to have **findMeetingTimes** return suggestions expressed in a specific time zone.</span></span>
```
Prefer: outlook.timezone="{time-zone-string}}"
```

<span data-ttu-id="bc4e5-111">Вы можете указать процент (**minimumAttendeePercentage**) для кворума, чтобы действие **findMeetingTimes** показывало предложения, только если этот минимальный процент участников может присутствовать. Это особенно полезно при планировании больших собраний.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-111">Especially useful for larger meetings, you can specify a percentage (**minimumAttendeePercentage**) for a quorum and have **findMeetingTimes** return suggestions only if that minimum attendee availability is met.</span></span>

<span data-ttu-id="bc4e5-p104">Если действие **findMeetingTimes** не может предложить время проведения собрания, оно указывает конкретную причину (**emptySuggestionsReason**), например, организатор или обязательный участник не может присутствовать. Это значение поможет вам лучше настраивать параметры и снова вызывать метод **findMeetingTimes**.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-p104">If **findMeetingTimes** cannot suggest any meeting times, it indicates a specific reason (**emptySuggestionsReason**), such as the organizer or a required attendee not available. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>

><span data-ttu-id="bc4e5-114">**Примечание.** В настоящее время действие **findMeetingTimes** доступно для рабочих и учебных почтовых ящиков Office 365, но не для личных почтовых ящиков outlook.com.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-114">**Note** The **findMeetingTimes** action is currently available to Office 365 work or school mailboxes, but not personal, outlook.com mailboxes.</span></span>

## <a name="example"></a><span data-ttu-id="bc4e5-115">Пример</span><span class="sxs-lookup"><span data-stu-id="bc4e5-115">Example</span></span>

<span data-ttu-id="bc4e5-p105">В следующем примере показано, как использовать действие **findMeetingTimes**, чтобы найти время для проведения двухчасового собрания двух пользователей, учитывая их сведения о доступности и рабочие графики, а также тот факт, что участник будет временно отсутствовать. Так как это собрание организовывается для двоих, требуется 100-процентное присутствие. Ниже показано расписание пользователей.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-p105">The following example shows how to use **findMeetingTimes** to return possible times for 2 users to meet for a couple of hours, taking into account the users' free/busy and work schedules, and the attendee being away for part of the time. Because there are only 2 users for this meeting, suggestions require 100% attendance. The following shows the users' free/busy schedule.</span></span>

### <a name="organizers-calendar"></a><span data-ttu-id="bc4e5-119">Календарь организатора</span><span class="sxs-lookup"><span data-stu-id="bc4e5-119">Organizer's calendar</span></span>

<span data-ttu-id="bc4e5-120">![Рабочий календарь организатора на 17–21 апреля: показано свободное и занятое время](./images/findmeetingtimes_organizer_free_busy.jpg "Рабочий календарь организатора на 17–21 апреля: показано свободное и занятое время")</span><span class="sxs-lookup"><span data-stu-id="bc4e5-120">![The organizer's work calendar for April 17-21 showing free-busy times](./images/findmeetingtimes_organizer_free_busy.jpg "The organizer's work calendar for April 17-21 showing free-busy times")</span></span>

### <a name="attendees-calendar"></a><span data-ttu-id="bc4e5-121">Календарь участника</span><span class="sxs-lookup"><span data-stu-id="bc4e5-121">Attendee's calendar</span></span>

<span data-ttu-id="bc4e5-122">![Рабочий календарь участника на 17–21 апреля: показано свободное и занятое время](./images/findmeetingtimes_attendee_free_busy.jpg "Рабочий календарь участника на 17–21 апреля: показано свободное и занятое время")</span><span class="sxs-lookup"><span data-stu-id="bc4e5-122">![The attendee's work calendar for April 17-21 showing free-busy times](./images/findmeetingtimes_attendee_free_busy.jpg "The attendee's work calendar for April 17-21 showing free-busy times")</span></span>

<span data-ttu-id="bc4e5-123">В примере выполняется 2 вызова **findMeetingTimes**:</span><span class="sxs-lookup"><span data-stu-id="bc4e5-123">The example makes 2 calls to **findMeetingTimes**:</span></span>

1. <span data-ttu-id="bc4e5-p106">Первый вызов ищет время для собрания с 18 по 20 апреля. Так как участника не будет на месте 18 и 19 апреля, а 20 апреля свободное время участников не совпадает, первый вызов не возвращает предложений по причине недоступности участников (**emptySuggestionsReason**).</span><span class="sxs-lookup"><span data-stu-id="bc4e5-p106">The first call looks in the date range of April 18-20. As the attendee is out-of-office on April 18-19, and there is no commonly available time on April 20, the first call returns no suggestions with the reason (**emptySuggestionsReason**) that attendees are not available.</span></span>
2. <span data-ttu-id="bc4e5-126">Второй вызов ищет время для собрания 21 апреля и предлагает провести его с 14:00 до 16:00.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-126">The second call looks for availability on April 21 and returns a suggestion of 2-4pm.</span></span>

<span data-ttu-id="bc4e5-p107">Два вызова действия **findMeetingTimes** включают следующие параметры. Все [параметры](../api-reference/v1.0/api/user_findmeetingtimes.md#request-body) для действия **findMeetingTimes** являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-p107">The two calls to **findMeetingTimes** include the following parameters. All [parameters](../api-reference/v1.0/api/user_findmeetingtimes.md#request-body) for **findMeetingTimes** are optional.</span></span>

- <span data-ttu-id="bc4e5-129">**attendees**: один участник, Samantha Booth, для свойства **type** которого задано значение `required`.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-129">**attendees**: one attendee, Samantha Booth, set as `required` for the **type** property</span></span>
- <span data-ttu-id="bc4e5-130">**locationConstraint**: предлагать место не нужно.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-130">**locationConstraint**: does not require any location suggestion</span></span>
- <span data-ttu-id="bc4e5-131">**timeConstraint**: первый вызов просматривает диапазон времени с 9:00 18 апреля до 17:00 20 апреля, после того как он не может предложить время, второй вызов просматривает диапазон времени с 9:00 до 17:00 21 апреля.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-131">**timeConstraint**: the first call looks in the date/time range of April 18, 9am to April 20, 5pm; after the first call fails to suggest any times, the second call looks at April 21, 9am to 5pm</span></span>
- <span data-ttu-id="bc4e5-132">**meetingDuration**: два часа.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-132">**meetingDuration**: two hours</span></span>
- <span data-ttu-id="bc4e5-133">**returnSuggestionReasons**: в этом примере требуется показать причину для каждого предложения.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-133">**returnSuggestionReasons**: this example requires a reason for each suggestion</span></span>
- <span data-ttu-id="bc4e5-134">**minimumAttendeePercentage**: 100 %, так как участник должен быть свободен в любое предложенное время.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-134">**minimumAttendeePercentage**: 100%, as the attendee must be able to attend for any suggested time</span></span>

### <a name="first-request"></a><span data-ttu-id="bc4e5-135">Первый запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e5-135">First request</span></span>

<span data-ttu-id="bc4e5-136">Поиск 2-часового интервала 18–20 апреля, в течение которого оба пользователя будут свободны.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-136">Look for a 2-hour free time slot for both users over April 18-20.</span></span>

<!-- {
  "blockType": "request",
  "name": "findmeetingtimes_example_first"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/findMeetingTimes
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com" 
      } 
    }
  ],  
  "locationConstraint": { 
    "isRequired": "false",  
    "suggestLocation": "false",  
    "locations": [ 
      { 
        "resolveAvailability": "false",
        "displayName": "Conf room Hood" 
      } 
    ] 
  },  
  "timeConstraint": {
    "activityDomain":"work", 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2017-04-18T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2017-04-20T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": "true",
  "minimumAttendeePercentage": "100"
}
```

### <a name="first-response"></a><span data-ttu-id="bc4e5-137">Первый ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e5-137">First response</span></span>
<span data-ttu-id="bc4e5-138">В рабочее время 18–20 апреля 2-часовый интервал, в течение которого оба пользователя будут свободны, отсутствует.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-138">There is no 2-hour time slot during the work hours of April 18-20 when both users are available.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-Length: 184

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
    "emptySuggestionsReason":"AttendeesUnavailable",
    "meetingTimeSuggestions":[

    ]
}
```

### <a name="second-request"></a><span data-ttu-id="bc4e5-139">Второй запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e5-139">Second request</span></span>
<span data-ttu-id="bc4e5-140">Поиск 2-часового интервала 21 апреля.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-140">Look for a 2-hour time slot on April 21.</span></span>
<!-- {
  "blockType": "request",
  "name": "findmeetingtimes_example_second"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/findMeetingTimes
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com" 
      } 
    }
  ],  
  "locationConstraint": { 
    "isRequired": "false",  
    "suggestLocation": "false",  
    "locations": [ 
      { 
        "resolveAvailability": "false",
        "displayName": "Conf room Hood" 
      } 
    ] 
  },  
  "timeConstraint": {
    "activityDomain":"work", 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2017-04-21T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2017-04-21T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": "true",
  "minimumAttendeePercentage": "100"
}
```

### <a name="second-response"></a><span data-ttu-id="bc4e5-141">Второй ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e5-141">Second response</span></span>
<span data-ttu-id="bc4e5-142">Второй запрос **findMeetingTimes** предлагает пользователям провести собрание 21 апреля с 14:00 до 16:00.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-142">The second **findMeetingTimes** request suggests April 21, 2-4pm for both users to meet.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-Length: 714

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
    "emptySuggestionsReason":"",
    "meetingTimeSuggestions":[
        {
            "confidence":100.0,
            "organizerAvailability":"free",
            "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available.",
            "meetingTimeSlot":{
                "start":{
                    "dateTime":"2017-04-21T14:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                },
                "end":{
                    "dateTime":"2017-04-21T16:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                }
            },
            "attendeeAvailability":[
                {
                    "availability":"free",
                    "attendee":{
                        "type":"required",
                        "emailAddress":{
                            "address":"samanthab@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations":[
                {
                    "displayName":"Conf room Hood"
                }
            ]
        }
    ]
}
```



## <a name="next-steps"></a><span data-ttu-id="bc4e5-143">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="bc4e5-143">Next steps</span></span>

<span data-ttu-id="bc4e5-p108">Иногда не все участники могут присутствовать на собрании. Указав необязательный параметр **minimumAttendeePercentage**, вы можете сделать так, чтобы действие **findMeetingTimes** предлагало время, только если _вероятность_ присутствия всех участников достигает определенного процента. Узнайте больше о [достоверности предложения](../api-reference/v1.0/api/user_findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) и других [параметрах](../api-reference/v1.0/api/user_findmeetingtimes.md#request-body) и применяйте их для больших собраний.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-p108">There are times when not all attendees can attend a meeting. You can have **findMeetingTimes** suggest a time if the _confidence_ for attendance reaches a certain percentage, by specifying the **minimumAttendeePercentage** optional parameter. Learn more about the [confidence of a meeting suggestion](../api-reference/v1.0/api/user_findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) and other [parameters](../api-reference/v1.0/api/user_findmeetingtimes.md#request-body), and apply them as appropriate for meetings of larger sizes.</span></span>

<span data-ttu-id="bc4e5-147">Получив предложения по времени проведения собрания, вы можете:</span><span class="sxs-lookup"><span data-stu-id="bc4e5-147">After getting meeting time suggestions, you may want to:</span></span>

1. <span data-ttu-id="bc4e5-148">[создать событие и отправить приглашение на собрание](../api-reference/v1.0/api/user_post_events.md);</span><span class="sxs-lookup"><span data-stu-id="bc4e5-148">[Create an event and send it as a meeting request](../api-reference/v1.0/api/user_post_events.md)</span></span>
2. <span data-ttu-id="bc4e5-149">[добавить вложение](../api-reference/v1.0/api/event_post_attachments.md) в событие.</span><span class="sxs-lookup"><span data-stu-id="bc4e5-149">[Add an attachment](../api-reference/v1.0/api/event_post_attachments.md) to the event</span></span>

<span data-ttu-id="bc4e5-150">Узнайте больше об [интеграции с Календарем Outlook](outlook-calendar-concept-overview.md).</span><span class="sxs-lookup"><span data-stu-id="bc4e5-150">Find out more about [integrating with Outlook calendar](outlook-calendar-concept-overview.md).</span></span>
