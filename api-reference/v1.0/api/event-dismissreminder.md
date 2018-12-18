---
title: 'event: dismissReminder'
description: Отключить напоминание, который будет активирована для события в календаре пользователя.
author: angelgolfer-ms
ms.openlocfilehash: 1075ee86ee174bab23bd0436c69da37f1f001d66
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357780"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="a5c26-103">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="a5c26-103">event: dismissReminder</span></span>

<span data-ttu-id="a5c26-104">Отключить напоминание, который будет активирована для [событий](../resources/event.md) [календаря](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="a5c26-104">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a5c26-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5c26-105">Permissions</span></span>
<span data-ttu-id="a5c26-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5c26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5c26-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5c26-108">Permission type</span></span>      | <span data-ttu-id="a5c26-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5c26-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5c26-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5c26-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a5c26-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5c26-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a5c26-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5c26-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5c26-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5c26-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a5c26-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5c26-114">Application</span></span> | <span data-ttu-id="a5c26-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5c26-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5c26-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5c26-116">HTTP request</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="a5c26-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5c26-117">Request headers</span></span>
| <span data-ttu-id="a5c26-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a5c26-118">Name</span></span>       | <span data-ttu-id="a5c26-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a5c26-119">Type</span></span> | <span data-ttu-id="a5c26-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a5c26-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a5c26-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5c26-121">Authorization</span></span>  | <span data-ttu-id="a5c26-122">string</span><span class="sxs-lookup"><span data-stu-id="a5c26-122">string</span></span>  | <span data-ttu-id="a5c26-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5c26-p102">Bearer {token}. Required.</span></span> |

<br/>

## <a name="response"></a><span data-ttu-id="a5c26-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5c26-125">Response</span></span>

<span data-ttu-id="a5c26-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a5c26-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5c26-128">Пример</span><span class="sxs-lookup"><span data-stu-id="a5c26-128">Example</span></span>

<span data-ttu-id="a5c26-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a5c26-129">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a5c26-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5c26-130">Request</span></span>
<span data-ttu-id="a5c26-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5c26-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```

<br/>

### <a name="response"></a><span data-ttu-id="a5c26-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="a5c26-132">Response</span></span>
<span data-ttu-id="a5c26-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a5c26-133">Here is an example of the response.</span></span>

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
