---
title: Получение расписания доступности пользователей и ресурсов (предварительная версия)
description: Общим сценарием на рабочем месте или в учебном заведении является просмотр доступности пользователя для собрания или доступности команды, помещения или оборудования в некоторый период времени.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 18497a7178086fea25fb581fb2ba7c5c82fbe204
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981268"
---
# <a name="get-freebusy-schedule-of-users-and-resources-preview"></a><span data-ttu-id="399f5-103">Получение расписания доступности пользователей и ресурсов (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="399f5-103">Get free/busy schedule of users and resources (preview)</span></span>

<span data-ttu-id="399f5-104">Общим сценарием на рабочем месте или в учебном заведении является просмотр доступности пользователя для собрания или доступности команды, помещения или оборудования в некоторый период времени.</span><span class="sxs-lookup"><span data-stu-id="399f5-104">In a work or school setting, a common scenario is to see when a user is free for meeting, or to browse the availability of a team, room, or equipment for a time period.</span></span>

<span data-ttu-id="399f5-105">Действие [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) позволяет получить сведения о доступности одной или нескольких сущностей (пользователей, списков рассылки или ресурсов) для определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="399f5-105">The [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) action lets you get the availability information of one or more entities - users, distribution lists, or resources - for a specific period of time.</span></span> 

## <a name="example"></a><span data-ttu-id="399f5-106">Пример</span><span class="sxs-lookup"><span data-stu-id="399f5-106">Example</span></span>

<span data-ttu-id="399f5-107">Простой пример поиска расписания доступности коллеги (Алексея) в определенную дату с 9:00 до 18:00 по тихоокеанскому времени:</span><span class="sxs-lookup"><span data-stu-id="399f5-107">A simple example is to find the free/busy schedule of a coworker, Alex, on a specific day, from 9am to 6pm, Pacitfic Standard Time:</span></span>

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

<span data-ttu-id="399f5-108">**getSchedule** возвращает два элемента расписания, соответствующие имеющимся событиям в стандартном календаре Алексея, с указанием времени начала и окончания каждого события и сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="399f5-108">**getSchedule** returns two schedule items that match existing events in Alex' default calendar, showing the start and end times of each event and its free/busy status.</span></span> <span data-ttu-id="399f5-109">Можно считать, что в остальное время Алексей свободен в этом диапазоне дат и времени.</span><span class="sxs-lookup"><span data-stu-id="399f5-109">You can assume Alex is free for the remaining time in that date/time range.</span></span>

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

<span data-ttu-id="399f5-110">Кроме расписания доступности и рабочего времени Алексея, **getSchedule** также возвращает свойство **availabilityView**, являющееся объединенным представлением доступности Алексея в этот день.</span><span class="sxs-lookup"><span data-stu-id="399f5-110">Apart from the free/busy schedule and working hours of Alex, **getSchedule** also returns **availabilityView**, which is a merged view of Alex' availability for that day.</span></span> <span data-ttu-id="399f5-111">Объединенное представление — это строка, состоящая из интервалов времени, охватывающих этот день, в каждом из которых указывается доступность Алексея с использованием следующего стандарта:</span><span class="sxs-lookup"><span data-stu-id="399f5-111">The merged view is a string that consists of time slots covering that day, with each time slot indicating Alex' availability using the following convention:</span></span> 

- <span data-ttu-id="399f5-112">`0`= свободен</span><span class="sxs-lookup"><span data-stu-id="399f5-112">`0`= free</span></span>
- <span data-ttu-id="399f5-113">`1`= под вопросом</span><span class="sxs-lookup"><span data-stu-id="399f5-113">`1`= tentative</span></span>
- <span data-ttu-id="399f5-114">`2`= занят</span><span class="sxs-lookup"><span data-stu-id="399f5-114">`2`= busy</span></span>
- <span data-ttu-id="399f5-115">`3`= не на месте</span><span class="sxs-lookup"><span data-stu-id="399f5-115">`3`= out of office</span></span>
- <span data-ttu-id="399f5-116">`4`= работает в другом месте.</span><span class="sxs-lookup"><span data-stu-id="399f5-116">`4`= working elsewhere.</span></span> 

<span data-ttu-id="399f5-117">По умолчанию длина каждого интервала времени составляет 30 минут.</span><span class="sxs-lookup"><span data-stu-id="399f5-117">By default, the length of each time slot is 30 minutes.</span></span> <span data-ttu-id="399f5-118">В этом примере используется свойство **availabilityViewInterval** для изменения интервала времени до 15 минут.</span><span class="sxs-lookup"><span data-stu-id="399f5-118">This example uses the **availabilityViewInterval** property to customize the time slot to be 15 minutes.</span></span>

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a><span data-ttu-id="399f5-119">Отличие getSchedule от findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="399f5-119">How is getSchedule different from findMeetingTimes</span></span>

<span data-ttu-id="399f5-120">Действие [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) похоже на **getSchedule** тем, что оба они считывают сведения о доступности и рабочем времени указанных пользователей и ресурсов.</span><span class="sxs-lookup"><span data-stu-id="399f5-120">The [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) action is similar to **getSchedule** in that both read the free/busy status and working hours of specified users and resources.</span></span> <span data-ttu-id="399f5-121">Эти два действиями отличаются по нескольким основным моментам.</span><span class="sxs-lookup"><span data-stu-id="399f5-121">The two actions differ in a few major ways.</span></span>

