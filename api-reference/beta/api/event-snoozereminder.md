---
title: 'event: snoozeReminder'
description: Отложить напоминание для события в календаре пользователя до нового времени.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 15cd83b1af1b68088bd9a789fdeacc88f7d7b3e4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528734"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="0ab02-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="0ab02-103">event: snoozeReminder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ab02-104">Отложить напоминание для [события](../resources/event.md) в [календаре](../resources/calendar.md) пользователя до нового времени.</span><span class="sxs-lookup"><span data-stu-id="0ab02-104">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ab02-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ab02-105">Permissions</span></span>
<span data-ttu-id="0ab02-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ab02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ab02-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ab02-108">Permission type</span></span>      | <span data-ttu-id="0ab02-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ab02-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ab02-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ab02-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ab02-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ab02-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0ab02-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ab02-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ab02-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ab02-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0ab02-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ab02-114">Application</span></span> | <span data-ttu-id="0ab02-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ab02-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ab02-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ab02-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/events/{id}/snoozeReminder

POST /me/calendar/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/snoozeReminder

POST /me/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroup/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
```
## <a name="request-headers"></a><span data-ttu-id="0ab02-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ab02-117">Request headers</span></span>
| <span data-ttu-id="0ab02-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0ab02-118">Name</span></span>       | <span data-ttu-id="0ab02-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0ab02-119">Type</span></span> | <span data-ttu-id="0ab02-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0ab02-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0ab02-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ab02-121">Authorization</span></span>  | <span data-ttu-id="0ab02-122">string</span><span class="sxs-lookup"><span data-stu-id="0ab02-122">string</span></span>  | <span data-ttu-id="0ab02-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ab02-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ab02-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0ab02-125">Content-Type</span></span> | <span data-ttu-id="0ab02-126">string</span><span class="sxs-lookup"><span data-stu-id="0ab02-126">string</span></span>  | <span data-ttu-id="0ab02-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ab02-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ab02-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ab02-129">Request body</span></span>
<span data-ttu-id="0ab02-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0ab02-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0ab02-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="0ab02-131">Parameter</span></span>    | <span data-ttu-id="0ab02-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0ab02-132">Type</span></span>   |<span data-ttu-id="0ab02-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0ab02-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ab02-134">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="0ab02-134">newReminderTime</span></span>|<span data-ttu-id="0ab02-135">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0ab02-135">DateTimeTimeZone</span></span>|<span data-ttu-id="0ab02-136">Новые дата и время для активации напоминания.</span><span class="sxs-lookup"><span data-stu-id="0ab02-136">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="0ab02-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ab02-137">Response</span></span>

<span data-ttu-id="0ab02-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0ab02-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ab02-140">Пример</span><span class="sxs-lookup"><span data-stu-id="0ab02-140">Example</span></span>
<span data-ttu-id="0ab02-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0ab02-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0ab02-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ab02-142">Request</span></span>
<span data-ttu-id="0ab02-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ab02-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "2016-10-19T10:37:00Z",
    "timeZone": "timeZone-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="0ab02-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ab02-144">Response</span></span>
<span data-ttu-id="0ab02-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0ab02-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-snoozereminder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
