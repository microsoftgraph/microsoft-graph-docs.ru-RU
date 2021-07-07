---
title: Получение расписания доступности пользователей и ресурсов
description: Общим сценарием на рабочем месте или в учебном заведении является просмотр доступности пользователя для собрания или доступности команды, помещения или оборудования в некоторый период времени.
author: tariq-sharif
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: d3d8379f05d6e19505bdf3c45cca0863a685423d
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317133"
---
# <a name="get-freebusy-schedule-of-users-and-resources"></a><span data-ttu-id="44b8d-103">Получение расписания доступности пользователей и ресурсов</span><span class="sxs-lookup"><span data-stu-id="44b8d-103">Get free/busy schedule of users and resources</span></span>

<span data-ttu-id="44b8d-104">Общим сценарием на рабочем месте или в учебном заведении является просмотр доступности пользователя для собрания или доступности команды, помещения или оборудования в некоторый период времени.</span><span class="sxs-lookup"><span data-stu-id="44b8d-104">In a work or school setting, a common scenario is to see when a user is free for meeting, or to browse the availability of a team, room, or equipment for a time period.</span></span>

<span data-ttu-id="44b8d-105">Действие [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0) позволяет получить сведения о доступности одной или нескольких сущностей (пользователей, списков рассылки или ресурсов) для определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="44b8d-105">The [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0) action lets you get the availability information of one or more entities - users, distribution lists, or resources - for a specific period of time.</span></span> 

## <a name="example"></a><span data-ttu-id="44b8d-106">Пример</span><span class="sxs-lookup"><span data-stu-id="44b8d-106">Example</span></span>

<span data-ttu-id="44b8d-107">Простой пример — поиск расписания доступности сотрудника Игоря в определенный день с 9:00 до 18:00 по тихоокеанскому времени:</span><span class="sxs-lookup"><span data-stu-id="44b8d-107">A simple example is to find the free/busy schedule of a coworker, Alex, on a specific day, from 9am to 6pm, Pacific Standard Time:</span></span>

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule_concept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendar/getschedule 
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