### <a name="application"></a><span data-ttu-id="399f5-122">Приложение</span><span class="sxs-lookup"><span data-stu-id="399f5-122">Application</span></span>

<span data-ttu-id="399f5-123">В действии **findMeetingTimes** применяется определенная бизнес-логика, чтобы предложить время и место собрания, например:</span><span class="sxs-lookup"><span data-stu-id="399f5-123">**findMeetingTimes** applies certain business logic to suggest meeting times and locations, such as:</span></span>

- <span data-ttu-id="399f5-124">необязательное или обязательное посещение каждой сущности;</span><span class="sxs-lookup"><span data-stu-id="399f5-124">Optional or mandatory attendance of each entity</span></span>
- <span data-ttu-id="399f5-125">тип запрошенного действия для времени суток;</span><span class="sxs-lookup"><span data-stu-id="399f5-125">The nature of the requested activity for the time of the day</span></span>
- <span data-ttu-id="399f5-126">необходимое минимальное присутствие для кворума на собрании.</span><span class="sxs-lookup"><span data-stu-id="399f5-126">The minimum attendance required for a quorum for a meeting</span></span>

<span data-ttu-id="399f5-127">Оно подходит для сценариев, зависящих от [оптимизации планирования встреч](findmeetingtimes-example.md).</span><span class="sxs-lookup"><span data-stu-id="399f5-127">It is appropriate for scenarios that depend on [streamlining appointment booking](findmeetingtimes-example.md).</span></span>

<span data-ttu-id="399f5-128">Действие **getSchedule** просто возвращает сведения о доступности с учетом существующих событий в каждом из запрошенных календарей для указанного промежутка времени, и предполагается, что остальное время в этом промежутке является свободным.</span><span class="sxs-lookup"><span data-stu-id="399f5-128">**getSchedule** simply returns the free/busy status of existing events in each of the requested calendars for a given time period, and assumes the remaining time in that time period tp be free.</span></span> <span data-ttu-id="399f5-129">После этого вы можете применить бизнес-логику, чтобы использовать эти данные для завершения сценария.</span><span class="sxs-lookup"><span data-stu-id="399f5-129">You would then apply further business logic to make use of this data to complete your scenario.</span></span>

### <a name="app-only-support"></a><span data-ttu-id="399f5-130">Поддержка только для приложений</span><span class="sxs-lookup"><span data-stu-id="399f5-130">App-only support</span></span>

<span data-ttu-id="399f5-131">Действие **findmeetingtimes** поддерживает только делегированные сценарии, требующие входа пользователя в приложение.</span><span class="sxs-lookup"><span data-stu-id="399f5-131">**findmeetingtimes** supports only delegated scenarios which require a user to have signed in to the app.</span></span> <span data-ttu-id="399f5-132">Приложения могут считывать события только в календарях, доступных вошедшему в систему пользователю.</span><span class="sxs-lookup"><span data-stu-id="399f5-132">The app can read events in only the calendars that the signed-in user can access.</span></span> <span data-ttu-id="399f5-133">К ним могут относится календари, делегированные или предоставленные в совместное использование вошедшему пользователю другими пользователями.</span><span class="sxs-lookup"><span data-stu-id="399f5-133">This can include calendars that other users have delegated or shared with the signed-in user.</span></span>

<span data-ttu-id="399f5-134">Действие **getSchedule** поддерживает как сценарии делегирования, так и сценарии только для приложений.</span><span class="sxs-lookup"><span data-stu-id="399f5-134">**getSchedule** supports both delegated and app-only scenarios.</span></span> <span data-ttu-id="399f5-135">В последнем случае администратор разрешает приложению получать доступ ко всем календарям без входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="399f5-135">In the latter, an administrator consents the app to access all calendars without a signed-in user.</span></span>


### <a name="version-support"></a><span data-ttu-id="399f5-136">Поддержка версии</span><span class="sxs-lookup"><span data-stu-id="399f5-136">Version support</span></span>

<span data-ttu-id="399f5-137">Действие **findmeetingtimes** общедоступно для всех приложений.</span><span class="sxs-lookup"><span data-stu-id="399f5-137">**findmeetingtimes** is generally available for all apps.</span></span> 

