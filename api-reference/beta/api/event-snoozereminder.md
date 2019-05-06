---
title: 'event: snoozeReminder'
description: Отложить напоминание о событии в календаре пользователя до нового времени.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 53643800e9148297be166e4f41deaa4eaf9ca542
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33586684"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="6c413-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="6c413-103">event: snoozeReminder</span></span>

<span data-ttu-id="6c413-104">Отложить напоминание о [событии](../resources/event.md) в календаре [](../resources/calendar.md) пользователя до нового времени.</span><span class="sxs-lookup"><span data-stu-id="6c413-104">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c413-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c413-105">Permissions</span></span>
<span data-ttu-id="6c413-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c413-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c413-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c413-108">Permission type</span></span>      | <span data-ttu-id="6c413-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c413-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c413-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c413-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6c413-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c413-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6c413-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c413-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c413-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c413-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6c413-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c413-114">Application</span></span> | <span data-ttu-id="6c413-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c413-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c413-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c413-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="6c413-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c413-117">Request headers</span></span>
| <span data-ttu-id="6c413-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6c413-118">Name</span></span>       | <span data-ttu-id="6c413-119">Тип</span><span class="sxs-lookup"><span data-stu-id="6c413-119">Type</span></span> | <span data-ttu-id="6c413-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6c413-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6c413-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c413-121">Authorization</span></span>  | <span data-ttu-id="6c413-122">string</span><span class="sxs-lookup"><span data-stu-id="6c413-122">string</span></span>  | <span data-ttu-id="6c413-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c413-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6c413-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c413-125">Content-Type</span></span> | <span data-ttu-id="6c413-126">string</span><span class="sxs-lookup"><span data-stu-id="6c413-126">string</span></span>  | <span data-ttu-id="6c413-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c413-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c413-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c413-129">Request body</span></span>
<span data-ttu-id="6c413-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6c413-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6c413-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="6c413-131">Parameter</span></span>    | <span data-ttu-id="6c413-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6c413-132">Type</span></span>   |<span data-ttu-id="6c413-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6c413-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c413-134">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="6c413-134">newReminderTime</span></span>|<span data-ttu-id="6c413-135">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6c413-135">DateTimeTimeZone</span></span>|<span data-ttu-id="6c413-136">Новые дата и время для активации напоминания.</span><span class="sxs-lookup"><span data-stu-id="6c413-136">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="6c413-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c413-137">Response</span></span>

<span data-ttu-id="6c413-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6c413-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c413-140">Пример</span><span class="sxs-lookup"><span data-stu-id="6c413-140">Example</span></span>
<span data-ttu-id="6c413-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6c413-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6c413-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c413-142">Request</span></span>
<span data-ttu-id="6c413-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c413-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "dateTime-value",
    "timeZone": "timeZone-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="6c413-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c413-144">Response</span></span>
<span data-ttu-id="6c413-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6c413-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6c413-146">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="6c413-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6c413-147">Языках</span><span class="sxs-lookup"><span data-stu-id="6c413-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/event_snoozereminder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c413-148">Язык</span><span class="sxs-lookup"><span data-stu-id="6c413-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/event_snoozereminder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/event-snoozereminder.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/event-snoozereminder.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
