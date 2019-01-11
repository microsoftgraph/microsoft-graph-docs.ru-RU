---
title: 'event: dismissReminder'
description: Отключить напоминание, который будет активирована для события в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 570a9b34031afe6d53b6e577127180ebdbe7a163
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864941"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="a0b8a-103">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="a0b8a-103">event: dismissReminder</span></span>

> <span data-ttu-id="a0b8a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a0b8a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0b8a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0b8a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a0b8a-106">Отключить напоминание, который будет активирована для [событий](../resources/event.md) [календаря](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="a0b8a-106">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a0b8a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0b8a-107">Permissions</span></span>
<span data-ttu-id="a0b8a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0b8a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0b8a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0b8a-110">Permission type</span></span>      | <span data-ttu-id="a0b8a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0b8a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0b8a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0b8a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a0b8a-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0b8a-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a0b8a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0b8a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0b8a-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0b8a-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a0b8a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0b8a-116">Application</span></span> | <span data-ttu-id="a0b8a-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0b8a-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0b8a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0b8a-118">HTTP request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a0b8a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0b8a-119">Request headers</span></span>

| <span data-ttu-id="a0b8a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a0b8a-120">Name</span></span>       | <span data-ttu-id="a0b8a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a0b8a-121">Type</span></span> | <span data-ttu-id="a0b8a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a0b8a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a0b8a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0b8a-123">Authorization</span></span>  | <span data-ttu-id="a0b8a-124">string</span><span class="sxs-lookup"><span data-stu-id="a0b8a-124">string</span></span>  | <span data-ttu-id="a0b8a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0b8a-p103">Bearer {token}. Required.</span></span> |


## <a name="response"></a><span data-ttu-id="a0b8a-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0b8a-127">Response</span></span>

<span data-ttu-id="a0b8a-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a0b8a-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0b8a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a0b8a-130">Example</span></span>

<span data-ttu-id="a0b8a-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a0b8a-131">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a0b8a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0b8a-132">Request</span></span>
<span data-ttu-id="a0b8a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0b8a-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/dismissReminder
```

### <a name="response"></a><span data-ttu-id="a0b8a-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0b8a-134">Response</span></span>
<span data-ttu-id="a0b8a-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a0b8a-135">Here is an example of the response.</span></span>

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
