---
title: 'event: snoozeReminder'
description: Отложить напоминание о событии в календаре пользователя до нового времени.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6e9d2fc688c14ee28f3405c1adc94383df0d69a3
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419921"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="96ca7-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="96ca7-103">event: snoozeReminder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96ca7-104">Отложить напоминание о [событии](../resources/event.md) в календаре [](../resources/calendar.md) пользователя до нового времени.</span><span class="sxs-lookup"><span data-stu-id="96ca7-104">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="96ca7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96ca7-105">Permissions</span></span>
<span data-ttu-id="96ca7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96ca7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96ca7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96ca7-108">Permission type</span></span>      | <span data-ttu-id="96ca7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96ca7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96ca7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96ca7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96ca7-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96ca7-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="96ca7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96ca7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96ca7-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96ca7-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="96ca7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96ca7-114">Application</span></span> | <span data-ttu-id="96ca7-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96ca7-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="96ca7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96ca7-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="96ca7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96ca7-117">Request headers</span></span>
| <span data-ttu-id="96ca7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="96ca7-118">Name</span></span>       | <span data-ttu-id="96ca7-119">Тип</span><span class="sxs-lookup"><span data-stu-id="96ca7-119">Type</span></span> | <span data-ttu-id="96ca7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="96ca7-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="96ca7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="96ca7-121">Authorization</span></span>  | <span data-ttu-id="96ca7-122">string</span><span class="sxs-lookup"><span data-stu-id="96ca7-122">string</span></span>  | <span data-ttu-id="96ca7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96ca7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96ca7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="96ca7-125">Content-Type</span></span> | <span data-ttu-id="96ca7-126">string</span><span class="sxs-lookup"><span data-stu-id="96ca7-126">string</span></span>  | <span data-ttu-id="96ca7-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96ca7-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96ca7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96ca7-129">Request body</span></span>
<span data-ttu-id="96ca7-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="96ca7-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="96ca7-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="96ca7-131">Parameter</span></span>    | <span data-ttu-id="96ca7-132">Тип</span><span class="sxs-lookup"><span data-stu-id="96ca7-132">Type</span></span>   |<span data-ttu-id="96ca7-133">Описание</span><span class="sxs-lookup"><span data-stu-id="96ca7-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96ca7-134">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="96ca7-134">newReminderTime</span></span>|<span data-ttu-id="96ca7-135">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="96ca7-135">DateTimeTimeZone</span></span>|<span data-ttu-id="96ca7-136">Новые дата и время для активации напоминания.</span><span class="sxs-lookup"><span data-stu-id="96ca7-136">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="96ca7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="96ca7-137">Response</span></span>

<span data-ttu-id="96ca7-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="96ca7-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96ca7-140">Пример</span><span class="sxs-lookup"><span data-stu-id="96ca7-140">Example</span></span>
<span data-ttu-id="96ca7-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="96ca7-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="96ca7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="96ca7-142">Request</span></span>
<span data-ttu-id="96ca7-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96ca7-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="96ca7-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="96ca7-144">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="96ca7-145">C#</span><span class="sxs-lookup"><span data-stu-id="96ca7-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-snoozereminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96ca7-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96ca7-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-snoozereminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96ca7-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="96ca7-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-snoozereminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="96ca7-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="96ca7-148">Response</span></span>
<span data-ttu-id="96ca7-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="96ca7-149">Here is an example of the response.</span></span>
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
