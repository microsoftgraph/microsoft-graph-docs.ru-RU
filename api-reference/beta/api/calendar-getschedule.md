---
title: 'calendar: getSchedule'
description: Получение сведений о доступности коллекции пользователей, списков рассылки или ресурсов для определенного периода времени.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9690412df1f4e1e27edec9d30555fb71f5d0c929
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317902"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="f9f6b-103">calendar: getSchedule</span><span class="sxs-lookup"><span data-stu-id="f9f6b-103">calendar: getSchedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9f6b-104">Получение сведений о доступности коллекции пользователей, списков рассылки или ресурсов (комнат или оборудования) для определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="f9f6b-104">Get the free/busy availability information for a collection of users, distributions lists, or resources (rooms or equipment) for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9f6b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9f6b-105">Permissions</span></span>
<span data-ttu-id="f9f6b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9f6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9f6b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9f6b-108">Permission type</span></span>      | <span data-ttu-id="f9f6b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9f6b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9f6b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9f6b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f9f6b-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9f6b-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f9f6b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9f6b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9f6b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9f6b-113">Not supported.</span></span> |
|<span data-ttu-id="f9f6b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9f6b-114">Application</span></span> | <span data-ttu-id="f9f6b-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9f6b-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9f6b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9f6b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="f9f6b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9f6b-117">Request headers</span></span>
| <span data-ttu-id="f9f6b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f9f6b-118">Name</span></span>       | <span data-ttu-id="f9f6b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f9f6b-119">Type</span></span> | <span data-ttu-id="f9f6b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f9f6b-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f9f6b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9f6b-121">Authorization</span></span>  | <span data-ttu-id="f9f6b-122">string</span><span class="sxs-lookup"><span data-stu-id="f9f6b-122">string</span></span>  | <span data-ttu-id="f9f6b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9f6b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9f6b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f9f6b-125">Content-Type</span></span>  | <span data-ttu-id="f9f6b-126">string</span><span class="sxs-lookup"><span data-stu-id="f9f6b-126">string</span></span> | <span data-ttu-id="f9f6b-127">Характер данных в тексте объекта (application/json).</span><span class="sxs-lookup"><span data-stu-id="f9f6b-127">Nature of the data in the body of an entity, which is application/json.</span></span> <span data-ttu-id="f9f6b-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9f6b-128">Required.</span></span>  |
| <span data-ttu-id="f9f6b-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="f9f6b-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="f9f6b-130">string</span><span class="sxs-lookup"><span data-stu-id="f9f6b-130">string</span></span> | <span data-ttu-id="f9f6b-131">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="f9f6b-131">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="f9f6b-132">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="f9f6b-132">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="f9f6b-133">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f9f6b-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9f6b-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9f6b-134">Request body</span></span>
<span data-ttu-id="f9f6b-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f9f6b-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f9f6b-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9f6b-136">Property</span></span>     | <span data-ttu-id="f9f6b-137">Тип</span><span class="sxs-lookup"><span data-stu-id="f9f6b-137">Type</span></span>   |<span data-ttu-id="f9f6b-138">Описание</span><span class="sxs-lookup"><span data-stu-id="f9f6b-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9f6b-139">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="f9f6b-139">availabilityViewInterval</span></span>|<span data-ttu-id="f9f6b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f9f6b-140">Int32</span></span>|<span data-ttu-id="f9f6b-141">Представляет длительность периода времени в свойстве **availabilityView** отклика.</span><span class="sxs-lookup"><span data-stu-id="f9f6b-141">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="f9f6b-142">Значение по умолчанию: 30 минут. Минимальное значение: 6. Максимальное значение: 1440.</span><span class="sxs-lookup"><span data-stu-id="f9f6b-142">The default is 30 minutes, minimum is 6, maximum is 1440.</span></span> <span data-ttu-id="f9f6b-143">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="f9f6b-143">Optional.</span></span>|
|<span data-ttu-id="f9f6b-144">endTime</span><span class="sxs-lookup"><span data-stu-id="f9f6b-144">endTime</span></span>|[<span data-ttu-id="f9f6b-145">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f9f6b-145">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="f9f6b-146">Дата, время и часовой пояс завершения периода.</span><span class="sxs-lookup"><span data-stu-id="f9f6b-146">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="f9f6b-147">schedules</span><span class="sxs-lookup"><span data-stu-id="f9f6b-147">schedules</span></span>|<span data-ttu-id="f9f6b-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f9f6b-148">String collection</span></span>|<span data-ttu-id="f9f6b-149">Коллекция SMTP-адресов пользователей, списков рассылки или ресурсов для получения сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="f9f6b-149">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="f9f6b-150">startTime</span><span class="sxs-lookup"><span data-stu-id="f9f6b-150">startTime</span></span>|[<span data-ttu-id="f9f6b-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f9f6b-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="f9f6b-152">Дата, время и часовой пояс начала периода.</span><span class="sxs-lookup"><span data-stu-id="f9f6b-152">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="f9f6b-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9f6b-153">Response</span></span>

<span data-ttu-id="f9f6b-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [scheduleInformation](../resources/scheduleinformation.md) для каждого объекта в параметре `schedules`.</span><span class="sxs-lookup"><span data-stu-id="f9f6b-154">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="f9f6b-155">Пример</span><span class="sxs-lookup"><span data-stu-id="f9f6b-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9f6b-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9f6b-156">Request</span></span>
<span data-ttu-id="f9f6b-157">В приведенном ниже примере возвращаются сведения о доступности двух пользователей для определенной даты, времени и часового пояса.</span><span class="sxs-lookup"><span data-stu-id="f9f6b-157">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f9f6b-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9f6b-158">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f9f6b-159">C#</span><span class="sxs-lookup"><span data-stu-id="f9f6b-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-getschedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9f6b-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9f6b-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-getschedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f9f6b-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9f6b-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-getschedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f9f6b-162">Java</span><span class="sxs-lookup"><span data-stu-id="f9f6b-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendar-getschedule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f9f6b-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9f6b-163">Response</span></span>
<span data-ttu-id="f9f6b-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9f6b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
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
