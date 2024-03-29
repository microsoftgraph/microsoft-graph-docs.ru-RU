---
title: Получить график занятости пользователей и ресурсов календаря Outlook
description: Используйте действие getSchedule, чтобы получить информацию о доступности одного или нескольких пользователей, списков рассылки или ресурсов за определенный период времени.
author: tariq-sharif
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: ac44432fee2b324a399a0411e92041f0eeaab0e4
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697640"
---
# <a name="get-freebusy-schedule-of-outlook-calendar-users-and-resources"></a>Получить график занятости пользователей и ресурсов календаря Outlook

Общим сценарием на рабочем месте или в учебном заведении является просмотр доступности пользователя для собрания или доступности команды, помещения или оборудования в некоторый период времени.

Действие [getSchedule](/graph/api/calendar-getschedule) позволяет получить сведения о доступности одной или нескольких сущностей (пользователей, списков рассылки или ресурсов) для определенного периода времени. 

## <a name="example"></a>Пример

Простой пример — поиск расписания доступности сотрудника Игоря в определенный день с 9:00 до 18:00 по тихоокеанскому времени:

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

**getSchedule** возвращает два элемента расписания, соответствующие имеющимся событиям в стандартном календаре Алексея, с указанием времени начала и окончания каждого события и сведений о доступности. Можно считать, что в остальное время Алексей свободен в этом диапазоне дат и времени.

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

Кроме расписания доступности и рабочего времени Алексея, **getSchedule** также возвращает свойство **availabilityView**, являющееся объединенным представлением доступности Алексея в этот день. Объединенное представление — это строка, состоящая из интервалов времени, охватывающих этот день, в каждом из которых указывается доступность Алексея с использованием следующего стандарта: 

- `0`= свободен
- `1`= под вопросом
- `2`= занят
- `3`= не на месте
- `4`= работает в другом месте. 

По умолчанию длина каждого интервала времени составляет 30 минут. В этом примере используется свойство **availabilityViewInterval** для изменения интервала времени до 15 минут.

## <a name="how-does-getschedule-compare-with-findmeetingtimes"></a>Сравнение getSchedule с findMeetingTimes

Действие [findMeetingTimes](/graph/api/user-findmeetingtimes) похоже на **getSchedule** тем, что оба они считывают сведения о доступности и рабочем времени указанных пользователей и ресурсов. Эти два действиями отличаются по нескольким основным моментам.

### <a name="application"></a>Приложение

В действии **findMeetingTimes** применяется определенная бизнес-логика, чтобы предложить время и место собрания, например:

- необязательное или обязательное посещение каждой сущности;
- тип запрошенного действия для времени суток;
- необходимое минимальное присутствие для кворума на собрании.

Оно подходит для сценариев, зависящих от [оптимизации планирования встреч](findmeetingtimes-example.md).

Действие **getSchedule** просто возвращает сведения о доступности с учетом существующих событий в каждом из запрошенных календарей для указанного промежутка времени, и предполагается, что остальное время в этом промежутке является свободным. После этого вы можете применить бизнес-логику, чтобы использовать эти данные для завершения сценария.

### <a name="app-only-support"></a>Поддержка только для приложений

Действие **findmeetingtimes** поддерживает только делегированные сценарии, требующие входа пользователя в приложение. Приложения могут считывать события только в календарях, доступных вошедшему в систему пользователю. К ним могут относится календари, делегированные или предоставленные в совместное использование вошедшему пользователю другими пользователями.

Действие **getSchedule** поддерживает как сценарии делегирования, так и сценарии только для приложений. В последнем случае администратор разрешает приложению получать доступ ко всем календарям без входа пользователя.

### <a name="permissions"></a>Разрешения
Разрешения с минимальным уровнем привилегий, необходимые для действия **findmeetingtimes**, — Calendars.Read.Shared.

Разрешение с минимальным уровнем привилегий, необходимое для действия **getSchedule**, — Calendars.Read. 

### <a name="version-support"></a>Поддержка версии

Действия **findmeetingtimes** и **getSchedule** общедоступны и подходят для применения в рабочих приложениях.


## <a name="event-data-returned"></a>Возвращаемые данные события
Разрешение с минимальным уровнем привилегий, необходимое действию **getSchedule** для получения приложением сведений о доступности, — Calendars.Read. В зависимости от сценария приложения согласие может даваться вошедшим в систему пользователем или администратором.

Если полученное разрешение позволяет приложению использовать действие **getSchedule** в календарях запрошенных пользователей через Outlook, запрошенный пользователь выбирает, какие данные события (при наличии) возвращает это действие **getSchedule**. 

Например, **getSchedule** может возвращать сведения о доступности и рабочем времени запрошенных пользователей или может просто вернуть свойства **subject**, **location** и **isPrivate** события, если:

- Событие помечено низким уровнем конфиденциальности (`normal` или `personal`) И применяется одно или несколько следующих условий:

  - параметры запрошенного календаря пользователя разрешают вошедшим пользователям просматривать строки тем и расположения;
  - к запрошенному календарю предоставлен общий доступ вошедшему в систему пользователю;

Эти условия применяются независимо от того, является ли пользователь, вошедший в систему, администратором в организации. Запрошенный пользователь управляет возвращаемыми данными события.

## <a name="time-zone-representation"></a>Представление часового пояса
По умолчанию время начала и окончания возвращаемых элементов расписания отображается в формате UTC. Вы можете использовать заголовок `Prefer`, чтобы указать соответствующий часовой пояс для приложения. Например: 
``` http
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a>Ограничения и состояния ошибок
Необходимо учитывать следующие ограничения и состояние ошибки:

- **getSchedule** может поддерживать поиск сведений о доступности для 20 сущностей одновременно. Это ограничение относится к количеству пользователей, определенных по отдельности или в качестве участников списка рассылки, а также к количеству ресурсов.
- Период времени для поиска должен быть меньше 42 дней.
- Если действие **getSchedule** не может определить указанного пользователя или ресурс, оно возвращает один элемент расписания и сообщает об ошибке. 


## <a name="see-also"></a>См. также
- [Справочник по разрешениям](permissions-reference.md#calendars-permissions)
- [Поиск времени для проведения собрания в календаре Outlook](findmeetingtimes-example.md)
