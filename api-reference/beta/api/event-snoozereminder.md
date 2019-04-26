---
title: 'event: snoozeReminder'
description: ОтЛожить напоминание о событии в календаре пользователя до нового времени.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 57fea89c98bfc2e699d0625db4d40fbfd0f57578
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325148"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="c2e32-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="c2e32-103">event: snoozeReminder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2e32-104">ОтЛожить напоминание о [событии](../resources/event.md) в календаре [](../resources/calendar.md) пользователя до нового времени.</span><span class="sxs-lookup"><span data-stu-id="c2e32-104">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2e32-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2e32-105">Permissions</span></span>
<span data-ttu-id="c2e32-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2e32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2e32-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2e32-108">Permission type</span></span>      | <span data-ttu-id="c2e32-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2e32-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2e32-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2e32-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c2e32-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2e32-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c2e32-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2e32-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2e32-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2e32-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c2e32-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2e32-114">Application</span></span> | <span data-ttu-id="c2e32-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2e32-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2e32-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2e32-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="c2e32-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2e32-117">Request headers</span></span>
| <span data-ttu-id="c2e32-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c2e32-118">Name</span></span>       | <span data-ttu-id="c2e32-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c2e32-119">Type</span></span> | <span data-ttu-id="c2e32-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c2e32-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c2e32-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2e32-121">Authorization</span></span>  | <span data-ttu-id="c2e32-122">string</span><span class="sxs-lookup"><span data-stu-id="c2e32-122">string</span></span>  | <span data-ttu-id="c2e32-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2e32-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c2e32-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2e32-125">Content-Type</span></span> | <span data-ttu-id="c2e32-126">string</span><span class="sxs-lookup"><span data-stu-id="c2e32-126">string</span></span>  | <span data-ttu-id="c2e32-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2e32-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2e32-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2e32-129">Request body</span></span>
<span data-ttu-id="c2e32-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c2e32-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c2e32-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="c2e32-131">Parameter</span></span>    | <span data-ttu-id="c2e32-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c2e32-132">Type</span></span>   |<span data-ttu-id="c2e32-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c2e32-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2e32-134">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="c2e32-134">newReminderTime</span></span>|<span data-ttu-id="c2e32-135">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c2e32-135">DateTimeTimeZone</span></span>|<span data-ttu-id="c2e32-136">Новые дата и время для активации напоминания.</span><span class="sxs-lookup"><span data-stu-id="c2e32-136">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="c2e32-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2e32-137">Response</span></span>

<span data-ttu-id="c2e32-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c2e32-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2e32-140">Пример</span><span class="sxs-lookup"><span data-stu-id="c2e32-140">Example</span></span>
<span data-ttu-id="c2e32-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c2e32-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c2e32-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2e32-142">Request</span></span>
<span data-ttu-id="c2e32-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2e32-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c2e32-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2e32-144">Response</span></span>
<span data-ttu-id="c2e32-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c2e32-145">Here is an example of the response.</span></span>
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
  "suppressions": []
}
-->
