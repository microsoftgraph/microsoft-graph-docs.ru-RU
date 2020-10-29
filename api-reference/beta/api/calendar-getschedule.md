---
title: 'calendar: getSchedule'
description: Получение сведений о доступности коллекции пользователей, списков рассылки или ресурсов для определенного периода времени.
localization_priority: Priority
author: tariq-sharif
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3d0d54eaf7ace80685f241b0e0cf191e85551f82
ms.sourcegitcommit: 70e09ebbf67f49a0c64ab7a275e751f8a68b8696
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/27/2020
ms.locfileid: "48771778"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="9bd68-103">calendar: getSchedule</span><span class="sxs-lookup"><span data-stu-id="9bd68-103">calendar: getSchedule</span></span>

<span data-ttu-id="9bd68-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bd68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bd68-105">Получение сведений о доступности коллекции пользователей, списков рассылки или ресурсов (комнат или оборудования) для определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="9bd68-105">Get the free/busy availability information for a collection of users, distributions lists, or resources (rooms or equipment) for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bd68-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9bd68-106">Permissions</span></span>
<span data-ttu-id="9bd68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bd68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bd68-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9bd68-109">Permission type</span></span>      | <span data-ttu-id="9bd68-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9bd68-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bd68-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9bd68-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9bd68-112">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9bd68-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="9bd68-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9bd68-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bd68-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bd68-114">Not supported.</span></span> |
|<span data-ttu-id="9bd68-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9bd68-115">Application</span></span> | <span data-ttu-id="9bd68-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9bd68-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9bd68-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9bd68-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="9bd68-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9bd68-118">Request headers</span></span>
| <span data-ttu-id="9bd68-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9bd68-119">Name</span></span>       | <span data-ttu-id="9bd68-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9bd68-120">Type</span></span> | <span data-ttu-id="9bd68-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9bd68-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9bd68-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bd68-122">Authorization</span></span>  | <span data-ttu-id="9bd68-123">string</span><span class="sxs-lookup"><span data-stu-id="9bd68-123">string</span></span>  | <span data-ttu-id="9bd68-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9bd68-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9bd68-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9bd68-126">Content-Type</span></span>  | <span data-ttu-id="9bd68-127">string</span><span class="sxs-lookup"><span data-stu-id="9bd68-127">string</span></span> | <span data-ttu-id="9bd68-128">Характер данных в тексте объекта (application/json).</span><span class="sxs-lookup"><span data-stu-id="9bd68-128">Nature of the data in the body of an entity, which is application/json.</span></span> <span data-ttu-id="9bd68-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9bd68-129">Required.</span></span>  |
| <span data-ttu-id="9bd68-130">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="9bd68-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="9bd68-131">string</span><span class="sxs-lookup"><span data-stu-id="9bd68-131">string</span></span> | <span data-ttu-id="9bd68-132">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="9bd68-132">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="9bd68-133">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="9bd68-133">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="9bd68-134">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9bd68-134">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9bd68-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9bd68-135">Request body</span></span>
<span data-ttu-id="9bd68-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9bd68-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9bd68-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="9bd68-137">Property</span></span>     | <span data-ttu-id="9bd68-138">Тип</span><span class="sxs-lookup"><span data-stu-id="9bd68-138">Type</span></span>   |<span data-ttu-id="9bd68-139">Описание</span><span class="sxs-lookup"><span data-stu-id="9bd68-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bd68-140">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="9bd68-140">availabilityViewInterval</span></span>|<span data-ttu-id="9bd68-141">Int32</span><span class="sxs-lookup"><span data-stu-id="9bd68-141">Int32</span></span>|<span data-ttu-id="9bd68-142">Представляет длительность периода времени в свойстве **availabilityView** отклика.</span><span class="sxs-lookup"><span data-stu-id="9bd68-142">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="9bd68-143">Значение по умолчанию: 30 минут. Минимальное значение: 5. Максимальное значение: 1440.</span><span class="sxs-lookup"><span data-stu-id="9bd68-143">The default is 30 minutes, minimum is 5, maximum is 1440.</span></span> <span data-ttu-id="9bd68-144">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="9bd68-144">Optional.</span></span>|
|<span data-ttu-id="9bd68-145">endTime</span><span class="sxs-lookup"><span data-stu-id="9bd68-145">endTime</span></span>|[<span data-ttu-id="9bd68-146">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9bd68-146">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="9bd68-147">Дата, время и часовой пояс завершения периода.</span><span class="sxs-lookup"><span data-stu-id="9bd68-147">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="9bd68-148">schedules</span><span class="sxs-lookup"><span data-stu-id="9bd68-148">schedules</span></span>|<span data-ttu-id="9bd68-149">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9bd68-149">String collection</span></span>|<span data-ttu-id="9bd68-150">Коллекция SMTP-адресов пользователей, списков рассылки или ресурсов для получения сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="9bd68-150">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="9bd68-151">startTime</span><span class="sxs-lookup"><span data-stu-id="9bd68-151">startTime</span></span>|[<span data-ttu-id="9bd68-152">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9bd68-152">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="9bd68-153">Дата, время и часовой пояс начала периода.</span><span class="sxs-lookup"><span data-stu-id="9bd68-153">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="9bd68-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bd68-154">Response</span></span>

<span data-ttu-id="9bd68-155">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [scheduleInformation](../resources/scheduleinformation.md) для каждого объекта в параметре `schedules`.</span><span class="sxs-lookup"><span data-stu-id="9bd68-155">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="9bd68-156">Пример</span><span class="sxs-lookup"><span data-stu-id="9bd68-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9bd68-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bd68-157">Request</span></span>
<span data-ttu-id="9bd68-158">В приведенном ниже примере возвращаются сведения о доступности двух пользователей для определенной даты, времени и часового пояса.</span><span class="sxs-lookup"><span data-stu-id="9bd68-158">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>


# <a name="http"></a>[<span data-ttu-id="9bd68-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bd68-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendar_getSchedule"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/getSchedule 
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
    "availabilityViewInterval": 60
}
```
# <a name="c"></a>[<span data-ttu-id="9bd68-160">C#</span><span class="sxs-lookup"><span data-stu-id="9bd68-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-getschedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9bd68-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bd68-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-getschedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9bd68-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bd68-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-getschedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9bd68-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bd68-163">Response</span></span>
<span data-ttu-id="9bd68-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9bd68-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


