# <a name="get-freebusy-schedule-of-users-and-resources-preview"></a><span data-ttu-id="f658a-101">Получение графика доступности пользователей и ресурсов (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="f658a-101">Get free/busy schedule for users and resources (preview)</span></span>

<span data-ttu-id="f658a-102">На работе или в школе часто возникают ситуации, в которых требуется отобразить информацию о том, свободен ли пользователь для проведения совещания, или получить данные о доступности рабочей группы, помещения или оборудования в определенный период времени.</span><span class="sxs-lookup"><span data-stu-id="f658a-102">In a work or school setting, a common scenario is to see when a user is free for meeting, or to browse the availability of a team, room, or equipment for a time period.</span></span>

<span data-ttu-id="f658a-103">Действие [getSchedule](../api-reference/beta/api/calendar_getschedule.md) позволяет получить информацию о доступности из одного или нескольких объектов — пользователей, списков рассылки или ресурсов — в течение определенного времени.</span><span class="sxs-lookup"><span data-stu-id="f658a-103">The [getSchedule](../api-reference/beta/api/calendar_getschedule.md) action lets you get the availability information of one or more entities - users, distribution lists, or resources - for a specific period of time.</span></span> 

## <a name="example"></a><span data-ttu-id="f658a-104">Пример</span><span class="sxs-lookup"><span data-stu-id="f658a-104">Example</span></span>

