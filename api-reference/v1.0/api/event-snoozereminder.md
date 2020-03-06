---
title: 'event: snoozeReminder'
description: Отложить напоминание о событии в календаре пользователя до нового времени.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: adb0b50231ceb64eb9c11d871adbbbe9a7bdee4a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517336"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="cba38-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="cba38-103">event: snoozeReminder</span></span>

<span data-ttu-id="cba38-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cba38-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cba38-105">Отложить напоминание о [событии](../resources/event.md) в [календаре](../resources/calendar.md) пользователя до нового времени.</span><span class="sxs-lookup"><span data-stu-id="cba38-105">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="cba38-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cba38-106">Permissions</span></span>
<span data-ttu-id="cba38-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cba38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cba38-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cba38-109">Permission type</span></span>      | <span data-ttu-id="cba38-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cba38-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cba38-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cba38-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cba38-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cba38-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cba38-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cba38-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cba38-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cba38-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cba38-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cba38-115">Application</span></span> | <span data-ttu-id="cba38-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cba38-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cba38-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cba38-117">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="cba38-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cba38-118">Request headers</span></span>
| <span data-ttu-id="cba38-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cba38-119">Name</span></span>       | <span data-ttu-id="cba38-120">Тип</span><span class="sxs-lookup"><span data-stu-id="cba38-120">Type</span></span> | <span data-ttu-id="cba38-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cba38-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cba38-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cba38-122">Authorization</span></span>  | <span data-ttu-id="cba38-123">string</span><span class="sxs-lookup"><span data-stu-id="cba38-123">string</span></span>  | <span data-ttu-id="cba38-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cba38-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cba38-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cba38-126">Content-Type</span></span> | <span data-ttu-id="cba38-127">string</span><span class="sxs-lookup"><span data-stu-id="cba38-127">string</span></span>  | <span data-ttu-id="cba38-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cba38-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cba38-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cba38-130">Request body</span></span>
<span data-ttu-id="cba38-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="cba38-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cba38-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="cba38-132">Parameter</span></span>    | <span data-ttu-id="cba38-133">Тип</span><span class="sxs-lookup"><span data-stu-id="cba38-133">Type</span></span>   |<span data-ttu-id="cba38-134">Описание</span><span class="sxs-lookup"><span data-stu-id="cba38-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cba38-135">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="cba38-135">newReminderTime</span></span>|<span data-ttu-id="cba38-136">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="cba38-136">DateTimeTimeZone</span></span>|<span data-ttu-id="cba38-137">Новые дата и время для активации напоминания.</span><span class="sxs-lookup"><span data-stu-id="cba38-137">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="cba38-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cba38-138">Response</span></span>

<span data-ttu-id="cba38-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cba38-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cba38-141">Пример</span><span class="sxs-lookup"><span data-stu-id="cba38-141">Example</span></span>
<span data-ttu-id="cba38-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cba38-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cba38-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="cba38-143">Request</span></span>
<span data-ttu-id="cba38-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cba38-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cba38-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="cba38-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cba38-146">C#</span><span class="sxs-lookup"><span data-stu-id="cba38-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-snoozereminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cba38-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cba38-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-snoozereminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cba38-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cba38-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-snoozereminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cba38-149">Java</span><span class="sxs-lookup"><span data-stu-id="cba38-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-snoozereminder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cba38-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="cba38-150">Response</span></span>
<span data-ttu-id="cba38-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cba38-151">Here is an example of the response.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
