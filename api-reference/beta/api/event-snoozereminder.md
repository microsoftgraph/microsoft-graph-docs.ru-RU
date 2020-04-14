---
title: 'event: snoozeReminder'
description: Отложить напоминание о событии в календаре пользователя до нового времени.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9082ce27e232e06db7867385942e409dfbbe727d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43365049"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="d7600-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="d7600-103">event: snoozeReminder</span></span>

<span data-ttu-id="d7600-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7600-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7600-105">Отложить напоминание о [событии](../resources/event.md) в [календаре](../resources/calendar.md) пользователя до нового времени.</span><span class="sxs-lookup"><span data-stu-id="d7600-105">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7600-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7600-106">Permissions</span></span>
<span data-ttu-id="d7600-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7600-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7600-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7600-109">Permission type</span></span>      | <span data-ttu-id="d7600-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7600-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7600-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7600-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d7600-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7600-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d7600-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7600-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7600-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7600-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d7600-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7600-115">Application</span></span> | <span data-ttu-id="d7600-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7600-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7600-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7600-117">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="d7600-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7600-118">Request headers</span></span>
| <span data-ttu-id="d7600-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d7600-119">Name</span></span>       | <span data-ttu-id="d7600-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d7600-120">Type</span></span> | <span data-ttu-id="d7600-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d7600-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d7600-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7600-122">Authorization</span></span>  | <span data-ttu-id="d7600-123">string</span><span class="sxs-lookup"><span data-stu-id="d7600-123">string</span></span>  | <span data-ttu-id="d7600-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7600-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7600-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7600-126">Content-Type</span></span> | <span data-ttu-id="d7600-127">string</span><span class="sxs-lookup"><span data-stu-id="d7600-127">string</span></span>  | <span data-ttu-id="d7600-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7600-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7600-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7600-130">Request body</span></span>
<span data-ttu-id="d7600-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d7600-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d7600-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="d7600-132">Parameter</span></span>    | <span data-ttu-id="d7600-133">Тип</span><span class="sxs-lookup"><span data-stu-id="d7600-133">Type</span></span>   |<span data-ttu-id="d7600-134">Описание</span><span class="sxs-lookup"><span data-stu-id="d7600-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7600-135">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="d7600-135">newReminderTime</span></span>|<span data-ttu-id="d7600-136">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d7600-136">DateTimeTimeZone</span></span>|<span data-ttu-id="d7600-137">Новые дата и время для активации напоминания.</span><span class="sxs-lookup"><span data-stu-id="d7600-137">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="d7600-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7600-138">Response</span></span>

<span data-ttu-id="d7600-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d7600-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7600-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d7600-141">Example</span></span>
<span data-ttu-id="d7600-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d7600-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d7600-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7600-143">Request</span></span>
<span data-ttu-id="d7600-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7600-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d7600-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7600-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d7600-146">C#</span><span class="sxs-lookup"><span data-stu-id="d7600-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-snoozereminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7600-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7600-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-snoozereminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7600-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7600-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-snoozereminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d7600-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7600-149">Response</span></span>
<span data-ttu-id="d7600-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d7600-150">Here is an example of the response.</span></span>
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
  ]
}
-->