<span data-ttu-id="f658a-105">Простым примером является получение графика занятости коллеги по имени Алекс, в определенный день, с 9:00 до 18:00 по стандартному тихоокеанскому времени.</span><span class="sxs-lookup"><span data-stu-id="f658a-105">A simple example is to find the free/busy schedule of a coworker, Alex, on a specific day, from 9am to 6pm, Pacitfic Standard Time:</span></span>

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule_concept"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/getschedule 
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{        
    "Schedules": ["AlexW@contoso.OnMicrosoft.com"],
    "StartTime": {
        "dateTime": "2018-08-06T09:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "EndTime": {
        "dateTime": "2018-08-06T18:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "availabilityViewInterval": "15"
}
```

<span data-ttu-id="f658a-106">**getSchedule** возвращает два элемента графика, которые соответствуют событиям, имеющимся в используемом Алекс по умолчанию календаре, и которые отображают время начала и время завершения каждого из событий, а также сведения о доступности пользователя в ходе каждого из них.</span><span class="sxs-lookup"><span data-stu-id="f658a-106">**getSchedule** returns two schedule items that match existing events in Alex' default calendar, showing the start and end times of each event and its free/busy status.</span></span> <span data-ttu-id="f658a-107">Можно предположить, что в оставшееся время, в течение указанного дня и временного диапазона, Алекс будет свободен.</span><span class="sxs-lookup"><span data-stu-id="f658a-107">You can assume Alex is free for the remaining time in that date/time range.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.scheduleInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value":[
        {
            "scheduleId":"AlexW@contoso.OnMicrosoft.com",
            "availabilityView":"111111002222222200000000000000000000",
            "scheduleItems":[
                {
                    "isPrivate":false,
                    "status":"Tentative",
                    "start":{
                        "dateTime":"2018-08-06T09:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T10:30:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                },
                {
                    "isPrivate":false,
                    "status":"Busy",
                    "start":{
                        "dateTime":"2018-08-06T11:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T13:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                }
            ],
            "workingHours":{
                "daysOfWeek":[
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime":"08:00:00.0000000",
                "endTime":"17:00:00.0000000",
                "timeZone":{
                    "@odata.type":"#microsoft.graph.customTimeZone",
                    "bias":480,
                    "name":"Customized Time Zone",
                    "standardOffset":{
                        "time":"02:00:00.0000000",
                        "dayOccurrence":1,
                        "dayOfWeek":"sunday",
                        "month":11,
                        "year":0
                    },
                    "daylightOffset":{
                        "daylightBias":-60,
                        "time":"02:00:00.0000000",
                        "dayOccurrence":2,
                        "dayOfWeek":"sunday",
                        "month":3,
                        "year":0
                    }
                }
            }
        }
    ]
}

```

<span data-ttu-id="f658a-108">Помимо сведений о доступности и рабочем времени Алекс **getSchedule** также возвращает **availabilityView** — объединенное представление доступности Алекс в течение этого дня.</span><span class="sxs-lookup"><span data-stu-id="f658a-108">Apart from the free/busy schedule and working hours of Alex, **getSchedule** also returns **availabilityView**, which is a merged view of Alex' availability for that day.</span></span> <span data-ttu-id="f658a-109">Объединенное представление — это строка, которая состоит из периодов времени, составляющих указанный день, где для каждого временного интервала указывается доступность Алекс с применением следующих условных обозначений:</span><span class="sxs-lookup"><span data-stu-id="f658a-109">The merged view is a string that consists of time slots covering that day, with each time slot indicating Alex' availability using the following convention:</span></span> 

- <span data-ttu-id="f658a-110">`0`= свободен</span><span class="sxs-lookup"><span data-stu-id="f658a-110">`0`= free</span></span>
- <span data-ttu-id="f658a-111">`1`= под вопросом</span><span class="sxs-lookup"><span data-stu-id="f658a-111">`1`= tentative</span></span>
- <span data-ttu-id="f658a-112">`2`= занят</span><span class="sxs-lookup"><span data-stu-id="f658a-112">`2`= busy</span></span>
- <span data-ttu-id="f658a-113">`3`= нет на месте</span><span class="sxs-lookup"><span data-stu-id="f658a-113">`3`= out of office</span></span>
- <span data-ttu-id="f658a-114">`4`= работа в другом месте.</span><span class="sxs-lookup"><span data-stu-id="f658a-114">`4`= working elsewhere.</span></span> 

<span data-ttu-id="f658a-115">По умолчанию продолжительность каждого периода времени составляет 30 минут.</span><span class="sxs-lookup"><span data-stu-id="f658a-115">By default, the length of each time slot is 30 minutes.</span></span> <span data-ttu-id="f658a-116">В данном примере для настройки периода времени и установки его продолжительности равной 15 минутам используется свойство **availabilityViewInterval**.</span><span class="sxs-lookup"><span data-stu-id="f658a-116">This example uses the **availabilityViewInterval** property to customize the time slot to be 15 minutes.</span></span>

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a><span data-ttu-id="f658a-117">Чем отличается getSchedule от findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="f658a-117">How is getSchedule different from findMeetingTimes</span></span>

<span data-ttu-id="f658a-118">Действия [findMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) и **getSchedule** похожи тем, что оба они позволяют получить информацию о доступности и рабочем времени указанных пользователей и ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f658a-118">The [findMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) action is similar to **getSchedule** in that both read the free/busy status and working hours of specified users and resources.</span></span> <span data-ttu-id="f658a-119">Тем не менее, эти два действия имеют несколько существенных отличий.</span><span class="sxs-lookup"><span data-stu-id="f658a-119">The two actions differ in a few major ways.</span></span>

### <a name="application"></a><span data-ttu-id="f658a-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="f658a-120">Application</span></span>

<span data-ttu-id="f658a-121">Действие **findMeetingTimes** использует определенную бизнес-логику для предложения времени и места проведения собраний и учитывает, к примеру:</span><span class="sxs-lookup"><span data-stu-id="f658a-121">**findMeetingTimes** applies certain business logic to suggest meeting times and locations, such as:</span></span>

- <span data-ttu-id="f658a-122">необязательное или обязательное присутствие каждого лица;</span><span class="sxs-lookup"><span data-stu-id="f658a-122">Optional or mandatory attendance of each entity</span></span>
- <span data-ttu-id="f658a-123">характер запрашиваемой деятельности для определенного времени суток;</span><span class="sxs-lookup"><span data-stu-id="f658a-123">The nature of the requested activity for the time of the day</span></span>
- <span data-ttu-id="f658a-124">минимальное количество лиц, присутствующих на совещании, необходимое для обеспечения кворума.</span><span class="sxs-lookup"><span data-stu-id="f658a-124">The minimum attendance required for a quorum for a meeting</span></span>

<span data-ttu-id="f658a-125">Это подходит для сценариев, которые зависят от[оптимизации определения времени встречи](findmeetingtimes_example.md).</span><span class="sxs-lookup"><span data-stu-id="f658a-125">It is appropriate for scenarios that depend on [streamlining appointment booking](findmeetingtimes_example.md).</span></span>

<span data-ttu-id="f658a-126">Действие **getSchedule** просто возвращает сведения о доступности событий, указанных в каждом из запрашиваемых календарей для заданного периода времени, и предполагает, что оставшееся время в пределах данного временного интервала остается свободным.</span><span class="sxs-lookup"><span data-stu-id="f658a-126">**getSchedule** simply returns the free/busy status of existing events in each of the requested calendars for a given time period, and assumes the remaining time in that time period tp be free.</span></span> <span data-ttu-id="f658a-127">Чтобы использовать эти данные для выполнения сценария, необходимо применить дополнительную бизнес-логику.</span><span class="sxs-lookup"><span data-stu-id="f658a-127">You would then apply further business logic to make use of this data to complete your scenario.</span></span>

### <a name="app-only-support"></a><span data-ttu-id="f658a-128">Поддержка только для программ</span><span class="sxs-lookup"><span data-stu-id="f658a-128">App-only support</span></span>

<span data-ttu-id="f658a-129">Действие **findmeetingtimes** поддерживает только делегированные сценарии, требующие от пользователя входа в программу.</span><span class="sxs-lookup"><span data-stu-id="f658a-129">**findmeetingtimes** supports only delegated scenarios which require a user to have signed in to the app.</span></span> <span data-ttu-id="f658a-130">Программа может считывать события только из тех календарей, которые доступны пользователю, выполнившему вход.</span><span class="sxs-lookup"><span data-stu-id="f658a-130">The app can read events in only the calendars that the signed-in user can access.</span></span> <span data-ttu-id="f658a-131">В число этих календарей могут входить календари, делегированные другими пользователями, или календари, которые используются совместно с пользователем, вошедшим в систему.</span><span class="sxs-lookup"><span data-stu-id="f658a-131">This can include calendars that other users have delegated or shared with the signed-in user.</span></span>

<span data-ttu-id="f658a-132">Действие **getSchedule** поддерживает как делегированные сценарии, так и сценарии, предназначенные только для программы.</span><span class="sxs-lookup"><span data-stu-id="f658a-132">**getSchedule** supports both delegated and app-only scenarios.</span></span> <span data-ttu-id="f658a-133">В дальнейшем, администратор может предоставить программе доступ ко всем календарям без пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="f658a-133">In the latter, an administrator consents the app to access all calendars without a signed-in user.</span></span>


### <a name="version-support"></a><span data-ttu-id="f658a-134">Поддержка версии</span><span class="sxs-lookup"><span data-stu-id="f658a-134">Version support</span></span>

<span data-ttu-id="f658a-135">**findmeetingtimes** обычно доступно для всех программ.</span><span class="sxs-lookup"><span data-stu-id="f658a-135">**findmeetingtimes** is generally available for all apps.</span></span> 

<span data-ttu-id="f658a-136">**getSchedule** в настоящее время доступно [в состоянии предварительной версии](versioning_and_support.md#beta-version) и не подходит для использования в производственных приложениях.</span><span class="sxs-lookup"><span data-stu-id="f658a-136">**getSchedule** is currently available [in preview status](versioning_and_support.md#beta-version), and therefore is not appropriate for use in production apps.</span></span>


## <a name="permissions"></a><span data-ttu-id="f658a-137">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f658a-137">Permissions</span></span>
<span data-ttu-id="f658a-138">Минимальное разрешение, необходимое для получения сведений о доступности, — Calendar.Read.</span><span class="sxs-lookup"><span data-stu-id="f658a-138">The least privileged permission you need to get free/busy information is Calendar.Read.</span></span> <span data-ttu-id="f658a-139">В зависимости от используемого программой сценария оно может предоставляться вошедшим в систему пользователем или администратором.</span><span class="sxs-lookup"><span data-stu-id="f658a-139">Depending on your app scenario, this can be consented by the signed-in user or administrator.</span></span>
<span data-ttu-id="f658a-140">Помимо сведений о доступности и рабочем времени указанных лиц **getSchedule** может также возвращать данные о характере и местоположении события в случае:</span><span class="sxs-lookup"><span data-stu-id="f658a-140">Other than the free/busy status and working hours of requested entities, **getSchedule** can also return the subject and location of an event, provided that:</span></span>

- <span data-ttu-id="f658a-141">если событие помечено, как событие с низким уровнем конфиденциальности — `normal` или `personal`, И если удовлетворяется одно или несколько следующих условий.</span><span class="sxs-lookup"><span data-stu-id="f658a-141">If the event is marked with low sensitivity level - `normal` or `personal` AND one or more of the following conditions applies:</span></span>

- <span data-ttu-id="f658a-142">Параметры календаря, запрашиваемого пользователем, позволяют всем пользователям в организации просматривать заголовки и сведения о местоположении</span><span class="sxs-lookup"><span data-stu-id="f658a-142">The requested user’s calendar settings allow all the users in the organization to view titles and locations</span></span>
- <span data-ttu-id="f658a-143">Календарь, запрашиваемый пользователем, используется совместно с пользователем, вошедшим в систему</span><span class="sxs-lookup"><span data-stu-id="f658a-143">The requested user’s calendar is shared with the signed-in user</span></span>
- <span data-ttu-id="f658a-144">Пользователь, выполнивший вход, является администратором в той же организации, в которой работает запрашиваемый пользователь.</span><span class="sxs-lookup"><span data-stu-id="f658a-144">The signed-in user is an administrator of the same organization as the requested user.</span></span>

## <a name="time-zone-representation"></a><span data-ttu-id="f658a-145">Представление часового пояса</span><span class="sxs-lookup"><span data-stu-id="f658a-145">Time zone representation</span></span>
<span data-ttu-id="f658a-146">По умолчанию время начала и завершения возвращаемых элементов графика доступности отображается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="f658a-146">By default, the start and end times of the returned schedule items are represented in UTC.</span></span> <span data-ttu-id="f658a-147">Чтобы указать часовой пояс, подходящей для вашей программы, можно использовать заоловок `Prefer`.</span><span class="sxs-lookup"><span data-stu-id="f658a-147">You can use a `Prefer` header to specify a time zone appropriate for your app.</span></span> <span data-ttu-id="f658a-148">Пример:</span><span class="sxs-lookup"><span data-stu-id="f658a-148">As an example:</span></span> 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a><span data-ttu-id="f658a-149">Ограничения и состояния ошибки</span><span class="sxs-lookup"><span data-stu-id="f658a-149">Limits and error conditions</span></span>
<span data-ttu-id="f658a-150">Принимайте во внимание следующие ограничения и состояния ошибки.</span><span class="sxs-lookup"><span data-stu-id="f658a-150">Be aware of the following limits and error condition:</span></span>

- <span data-ttu-id="f658a-151">**getSchedule** может выполнять поиск информации о доступности для 20 объектов единовременно.</span><span class="sxs-lookup"><span data-stu-id="f658a-151">**getSchedule** can support looking up free/busy information for up to 20 entities at once.</span></span> <span data-ttu-id="f658a-152">Это ограничение распространяется на количество пользователей, указанных в индивидуальном порядке, или заданных в качестве членов списка рассылки, а также  на количество ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f658a-152">This limit applies to the number of users identified individually or as members of a distribution list, and to the number of resources as well.</span></span>
- <span data-ttu-id="f658a-153">Период времени, используемый для поиска, должен составлять менее 42 дней.</span><span class="sxs-lookup"><span data-stu-id="f658a-153">The time period to look up must be less than 42 days.</span></span>
- <span data-ttu-id="f658a-154">Если действие **getSchedule** не может определить указанного пользователя или запрашиваемый ресурс, то оно возвращает один элемент графика и выдает ошибку.</span><span class="sxs-lookup"><span data-stu-id="f658a-154">If **getSchedule** cannot identify a specified user or resource, it returns a single schedule item and indicates the error.</span></span> 

## <a name="see-also"></a><span data-ttu-id="f658a-155">См. также</span><span class="sxs-lookup"><span data-stu-id="f658a-155">See also</span></span>
- [<span data-ttu-id="f658a-156">Справочник по разрешениям</span><span class="sxs-lookup"><span data-stu-id="f658a-156">Permissions reference</span></span>](permissions_reference.md#calendars-permissions)
- [<span data-ttu-id="f658a-157">Поиск времени для проведения собрания в календаре Outlook</span><span class="sxs-lookup"><span data-stu-id="f658a-157">Find possible meeting times on the Outlook calendar</span></span>](findmeetingtimes_example.md)
