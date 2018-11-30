---
title: 'календарь: getSchedule'
description: Получение сведений о доступности данных о доступности для коллекции пользователей, списки рассылки и ресурсы, для заданного периода времени.
ms.openlocfilehash: 5122cf34530f18f872e80863f259f348193d252e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076348"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="23e30-103">календарь: getSchedule</span><span class="sxs-lookup"><span data-stu-id="23e30-103">calendar: getSchedule</span></span>

> <span data-ttu-id="23e30-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="23e30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23e30-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23e30-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23e30-106">Получение сведений о доступности данных о доступности для коллекции пользователей, списки рассылки и ресурсы, для заданного периода времени.</span><span class="sxs-lookup"><span data-stu-id="23e30-106">Get the free/busy availability information for a collection of users, distributions lists, or resources, for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="23e30-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23e30-107">Permissions</span></span>
<span data-ttu-id="23e30-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23e30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23e30-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23e30-110">Permission type</span></span>      | <span data-ttu-id="23e30-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23e30-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23e30-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23e30-112">Delegated (work or school account)</span></span> | <span data-ttu-id="23e30-113">Calendar.Read Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23e30-113">Calendar.Read, Calendar.ReadWrite</span></span>    |
|<span data-ttu-id="23e30-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23e30-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23e30-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23e30-115">Not supported.</span></span> |
|<span data-ttu-id="23e30-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="23e30-116">Application</span></span> | <span data-ttu-id="23e30-117">Calendar.Read Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23e30-117">Calendar.Read, Calendar.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="23e30-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23e30-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="23e30-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23e30-119">Request headers</span></span>
| <span data-ttu-id="23e30-120">Имя</span><span class="sxs-lookup"><span data-stu-id="23e30-120">Name</span></span>       | <span data-ttu-id="23e30-121">Тип</span><span class="sxs-lookup"><span data-stu-id="23e30-121">Type</span></span> | <span data-ttu-id="23e30-122">Описание</span><span class="sxs-lookup"><span data-stu-id="23e30-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="23e30-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23e30-123">Authorization</span></span>  | <span data-ttu-id="23e30-124">string</span><span class="sxs-lookup"><span data-stu-id="23e30-124">string</span></span>  | <span data-ttu-id="23e30-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23e30-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="23e30-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="23e30-127">Content-Type</span></span>  | <span data-ttu-id="23e30-128">string</span><span class="sxs-lookup"><span data-stu-id="23e30-128">string</span></span> | <span data-ttu-id="23e30-129">Характер данные в теле сущности, который является приложение/json.</span><span class="sxs-lookup"><span data-stu-id="23e30-129">Nature of the data in the body of an entity, which is application/json.</span></span> <span data-ttu-id="23e30-130">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="23e30-130">Required.</span></span>  |
| <span data-ttu-id="23e30-131">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="23e30-131">Prefer: outlook.timezone</span></span> | <span data-ttu-id="23e30-132">string</span><span class="sxs-lookup"><span data-stu-id="23e30-132">string</span></span> | <span data-ttu-id="23e30-133">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="23e30-133">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="23e30-134">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="23e30-134">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="23e30-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="23e30-135">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23e30-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="23e30-136">Request body</span></span>
<span data-ttu-id="23e30-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="23e30-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="23e30-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="23e30-138">Property</span></span>     | <span data-ttu-id="23e30-139">Тип</span><span class="sxs-lookup"><span data-stu-id="23e30-139">Type</span></span>   |<span data-ttu-id="23e30-140">Description</span><span class="sxs-lookup"><span data-stu-id="23e30-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23e30-141">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="23e30-141">availabilityViewInterval</span></span>|<span data-ttu-id="23e30-142">String</span><span class="sxs-lookup"><span data-stu-id="23e30-142">String</span></span>|<span data-ttu-id="23e30-143">Представляет продолжительность промежуток времени в **availabilityView** в ответе.</span><span class="sxs-lookup"><span data-stu-id="23e30-143">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="23e30-144">Значение по умолчанию — 30 минут, как минимум — 6, максимум — 1440.</span><span class="sxs-lookup"><span data-stu-id="23e30-144">The default is 30 minutes, minimum is 6, maximum is 1440.</span></span> <span data-ttu-id="23e30-145">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="23e30-145">Optional.</span></span>|
|<span data-ttu-id="23e30-146">endTime</span><span class="sxs-lookup"><span data-stu-id="23e30-146">endTime</span></span>|[<span data-ttu-id="23e30-147">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="23e30-147">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="23e30-148">Даты, времени и часового пояса окончания периода.</span><span class="sxs-lookup"><span data-stu-id="23e30-148">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="23e30-149">расписания</span><span class="sxs-lookup"><span data-stu-id="23e30-149">schedules</span></span>|<span data-ttu-id="23e30-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="23e30-150">String collection</span></span>|<span data-ttu-id="23e30-151">Коллекция SMTP-адреса пользователей, списков рассылки и ресурсы для получения сведений о доступности для.</span><span class="sxs-lookup"><span data-stu-id="23e30-151">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="23e30-152">startTime</span><span class="sxs-lookup"><span data-stu-id="23e30-152">startTime</span></span>|[<span data-ttu-id="23e30-153">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="23e30-153">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="23e30-154">Даты, времени и часового пояса начала периода.</span><span class="sxs-lookup"><span data-stu-id="23e30-154">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="23e30-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="23e30-155">Response</span></span>

<span data-ttu-id="23e30-156">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [scheduleInformation](../resources/scheduleinformation.md) для каждого объекта в `schedules` параметр.</span><span class="sxs-lookup"><span data-stu-id="23e30-156">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="23e30-157">Пример</span><span class="sxs-lookup"><span data-stu-id="23e30-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23e30-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="23e30-158">Request</span></span>
<span data-ttu-id="23e30-159">Следующий пример возвращает сведения о доступности для двух пользователей для определенной даты, времени и часового пояса.</span><span class="sxs-lookup"><span data-stu-id="23e30-159">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/getschedule 
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{        
    "schedules": ["AdeleV@contoso.onmicrosoft.com", "AlexW@contoso.OnMicrosoft.com"],
    "startTime": {
        "dateTime": "2018-08-06T09:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "endTime": {
        "dateTime": "2018-08-06T18:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "availabilityViewInterval": "15"
}
```

##### <a name="response"></a><span data-ttu-id="23e30-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="23e30-160">Response</span></span>
<span data-ttu-id="23e30-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="23e30-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
            "scheduleId":"AdeleV@contoso.onmicrosoft.com",
            "availabilityView":"222222000022000000000000000000000000",
            "scheduleItems":[
                {
                    "isPrivate":false,
                    "status":"Busy",
                    "subject":"Admininstrators debrief",
                    "location":"Foyer",
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
                    "subject":"Lunch yoga",
                    "location":"Courtyard",
                    "start":{
                        "dateTime":"2018-08-06T11:30:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T12:00:00.0000000",
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
        },
        {
            "scheduleId":"AlexW@contoso.OnMicrosoft.com",
            "availabilityView":"111111002222222200000000000000000000",
            "scheduleItems":[
                {
                    "isPrivate":false,
                    "status":"Tentative",
                    "subject":"Admininstrators debrief",
                    "location":"Foyer",
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
                    "subject":"Q4 planning",
                    "location":"Big Bear",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar: getSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
