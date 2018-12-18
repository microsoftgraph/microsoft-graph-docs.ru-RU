---
title: Получение события
description: Получение объекта event.
author: dkershaw10
ms.openlocfilehash: 88a19af3e9f57e4b4c5856b56387136ccdd876de
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362414"
---
# <a name="get-event"></a><span data-ttu-id="02974-103">Получение события</span><span class="sxs-lookup"><span data-stu-id="02974-103">Get event</span></span>

> <span data-ttu-id="02974-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="02974-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02974-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02974-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="02974-106">Получение объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="02974-106">Get an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="02974-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02974-107">Permissions</span></span>
<span data-ttu-id="02974-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02974-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02974-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02974-110">Permission type</span></span>      | <span data-ttu-id="02974-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02974-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02974-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02974-112">Delegated (work or school account)</span></span> | <span data-ttu-id="02974-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02974-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="02974-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02974-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02974-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02974-115">Not supported.</span></span>    |
|<span data-ttu-id="02974-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02974-116">Application</span></span> | <span data-ttu-id="02974-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02974-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02974-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02974-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}
GET /groups/{id}/calendar/events/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02974-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="02974-119">Optional query parameters</span></span>
<span data-ttu-id="02974-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="02974-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02974-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02974-121">Request headers</span></span>
| <span data-ttu-id="02974-122">Имя</span><span class="sxs-lookup"><span data-stu-id="02974-122">Name</span></span>       | <span data-ttu-id="02974-123">Тип</span><span class="sxs-lookup"><span data-stu-id="02974-123">Type</span></span> | <span data-ttu-id="02974-124">Описание</span><span class="sxs-lookup"><span data-stu-id="02974-124">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="02974-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="02974-125">Authorization</span></span>  | <span data-ttu-id="02974-126">string</span><span class="sxs-lookup"><span data-stu-id="02974-126">string</span></span> | <span data-ttu-id="02974-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02974-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="02974-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="02974-129">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="02974-130">string</span><span class="sxs-lookup"><span data-stu-id="02974-130">string</span></span> | <span data-ttu-id="02974-131">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="02974-131">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="02974-132">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="02974-132">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="02974-133">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="02974-133">Optional.</span></span> |
| <span data-ttu-id="02974-134">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="02974-134">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="02974-135">string</span><span class="sxs-lookup"><span data-stu-id="02974-135">string</span></span> | <span data-ttu-id="02974-136">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="02974-136">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="02974-137">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="02974-137">Values can be "text" or "html".</span></span> <span data-ttu-id="02974-138">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="02974-138">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="02974-139">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="02974-139">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="02974-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="02974-140">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02974-141">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="02974-141">Request body</span></span>
<span data-ttu-id="02974-142">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="02974-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02974-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="02974-143">Response</span></span>
<span data-ttu-id="02974-144">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="02974-144">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02974-145">Пример</span><span class="sxs-lookup"><span data-stu-id="02974-145">Example</span></span>
#### <a name="request"></a><span data-ttu-id="02974-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="02974-146">Request</span></span>
<span data-ttu-id="02974-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02974-147">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_event"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="02974-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="02974-148">Response</span></span>
<span data-ttu-id="02974-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="02974-149">The following is an example of the response.</span></span>
><span data-ttu-id="02974-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02974-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1728

{
    "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==",
    "createdDateTime": "2017-07-31T18:58:31.011909Z",
    "lastModifiedDateTime": "2017-07-31T18:58:35.418473Z",
    "changeKey": "xPZF2y46pEiVBni87OnrpgAAAAAJTg==",
    "categories": [],
    "originalStartTimeZone": "Eastern Standard Time",
    "originalEndTimeZone": "Eastern Standard Time",
    "uid": "040000008200E00074C5B7101A82E00800000000B23663002F0AD301000000000000000010000000B7C936D4C2FEC749824EE24B2FD7DA62",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Continuing Education Sync",
    "bodyPreview": "Higher Education Planning.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "seriesMaster",
    "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA%3D%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Higher Education Planning.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2017-08-15T14:30:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2017-08-15T15:30:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "HR Taskforce / Benefits"
    },
    "recurrence": {
        "pattern": {
            "type": "weekly",
            "interval": 1,
            "month": 0,
            "dayOfMonth": 0,
            "daysOfWeek": [
                "tuesday",
                "thursday"
            ],
            "firstDayOfWeek": "sunday",
            "index": "first"
        },
        "range": {
            "type": "noEnd",
            "startDate": "2017-08-15",
            "endDate": "0001-01-01",
            "recurrenceTimeZone": "Eastern Standard Time",
            "numberOfOccurrences": 0
        }
    },
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "accepted",
                "time": "2017-07-31T18:58:34.3298022Z"
            },
            "emailAddress": {
                "name": "Lidia Holloway",
                "address": "LidiaH@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "HR Taskforce",
                "address": "HRTaskforce@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Diego Siciliani",
                "address": "DiegoS@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Johanna Lorenz",
                "address": "JohannaL@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "HR Taskforce",
            "address": "HRTaskforce@contoso.com"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
