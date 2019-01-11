---
title: 'event: dismissReminder'
description: Отключить напоминание, который будет активирована для события в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 1165dbf036848ee01ad80a1080a01e9b344fc399
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811573"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="1435f-103">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="1435f-103">event: dismissReminder</span></span>

<span data-ttu-id="1435f-104">Отключить напоминание, который будет активирована для [событий](../resources/event.md) [календаря](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="1435f-104">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1435f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1435f-105">Permissions</span></span>
<span data-ttu-id="1435f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1435f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1435f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1435f-108">Permission type</span></span>      | <span data-ttu-id="1435f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1435f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1435f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1435f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1435f-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1435f-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="1435f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1435f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1435f-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1435f-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="1435f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1435f-114">Application</span></span> | <span data-ttu-id="1435f-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1435f-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1435f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1435f-116">HTTP request</span></span>

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

<br/>

## <a name="request-headers"></a><span data-ttu-id="1435f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1435f-117">Request headers</span></span>
| <span data-ttu-id="1435f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1435f-118">Name</span></span>       | <span data-ttu-id="1435f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="1435f-119">Type</span></span> | <span data-ttu-id="1435f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1435f-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1435f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1435f-121">Authorization</span></span>  | <span data-ttu-id="1435f-122">string</span><span class="sxs-lookup"><span data-stu-id="1435f-122">string</span></span>  | <span data-ttu-id="1435f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1435f-p102">Bearer {token}. Required.</span></span> |

<br/>

## <a name="response"></a><span data-ttu-id="1435f-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="1435f-125">Response</span></span>

<span data-ttu-id="1435f-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1435f-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1435f-128">Пример</span><span class="sxs-lookup"><span data-stu-id="1435f-128">Example</span></span>

<span data-ttu-id="1435f-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1435f-129">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1435f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1435f-130">Request</span></span>
<span data-ttu-id="1435f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1435f-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```

<br/>

### <a name="response"></a><span data-ttu-id="1435f-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="1435f-132">Response</span></span>
<span data-ttu-id="1435f-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1435f-133">Here is an example of the response.</span></span>

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