<span data-ttu-id="399f5-138">Действие **getSchedule** в настоящее время доступно [в состоянии предварительной версии](versioning-and-support.md#beta-version) и поэтому не подходит для применения в рабочих приложениях.</span><span class="sxs-lookup"><span data-stu-id="399f5-138">**getSchedule** is currently available [in preview status](versioning-and-support.md#beta-version), and therefore is not appropriate for use in production apps.</span></span>


## <a name="permissions"></a><span data-ttu-id="399f5-139">Разрешения</span><span class="sxs-lookup"><span data-stu-id="399f5-139">Permissions</span></span>
<span data-ttu-id="399f5-140">Разрешение с минимальным уровнем привилегий, необходимое для получения сведений о доступности, — Calendar.Read.</span><span class="sxs-lookup"><span data-stu-id="399f5-140">The least privileged permission you need to get free/busy information is Calendar.Read.</span></span> <span data-ttu-id="399f5-141">В зависимости от сценария приложения согласие может даваться вошедшим в систему пользователем или администратором.</span><span class="sxs-lookup"><span data-stu-id="399f5-141">Depending on your app scenario, this can be consented by the signed-in user or administrator.</span></span>
<span data-ttu-id="399f5-142">Кроме сведений о доступности и рабочем времени запрошенных сущностей, **getSchedule** может возвращать тему и место события, если:</span><span class="sxs-lookup"><span data-stu-id="399f5-142">Other than the free/busy status and working hours of requested entities, **getSchedule** can also return the subject and location of an event, provided that:</span></span>

- <span data-ttu-id="399f5-143">Событие помечено низким уровнем конфиденциальности (`normal` или `personal`) И применяется одно или несколько следующих условий:</span><span class="sxs-lookup"><span data-stu-id="399f5-143">If the event is marked with low sensitivity level - `normal` or `personal` AND one or more of the following conditions applies:</span></span>

- <span data-ttu-id="399f5-144">параметры запрошенного календаря пользователя разрешают всем пользователям в организации просматривать названия и расположения;</span><span class="sxs-lookup"><span data-stu-id="399f5-144">The requested user’s calendar settings allow all the users in the organization to view titles and locations</span></span>
- <span data-ttu-id="399f5-145">к запрошенному календарю предоставлен общий доступ вошедшему в систему пользователю;</span><span class="sxs-lookup"><span data-stu-id="399f5-145">The requested user’s calendar is shared with the signed-in user</span></span>
- <span data-ttu-id="399f5-146">вошедший в систему пользователь является администратором той же организации, что и запрошенный пользователь.</span><span class="sxs-lookup"><span data-stu-id="399f5-146">The signed-in user is an administrator of the same organization as the requested user.</span></span>

## <a name="time-zone-representation"></a><span data-ttu-id="399f5-147">Представление часового пояса</span><span class="sxs-lookup"><span data-stu-id="399f5-147">Time zone representation</span></span>
<span data-ttu-id="399f5-148">По умолчанию время начала и окончания возвращаемых элементов расписания отображается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="399f5-148">By default, the start and end times of the returned schedule items are represented in UTC.</span></span> <span data-ttu-id="399f5-149">Вы можете использовать заголовок `Prefer`, чтобы указать соответствующий часовой пояс для приложения.</span><span class="sxs-lookup"><span data-stu-id="399f5-149">You can use a `Prefer` header to specify a time zone appropriate for your app.</span></span> <span data-ttu-id="399f5-150">Например:</span><span class="sxs-lookup"><span data-stu-id="399f5-150">As an example:</span></span> 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a><span data-ttu-id="399f5-151">Ограничения и состояния ошибок</span><span class="sxs-lookup"><span data-stu-id="399f5-151">Limits and error conditions</span></span>
<span data-ttu-id="399f5-152">Необходимо учитывать следующие ограничения и состояние ошибки:</span><span class="sxs-lookup"><span data-stu-id="399f5-152">Be aware of the following limits and error condition:</span></span>

- <span data-ttu-id="399f5-153">**getSchedule** может поддерживать поиск сведений о доступности для 20 сущностей одновременно.</span><span class="sxs-lookup"><span data-stu-id="399f5-153">**getSchedule** can support looking up free/busy information for up to 20 entities at once.</span></span> <span data-ttu-id="399f5-154">Это ограничение относится к количеству пользователей, определенных по отдельности или в качестве участников списка рассылки, а также к количеству ресурсов.</span><span class="sxs-lookup"><span data-stu-id="399f5-154">This limit applies to the number of users identified individually or as members of a distribution list, and to the number of resources as well.</span></span>
- <span data-ttu-id="399f5-155">Период времени для поиска должен быть меньше 42 дней.</span><span class="sxs-lookup"><span data-stu-id="399f5-155">The time period to look up must be less than 42 days.</span></span>
- <span data-ttu-id="399f5-156">Если действие **getSchedule** не может определить указанного пользователя или ресурс, оно возвращает один элемент расписания и сообщает об ошибке.</span><span class="sxs-lookup"><span data-stu-id="399f5-156">If **getSchedule** cannot identify a specified user or resource, it returns a single schedule item and indicates the error.</span></span> 

## <a name="see-also"></a><span data-ttu-id="399f5-157">См. также</span><span class="sxs-lookup"><span data-stu-id="399f5-157">See also</span></span>
- [<span data-ttu-id="399f5-158">Справочник по разрешениям</span><span class="sxs-lookup"><span data-stu-id="399f5-158">Permissions reference</span></span>](permissions-reference.md#calendars-permissions)
- [<span data-ttu-id="399f5-159">Поиск времени для проведения собрания в календаре Outlook</span><span class="sxs-lookup"><span data-stu-id="399f5-159">Find possible meeting times on the Outlook calendar</span></span>](findmeetingtimes-example.md)