<span data-ttu-id="44b8d-108">**getSchedule** возвращает два элемента расписания, соответствующие имеющимся событиям в стандартном календаре Алексея, с указанием времени начала и окончания каждого события и сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="44b8d-108">**getSchedule** returns two schedule items that match existing events in Alex' default calendar, showing the start and end times of each event and its free/busy status.</span></span> <span data-ttu-id="44b8d-109">Можно считать, что в остальное время Алексей свободен в этом диапазоне дат и времени.</span><span class="sxs-lookup"><span data-stu-id="44b8d-109">You can assume Alex is free for the remaining time in that date/time range.</span></span>

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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value":[
        {
            "scheduleId":"AlexW@contoso.OnMicrosoft.com",
            "availabilityView":"111111002222222200000000000000000000",
            "scheduleItems":[
                {
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

<span data-ttu-id="44b8d-110">Кроме расписания доступности и рабочего времени Алексея, **getSchedule** также возвращает свойство **availabilityView**, являющееся объединенным представлением доступности Алексея в этот день.</span><span class="sxs-lookup"><span data-stu-id="44b8d-110">Apart from the free/busy schedule and working hours of Alex, **getSchedule** also returns **availabilityView**, which is a merged view of Alex' availability for that day.</span></span> <span data-ttu-id="44b8d-111">Объединенное представление — это строка, состоящая из интервалов времени, охватывающих этот день, в каждом из которых указывается доступность Алексея с использованием следующего стандарта:</span><span class="sxs-lookup"><span data-stu-id="44b8d-111">The merged view is a string that consists of time slots covering that day, with each time slot indicating Alex' availability using the following convention:</span></span> 

- <span data-ttu-id="44b8d-112">`0`= свободен</span><span class="sxs-lookup"><span data-stu-id="44b8d-112">`0`= free</span></span>
- <span data-ttu-id="44b8d-113">`1`= под вопросом</span><span class="sxs-lookup"><span data-stu-id="44b8d-113">`1`= tentative</span></span>
- <span data-ttu-id="44b8d-114">`2`= занят</span><span class="sxs-lookup"><span data-stu-id="44b8d-114">`2`= busy</span></span>
- <span data-ttu-id="44b8d-115">`3`= не на месте</span><span class="sxs-lookup"><span data-stu-id="44b8d-115">`3`= out of office</span></span>
- <span data-ttu-id="44b8d-116">`4`= работает в другом месте.</span><span class="sxs-lookup"><span data-stu-id="44b8d-116">`4`= working elsewhere.</span></span> 

<span data-ttu-id="44b8d-117">По умолчанию длина каждого интервала времени составляет 30 минут.</span><span class="sxs-lookup"><span data-stu-id="44b8d-117">By default, the length of each time slot is 30 minutes.</span></span> <span data-ttu-id="44b8d-118">В этом примере используется свойство **availabilityViewInterval** для изменения интервала времени до 15 минут.</span><span class="sxs-lookup"><span data-stu-id="44b8d-118">This example uses the **availabilityViewInterval** property to customize the time slot to be 15 minutes.</span></span>

## <a name="how-does-getschedule-compare-with-findmeetingtimes"></a><span data-ttu-id="44b8d-119">Сравнение getSchedule с findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="44b8d-119">How does getSchedule compare with findMeetingTimes</span></span>

<span data-ttu-id="44b8d-120">Действие [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) похоже на **getSchedule** тем, что оба они считывают сведения о доступности и рабочем времени указанных пользователей и ресурсов.</span><span class="sxs-lookup"><span data-stu-id="44b8d-120">The [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) action is similar to **getSchedule** in that both read the free/busy status and working hours of specified users and resources.</span></span> <span data-ttu-id="44b8d-121">Эти два действиями отличаются по нескольким основным моментам.</span><span class="sxs-lookup"><span data-stu-id="44b8d-121">The two actions differ in a few major ways.</span></span>

### <a name="application"></a><span data-ttu-id="44b8d-122">Приложение</span><span class="sxs-lookup"><span data-stu-id="44b8d-122">Application</span></span>

<span data-ttu-id="44b8d-123">В действии **findMeetingTimes** применяется определенная бизнес-логика, чтобы предложить время и место собрания, например:</span><span class="sxs-lookup"><span data-stu-id="44b8d-123">**findMeetingTimes** applies certain business logic to suggest meeting times and locations, such as:</span></span>

- <span data-ttu-id="44b8d-124">необязательное или обязательное посещение каждой сущности;</span><span class="sxs-lookup"><span data-stu-id="44b8d-124">Optional or mandatory attendance of each entity</span></span>
- <span data-ttu-id="44b8d-125">тип запрошенного действия для времени суток;</span><span class="sxs-lookup"><span data-stu-id="44b8d-125">The nature of the requested activity for the time of the day</span></span>
- <span data-ttu-id="44b8d-126">необходимое минимальное присутствие для кворума на собрании.</span><span class="sxs-lookup"><span data-stu-id="44b8d-126">The minimum attendance required for a quorum for a meeting</span></span>

<span data-ttu-id="44b8d-127">Оно подходит для сценариев, зависящих от [оптимизации планирования встреч](findmeetingtimes-example.md).</span><span class="sxs-lookup"><span data-stu-id="44b8d-127">It is appropriate for scenarios that depend on [streamlining appointment booking](findmeetingtimes-example.md).</span></span>

<span data-ttu-id="44b8d-128">Действие **getSchedule** просто возвращает сведения о доступности с учетом существующих событий в каждом из запрошенных календарей для указанного промежутка времени, и предполагается, что остальное время в этом промежутке является свободным.</span><span class="sxs-lookup"><span data-stu-id="44b8d-128">**getSchedule** simply returns the free/busy status of existing events in each of the requested calendars for a given time period, and assumes the remaining time in that time period to be free.</span></span> <span data-ttu-id="44b8d-129">После этого вы можете применить бизнес-логику, чтобы использовать эти данные для завершения сценария.</span><span class="sxs-lookup"><span data-stu-id="44b8d-129">You would then apply further business logic to make use of this data to complete your scenario.</span></span>

### <a name="app-only-support"></a><span data-ttu-id="44b8d-130">Поддержка только для приложений</span><span class="sxs-lookup"><span data-stu-id="44b8d-130">App-only support</span></span>

<span data-ttu-id="44b8d-131">Действие **findmeetingtimes** поддерживает только делегированные сценарии, требующие входа пользователя в приложение.</span><span class="sxs-lookup"><span data-stu-id="44b8d-131">**findmeetingtimes** supports only delegated scenarios which require a user to have signed in to the app.</span></span> <span data-ttu-id="44b8d-132">Приложения могут считывать события только в календарях, доступных вошедшему в систему пользователю.</span><span class="sxs-lookup"><span data-stu-id="44b8d-132">The app can read events in only the calendars that the signed-in user can access.</span></span> <span data-ttu-id="44b8d-133">К ним могут относится календари, делегированные или предоставленные в совместное использование вошедшему пользователю другими пользователями.</span><span class="sxs-lookup"><span data-stu-id="44b8d-133">This can include calendars that other users have delegated or shared with the signed-in user.</span></span>

<span data-ttu-id="44b8d-134">Действие **getSchedule** поддерживает как сценарии делегирования, так и сценарии только для приложений.</span><span class="sxs-lookup"><span data-stu-id="44b8d-134">**getSchedule** supports both delegated and app-only scenarios.</span></span> <span data-ttu-id="44b8d-135">В последнем случае администратор разрешает приложению получать доступ ко всем календарям без входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="44b8d-135">In the latter, an administrator consents the app to access all calendars without a signed-in user.</span></span>

### <a name="permissions"></a><span data-ttu-id="44b8d-136">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44b8d-136">Permissions</span></span>
<span data-ttu-id="44b8d-137">Разрешения с минимальным уровнем привилегий, необходимые для действия **findmeetingtimes**, — Calendars.Read.Shared.</span><span class="sxs-lookup"><span data-stu-id="44b8d-137">The least privileged permissions required by **findmeetingtimes** is Calendars.Read.Shared.</span></span>

<span data-ttu-id="44b8d-138">Разрешение с минимальным уровнем привилегий, необходимое для действия **getSchedule**, — Calendars.Read.</span><span class="sxs-lookup"><span data-stu-id="44b8d-138">The least privileged permission required by **getSchedule** is Calendars.Read.</span></span> 

### <a name="version-support"></a><span data-ttu-id="44b8d-139">Поддержка версии</span><span class="sxs-lookup"><span data-stu-id="44b8d-139">Version support</span></span>

<span data-ttu-id="44b8d-140">Действия **findmeetingtimes** и **getSchedule** общедоступны и подходят для применения в рабочих приложениях.</span><span class="sxs-lookup"><span data-stu-id="44b8d-140">**findmeetingtimes** and **getSchedule** are both generally available and appropriate for use in production apps.</span></span>


## <a name="event-data-returned"></a><span data-ttu-id="44b8d-141">Возвращаемые данные события</span><span class="sxs-lookup"><span data-stu-id="44b8d-141">Event data returned</span></span>
<span data-ttu-id="44b8d-142">Разрешение с минимальным уровнем привилегий, необходимое действию **getSchedule** для получения приложением сведений о доступности, — Calendars.Read.</span><span class="sxs-lookup"><span data-stu-id="44b8d-142">The least privileged permission required by **getSchedule** for an app to get free/busy information is Calendars.Read.</span></span> <span data-ttu-id="44b8d-143">В зависимости от сценария приложения согласие может даваться вошедшим в систему пользователем или администратором.</span><span class="sxs-lookup"><span data-stu-id="44b8d-143">Depending on your app scenario, this can be consented by the signed-in user or administrator.</span></span>

<span data-ttu-id="44b8d-144">Если полученное разрешение позволяет приложению использовать действие **getSchedule** в календарях запрошенных пользователей через Outlook, запрошенный пользователь выбирает, какие данные события (при наличии) возвращает это действие **getSchedule**.</span><span class="sxs-lookup"><span data-stu-id="44b8d-144">While the consented permission lets an app use **getSchedule** on the requested users' calendars, through Outlook, the requested user controls which event data, if any, that **getSchedule** returns.</span></span> 

<span data-ttu-id="44b8d-145">Например, **getSchedule** может возвращать сведения о доступности и рабочем времени запрошенных пользователей или может просто вернуть свойства **subject**, **location** и **isPrivate** события, если:</span><span class="sxs-lookup"><span data-stu-id="44b8d-145">For example, **getSchedule** can return the free/busy status and working hours of the requested users, or it can also return the **subject**, **location**, and **isPrivate** properties of an event, provided that:</span></span>

- <span data-ttu-id="44b8d-146">Событие помечено низким уровнем конфиденциальности (`normal` или `personal`) И применяется одно или несколько следующих условий:</span><span class="sxs-lookup"><span data-stu-id="44b8d-146">The event is marked with low sensitivity level - `normal` or `personal` - AND one or more of the following conditions apply:</span></span>

  - <span data-ttu-id="44b8d-147">параметры запрошенного календаря пользователя разрешают вошедшим пользователям просматривать строки тем и расположения;</span><span class="sxs-lookup"><span data-stu-id="44b8d-147">The requested user’s calendar settings allow the signed-in user to view subject lines and locations</span></span>
  - <span data-ttu-id="44b8d-148">к запрошенному календарю предоставлен общий доступ вошедшему в систему пользователю;</span><span class="sxs-lookup"><span data-stu-id="44b8d-148">The requested user’s calendar is shared with the signed-in user</span></span>

<span data-ttu-id="44b8d-149">Эти условия применяются независимо от того, является ли пользователь, вошедший в систему, администратором в организации.</span><span class="sxs-lookup"><span data-stu-id="44b8d-149">These conditions apply regardless of whether the signed-in user is an administrator in the organization.</span></span> <span data-ttu-id="44b8d-150">Запрошенный пользователь управляет возвращаемыми данными события.</span><span class="sxs-lookup"><span data-stu-id="44b8d-150">The requested user has control over the event data returned.</span></span>

## <a name="time-zone-representation"></a><span data-ttu-id="44b8d-151">Представление часового пояса</span><span class="sxs-lookup"><span data-stu-id="44b8d-151">Time zone representation</span></span>
<span data-ttu-id="44b8d-152">По умолчанию время начала и окончания возвращаемых элементов расписания отображается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="44b8d-152">By default, the start and end times of the returned schedule items are represented in UTC.</span></span> <span data-ttu-id="44b8d-153">Вы можете использовать заголовок `Prefer`, чтобы указать соответствующий часовой пояс для приложения.</span><span class="sxs-lookup"><span data-stu-id="44b8d-153">You can use a `Prefer` header to specify a time zone appropriate for your app.</span></span> <span data-ttu-id="44b8d-154">Например:</span><span class="sxs-lookup"><span data-stu-id="44b8d-154">As an example:</span></span> 
``` http
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a><span data-ttu-id="44b8d-155">Ограничения и состояния ошибок</span><span class="sxs-lookup"><span data-stu-id="44b8d-155">Limits and error conditions</span></span>
<span data-ttu-id="44b8d-156">Необходимо учитывать следующие ограничения и состояние ошибки:</span><span class="sxs-lookup"><span data-stu-id="44b8d-156">Be aware of the following limits and error condition:</span></span>

- <span data-ttu-id="44b8d-157">**getSchedule** может поддерживать поиск сведений о доступности для 20 сущностей одновременно.</span><span class="sxs-lookup"><span data-stu-id="44b8d-157">**getSchedule** can support looking up free/busy information for up to 20 entities at once.</span></span> <span data-ttu-id="44b8d-158">Это ограничение относится к количеству пользователей, определенных по отдельности или в качестве участников списка рассылки, а также к количеству ресурсов.</span><span class="sxs-lookup"><span data-stu-id="44b8d-158">This limit applies to the number of users identified individually or as members of a distribution list, and to the number of resources as well.</span></span>
- <span data-ttu-id="44b8d-159">Период времени для поиска должен быть меньше 42 дней.</span><span class="sxs-lookup"><span data-stu-id="44b8d-159">The time period to look up must be less than 42 days.</span></span>
- <span data-ttu-id="44b8d-160">Если действие **getSchedule** не может определить указанного пользователя или ресурс, оно возвращает один элемент расписания и сообщает об ошибке.</span><span class="sxs-lookup"><span data-stu-id="44b8d-160">If **getSchedule** cannot identify a specified user or resource, it returns a single schedule item and indicates the error.</span></span> 


## <a name="see-also"></a><span data-ttu-id="44b8d-161">См. также</span><span class="sxs-lookup"><span data-stu-id="44b8d-161">See also</span></span>
- [<span data-ttu-id="44b8d-162">Справочник по разрешениям</span><span class="sxs-lookup"><span data-stu-id="44b8d-162">Permissions reference</span></span>](permissions-reference.md#calendars-permissions)
- [<span data-ttu-id="44b8d-163">Поиск времени для проведения собрания в календаре Outlook</span><span class="sxs-lookup"><span data-stu-id="44b8d-163">Find possible meeting times on the Outlook calendar</span></span>](findmeetingtimes-example.md)
