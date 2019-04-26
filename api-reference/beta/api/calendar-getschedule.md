---
title: 'calendar: getSchedule'
description: Получение сведений о доступности коллекции пользователей, списков рассылки или ресурсов для определенного периода времени.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b7146bf264b2435694848062dc263d081bd23b01
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322392"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="da76f-103">calendar: getSchedule</span><span class="sxs-lookup"><span data-stu-id="da76f-103">calendar: getSchedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da76f-104">Получение сведений о доступности коллекции пользователей, списков рассылки или ресурсов (комнат или оборудования) для определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="da76f-104">Get the free/busy availability information for a collection of users, distributions lists, or resources (rooms or equipment) for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="da76f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da76f-105">Permissions</span></span>
<span data-ttu-id="da76f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da76f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da76f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da76f-108">Permission type</span></span>      | <span data-ttu-id="da76f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da76f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da76f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da76f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="da76f-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da76f-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="da76f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da76f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da76f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da76f-113">Not supported.</span></span> |
|<span data-ttu-id="da76f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da76f-114">Application</span></span> | <span data-ttu-id="da76f-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da76f-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="da76f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da76f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="da76f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da76f-117">Request headers</span></span>
| <span data-ttu-id="da76f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="da76f-118">Name</span></span>       | <span data-ttu-id="da76f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="da76f-119">Type</span></span> | <span data-ttu-id="da76f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="da76f-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="da76f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="da76f-121">Authorization</span></span>  | <span data-ttu-id="da76f-122">string</span><span class="sxs-lookup"><span data-stu-id="da76f-122">string</span></span>  | <span data-ttu-id="da76f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da76f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="da76f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da76f-125">Content-Type</span></span>  | <span data-ttu-id="da76f-126">string</span><span class="sxs-lookup"><span data-stu-id="da76f-126">string</span></span> | <span data-ttu-id="da76f-127">Характер данных в тексте объекта (application/json).</span><span class="sxs-lookup"><span data-stu-id="da76f-127">Nature of the data in the body of an entity, which is application/json.</span></span> <span data-ttu-id="da76f-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da76f-128">Required.</span></span>  |
| <span data-ttu-id="da76f-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="da76f-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="da76f-130">string</span><span class="sxs-lookup"><span data-stu-id="da76f-130">string</span></span> | <span data-ttu-id="da76f-131">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="da76f-131">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="da76f-132">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="da76f-132">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="da76f-133">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="da76f-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da76f-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da76f-134">Request body</span></span>
<span data-ttu-id="da76f-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="da76f-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="da76f-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="da76f-136">Property</span></span>     | <span data-ttu-id="da76f-137">Тип</span><span class="sxs-lookup"><span data-stu-id="da76f-137">Type</span></span>   |<span data-ttu-id="da76f-138">Описание</span><span class="sxs-lookup"><span data-stu-id="da76f-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da76f-139">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="da76f-139">availabilityViewInterval</span></span>|<span data-ttu-id="da76f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="da76f-140">Int32</span></span>|<span data-ttu-id="da76f-141">Представляет длительность периода времени в свойстве **availabilityView** отклика.</span><span class="sxs-lookup"><span data-stu-id="da76f-141">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="da76f-142">Значение по умолчанию: 30 минут. Минимальное значение: 6. Максимальное значение: 1440.</span><span class="sxs-lookup"><span data-stu-id="da76f-142">The default is 30 minutes, minimum is 6, maximum is 1440.</span></span> <span data-ttu-id="da76f-143">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="da76f-143">Optional.</span></span>|
|<span data-ttu-id="da76f-144">endTime</span><span class="sxs-lookup"><span data-stu-id="da76f-144">endTime</span></span>|[<span data-ttu-id="da76f-145">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="da76f-145">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="da76f-146">Дата, время и часовой пояс завершения периода.</span><span class="sxs-lookup"><span data-stu-id="da76f-146">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="da76f-147">schedules</span><span class="sxs-lookup"><span data-stu-id="da76f-147">schedules</span></span>|<span data-ttu-id="da76f-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="da76f-148">String collection</span></span>|<span data-ttu-id="da76f-149">Коллекция SMTP-адресов пользователей, списков рассылки или ресурсов для получения сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="da76f-149">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="da76f-150">startTime</span><span class="sxs-lookup"><span data-stu-id="da76f-150">startTime</span></span>|[<span data-ttu-id="da76f-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="da76f-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="da76f-152">Дата, время и часовой пояс начала периода.</span><span class="sxs-lookup"><span data-stu-id="da76f-152">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="da76f-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="da76f-153">Response</span></span>

<span data-ttu-id="da76f-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [scheduleInformation](../resources/scheduleinformation.md) для каждого объекта в параметре `schedules`.</span><span class="sxs-lookup"><span data-stu-id="da76f-154">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="da76f-155">Пример</span><span class="sxs-lookup"><span data-stu-id="da76f-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da76f-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="da76f-156">Request</span></span>
<span data-ttu-id="da76f-157">В приведенном ниже примере возвращаются сведения о доступности двух пользователей для определенной даты, времени и часового пояса.</span><span class="sxs-lookup"><span data-stu-id="da76f-157">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/getschedule 
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{        
    "schedules": ["adelev@contoso.onmicrosoft.com", "meganb@contoso.onmicrosoft.com"],
    "startTime": {
        "dateTime": "2019-03-15T09:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "endTime": {
        "dateTime": "2019-03-15T18:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "availabilityViewInterval": "60"
}
```

##### <a name="response"></a><span data-ttu-id="da76f-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="da76f-158">Response</span></span>
<span data-ttu-id="da76f-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da76f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value": [
        {
            "scheduleId": "adelev@contoso.onmicrosoft.com",
            "availabilityView": "000220000",
            "scheduleItems": [
                {
                    "isPrivate": false,
                    "status": "busy",
                    "subject": "Let's go for lunch",
                    "location": "Harry's Bar",
                    "start": {
                        "dateTime": "2019-03-15T12:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T14:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                }
            ],
            "workingHours": {
                "daysOfWeek": [
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime": "08:00:00.0000000",
                "endTime": "17:00:00.0000000",
                "timeZone": {
                    "name": "Pacific Standard Time"
                }
            }
        },
        {
            "scheduleId": "meganb@contoso.onmicrosoft.com",
            "availabilityView": "200220010",
            "scheduleItems": [
                {
                    "status": "busy",
                    "start": {
                        "dateTime": "2019-03-15T08:30:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T09:30:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                {
                    "status": "busy",
                    "start": {
                        "dateTime": "2019-03-15T12:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T14:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                {
                    "status": "tentative",
                    "start": {
                        "dateTime": "2019-03-15T12:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T13:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                {
                    "status": "busy",
                    "start": {
                        "dateTime": "2019-03-15T13:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T14:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                {
                    "status": "tentative",
                    "start": {
                        "dateTime": "2019-03-15T16:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T17:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                }
            ],
            "workingHours": {
                "daysOfWeek": [
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime": "08:00:00.0000000",
                "endTime": "17:00:00.0000000",
                "timeZone": {
                    "@odata.type": "#microsoft.graph.customTimeZone",
                    "bias": 480,
                    "name": "Customized Time Zone",
                    "standardOffset": {
                        "time": "02:00:00.0000000",
                        "dayOccurrence": 1,
                        "dayOfWeek": "sunday",
                        "month": 11,
                        "year": 0
                    },
                    "daylightOffset": {
                        "daylightBias": -60,
                        "time": "02:00:00.0000000",
                        "dayOccurrence": 2,
                        "dayOfWeek": "sunday",
                        "month": 3,
                        "year": 0
                    }
                }
            }
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "calendar: getSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
