---
title: 'event: dismissReminder'
description: Отклонить напоминание, запущенное для события в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: e3999f6e218c74396f298b2ed5bf366eb9006021
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259166"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="b0ada-103">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="b0ada-103">event: dismissReminder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0ada-104">Отклонить напоминание, запущенное для [события](../resources/event.md) в календаре пользователя [](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="b0ada-104">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b0ada-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0ada-105">Permissions</span></span>
<span data-ttu-id="b0ada-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0ada-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0ada-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0ada-108">Permission type</span></span>      | <span data-ttu-id="b0ada-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0ada-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0ada-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0ada-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b0ada-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0ada-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b0ada-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0ada-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0ada-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0ada-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b0ada-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0ada-114">Application</span></span> | <span data-ttu-id="b0ada-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0ada-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0ada-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0ada-116">HTTP request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b0ada-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0ada-117">Request headers</span></span>

| <span data-ttu-id="b0ada-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b0ada-118">Name</span></span>       | <span data-ttu-id="b0ada-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b0ada-119">Type</span></span> | <span data-ttu-id="b0ada-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b0ada-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b0ada-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0ada-121">Authorization</span></span>  | <span data-ttu-id="b0ada-122">string</span><span class="sxs-lookup"><span data-stu-id="b0ada-122">string</span></span>  | <span data-ttu-id="b0ada-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0ada-p102">Bearer {token}. Required.</span></span> |


## <a name="response"></a><span data-ttu-id="b0ada-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0ada-125">Response</span></span>

<span data-ttu-id="b0ada-p103">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b0ada-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0ada-128">Пример</span><span class="sxs-lookup"><span data-stu-id="b0ada-128">Example</span></span>

<span data-ttu-id="b0ada-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b0ada-129">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="b0ada-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0ada-130">Request</span></span>
<span data-ttu-id="b0ada-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0ada-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/dismissReminder
```

### <a name="response"></a><span data-ttu-id="b0ada-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0ada-132">Response</span></span>
<span data-ttu-id="b0ada-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b0ada-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b0ada-134">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="b0ada-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b0ada-135">C#</span><span class="sxs-lookup"><span data-stu-id="b0ada-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/event_dismissreminder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0ada-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="b0ada-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/event_dismissreminder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b0ada-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b0ada-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/event_dismissreminder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-dismissreminder.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/event-dismissreminder.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-dismissreminder.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
