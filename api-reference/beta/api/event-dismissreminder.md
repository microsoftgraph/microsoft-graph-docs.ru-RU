---
title: 'event: dismissReminder'
description: ОтКлонить напоминание, запущенное для события в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: dd10d8a94e2661f2006ccb10c4a823c4afc3fdb4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324415"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="aaf33-103">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="aaf33-103">event: dismissReminder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aaf33-104">ОтКлонить напоминание, запущенное для [события](../resources/event.md) в календаре пользователя [](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="aaf33-104">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="aaf33-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aaf33-105">Permissions</span></span>
<span data-ttu-id="aaf33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaf33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaf33-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aaf33-108">Permission type</span></span>      | <span data-ttu-id="aaf33-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aaf33-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aaf33-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aaf33-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aaf33-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aaf33-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="aaf33-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aaf33-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aaf33-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aaf33-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="aaf33-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aaf33-114">Application</span></span> | <span data-ttu-id="aaf33-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aaf33-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="aaf33-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aaf33-116">HTTP request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="aaf33-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aaf33-117">Request headers</span></span>

| <span data-ttu-id="aaf33-118">Имя</span><span class="sxs-lookup"><span data-stu-id="aaf33-118">Name</span></span>       | <span data-ttu-id="aaf33-119">Тип</span><span class="sxs-lookup"><span data-stu-id="aaf33-119">Type</span></span> | <span data-ttu-id="aaf33-120">Описание</span><span class="sxs-lookup"><span data-stu-id="aaf33-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aaf33-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaf33-121">Authorization</span></span>  | <span data-ttu-id="aaf33-122">string</span><span class="sxs-lookup"><span data-stu-id="aaf33-122">string</span></span>  | <span data-ttu-id="aaf33-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aaf33-p102">Bearer {token}. Required.</span></span> |


## <a name="response"></a><span data-ttu-id="aaf33-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaf33-125">Response</span></span>

<span data-ttu-id="aaf33-p103">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="aaf33-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaf33-128">Пример</span><span class="sxs-lookup"><span data-stu-id="aaf33-128">Example</span></span>

<span data-ttu-id="aaf33-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="aaf33-129">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="aaf33-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="aaf33-130">Request</span></span>
<span data-ttu-id="aaf33-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aaf33-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/dismissReminder
```

### <a name="response"></a><span data-ttu-id="aaf33-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaf33-132">Response</span></span>
<span data-ttu-id="aaf33-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aaf33-133">Here is an example of the response.</span></span>

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
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
