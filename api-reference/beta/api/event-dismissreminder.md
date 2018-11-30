---
title: 'event: dismissReminder'
description: Отключить напоминание, который будет активирована для события в календаре пользователя.
ms.openlocfilehash: bb04048d82bc2fa06e1b8a19d453510f88da17a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080989"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="fc7d6-103">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="fc7d6-103">event: dismissReminder</span></span>

> <span data-ttu-id="fc7d6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fc7d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc7d6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc7d6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fc7d6-106">Отключить напоминание, который будет активирована для [событий](../resources/event.md) [календаря](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="fc7d6-106">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fc7d6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc7d6-107">Permissions</span></span>
<span data-ttu-id="fc7d6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc7d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc7d6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc7d6-110">Permission type</span></span>      | <span data-ttu-id="fc7d6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc7d6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc7d6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc7d6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fc7d6-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc7d6-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fc7d6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc7d6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc7d6-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc7d6-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fc7d6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc7d6-116">Application</span></span> | <span data-ttu-id="fc7d6-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc7d6-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc7d6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc7d6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/events/{id}/dismissReminder

POST /me/calendar/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/dismissReminder

POST /me/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroup/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
```

## <a name="request-headers"></a><span data-ttu-id="fc7d6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc7d6-119">Request headers</span></span>

| <span data-ttu-id="fc7d6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fc7d6-120">Name</span></span>       | <span data-ttu-id="fc7d6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fc7d6-121">Type</span></span> | <span data-ttu-id="fc7d6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fc7d6-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fc7d6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc7d6-123">Authorization</span></span>  | <span data-ttu-id="fc7d6-124">string</span><span class="sxs-lookup"><span data-stu-id="fc7d6-124">string</span></span>  | <span data-ttu-id="fc7d6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc7d6-p103">Bearer {token}. Required.</span></span> |


## <a name="response"></a><span data-ttu-id="fc7d6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc7d6-127">Response</span></span>

<span data-ttu-id="fc7d6-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fc7d6-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc7d6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fc7d6-130">Example</span></span>

<span data-ttu-id="fc7d6-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="fc7d6-131">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="fc7d6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc7d6-132">Request</span></span>
<span data-ttu-id="fc7d6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc7d6-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/dismissReminder
```

### <a name="response"></a><span data-ttu-id="fc7d6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc7d6-134">Response</span></span>
<span data-ttu-id="fc7d6-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc7d6-135">Here is an example of the response.</span></span>

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
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
