---
title: 'event: snoozeReminder'
description: Отложить напоминание для события в календаре пользователя до нового времени.
author: angelgolfer-ms
ms.openlocfilehash: fc97ae4fffca5eeb054f708fe1dec8575382e6be
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305714"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="f29ce-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="f29ce-103">event: snoozeReminder</span></span>

> <span data-ttu-id="f29ce-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f29ce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f29ce-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f29ce-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f29ce-106">Отложить напоминание для [события](../resources/event.md) в [календаре](../resources/calendar.md) пользователя до нового времени.</span><span class="sxs-lookup"><span data-stu-id="f29ce-106">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="f29ce-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f29ce-107">Permissions</span></span>
<span data-ttu-id="f29ce-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f29ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f29ce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f29ce-110">Permission type</span></span>      | <span data-ttu-id="f29ce-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f29ce-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f29ce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f29ce-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f29ce-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f29ce-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f29ce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f29ce-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f29ce-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f29ce-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f29ce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f29ce-116">Application</span></span> | <span data-ttu-id="f29ce-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f29ce-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f29ce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f29ce-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="f29ce-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f29ce-119">Request headers</span></span>
| <span data-ttu-id="f29ce-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f29ce-120">Name</span></span>       | <span data-ttu-id="f29ce-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f29ce-121">Type</span></span> | <span data-ttu-id="f29ce-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f29ce-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f29ce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f29ce-123">Authorization</span></span>  | <span data-ttu-id="f29ce-124">string</span><span class="sxs-lookup"><span data-stu-id="f29ce-124">string</span></span>  | <span data-ttu-id="f29ce-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f29ce-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f29ce-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f29ce-127">Content-Type</span></span> | <span data-ttu-id="f29ce-128">string</span><span class="sxs-lookup"><span data-stu-id="f29ce-128">string</span></span>  | <span data-ttu-id="f29ce-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f29ce-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f29ce-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f29ce-131">Request body</span></span>
<span data-ttu-id="f29ce-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f29ce-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f29ce-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="f29ce-133">Parameter</span></span>    | <span data-ttu-id="f29ce-134">Тип</span><span class="sxs-lookup"><span data-stu-id="f29ce-134">Type</span></span>   |<span data-ttu-id="f29ce-135">Описание</span><span class="sxs-lookup"><span data-stu-id="f29ce-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f29ce-136">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="f29ce-136">newReminderTime</span></span>|<span data-ttu-id="f29ce-137">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f29ce-137">DateTimeTimeZone</span></span>|<span data-ttu-id="f29ce-138">Новые дата и время для активации напоминания.</span><span class="sxs-lookup"><span data-stu-id="f29ce-138">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="f29ce-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f29ce-139">Response</span></span>

<span data-ttu-id="f29ce-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f29ce-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f29ce-142">Пример</span><span class="sxs-lookup"><span data-stu-id="f29ce-142">Example</span></span>
<span data-ttu-id="f29ce-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f29ce-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f29ce-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="f29ce-144">Request</span></span>
<span data-ttu-id="f29ce-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f29ce-145">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f29ce-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="f29ce-146">Response</span></span>
<span data-ttu-id="f29ce-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f29ce-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
