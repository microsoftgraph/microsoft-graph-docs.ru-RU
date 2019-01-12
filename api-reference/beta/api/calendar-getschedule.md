---
title: 'календарь: getSchedule'
description: Получение сведений о доступности данных о доступности для коллекции пользователей, списки рассылки и ресурсы, для заданного периода времени.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 9089489d2b26b3dd4cd56b950538a72ab533c933
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956957"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="6e6ef-103">календарь: getSchedule</span><span class="sxs-lookup"><span data-stu-id="6e6ef-103">calendar: getSchedule</span></span>

> <span data-ttu-id="6e6ef-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e6ef-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e6ef-106">Получение сведений о доступности данных о доступности для коллекции пользователей, списки рассылки и ресурсы, для заданного периода времени.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-106">Get the free/busy availability information for a collection of users, distributions lists, or resources, for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e6ef-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e6ef-107">Permissions</span></span>
<span data-ttu-id="6e6ef-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e6ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e6ef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e6ef-110">Permission type</span></span>      | <span data-ttu-id="6e6ef-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e6ef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e6ef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e6ef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6e6ef-113">Calendar.Read Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e6ef-113">Calendar.Read, Calendar.ReadWrite</span></span>    |
|<span data-ttu-id="6e6ef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e6ef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e6ef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-115">Not supported.</span></span> |
|<span data-ttu-id="6e6ef-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e6ef-116">Application</span></span> | <span data-ttu-id="6e6ef-117">Calendar.Read Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e6ef-117">Calendar.Read, Calendar.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e6ef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e6ef-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="6e6ef-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e6ef-119">Request headers</span></span>
| <span data-ttu-id="6e6ef-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6e6ef-120">Name</span></span>       | <span data-ttu-id="6e6ef-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6e6ef-121">Type</span></span> | <span data-ttu-id="6e6ef-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6e6ef-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6e6ef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e6ef-123">Authorization</span></span>  | <span data-ttu-id="6e6ef-124">строка</span><span class="sxs-lookup"><span data-stu-id="6e6ef-124">string</span></span>  | <span data-ttu-id="6e6ef-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6e6ef-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e6ef-127">Content-Type</span></span>  | <span data-ttu-id="6e6ef-128">строка</span><span class="sxs-lookup"><span data-stu-id="6e6ef-128">string</span></span> | <span data-ttu-id="6e6ef-129">Характер данные в теле сущности, который является приложение/json.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-129">Nature of the data in the body of an entity, which is application/json.</span></span> <span data-ttu-id="6e6ef-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-130">Required.</span></span>  |
| <span data-ttu-id="6e6ef-131">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="6e6ef-131">Prefer: outlook.timezone</span></span> | <span data-ttu-id="6e6ef-132">строка</span><span class="sxs-lookup"><span data-stu-id="6e6ef-132">string</span></span> | <span data-ttu-id="6e6ef-133">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-133">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="6e6ef-134">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-134">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="6e6ef-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-135">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e6ef-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6e6ef-136">Request body</span></span>
<span data-ttu-id="6e6ef-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6e6ef-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e6ef-138">Property</span></span>     | <span data-ttu-id="6e6ef-139">Тип</span><span class="sxs-lookup"><span data-stu-id="6e6ef-139">Type</span></span>   |<span data-ttu-id="6e6ef-140">Описание</span><span class="sxs-lookup"><span data-stu-id="6e6ef-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e6ef-141">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="6e6ef-141">availabilityViewInterval</span></span>|<span data-ttu-id="6e6ef-142">String</span><span class="sxs-lookup"><span data-stu-id="6e6ef-142">String</span></span>|<span data-ttu-id="6e6ef-143">Представляет продолжительность промежуток времени в **availabilityView** в ответе.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-143">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="6e6ef-144">Значение по умолчанию — 30 минут, как минимум — 6, максимум — 1440.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-144">The default is 30 minutes, minimum is 6, maximum is 1440.</span></span> <span data-ttu-id="6e6ef-145">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-145">Optional.</span></span>|
|<span data-ttu-id="6e6ef-146">endTime</span><span class="sxs-lookup"><span data-stu-id="6e6ef-146">endTime</span></span>|[<span data-ttu-id="6e6ef-147">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6e6ef-147">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="6e6ef-148">Даты, времени и часового пояса окончания периода.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-148">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="6e6ef-149">расписания</span><span class="sxs-lookup"><span data-stu-id="6e6ef-149">schedules</span></span>|<span data-ttu-id="6e6ef-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6e6ef-150">String collection</span></span>|<span data-ttu-id="6e6ef-151">Коллекция SMTP-адреса пользователей, списков рассылки и ресурсы для получения сведений о доступности для.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-151">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="6e6ef-152">startTime</span><span class="sxs-lookup"><span data-stu-id="6e6ef-152">startTime</span></span>|[<span data-ttu-id="6e6ef-153">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6e6ef-153">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="6e6ef-154">Даты, времени и часового пояса начала периода.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-154">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="6e6ef-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e6ef-155">Response</span></span>

<span data-ttu-id="6e6ef-156">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [scheduleInformation](../resources/scheduleinformation.md) для каждого объекта в `schedules` параметр.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-156">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="6e6ef-157">Пример</span><span class="sxs-lookup"><span data-stu-id="6e6ef-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e6ef-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e6ef-158">Request</span></span>
<span data-ttu-id="6e6ef-159">Следующий пример возвращает сведения о доступности для двух пользователей для определенной даты, времени и часового пояса.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-159">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>

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

##### <a name="response"></a><span data-ttu-id="6e6ef-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e6ef-160">Response</span></span>
<span data-ttu-id="6e6ef-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6e6ef-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
