---
title: 'event: dismissReminder'
description: Отклонить напоминание, запущенное для события в календаре пользователя.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 05102f7d8382dbb97ce4d394cd597c0d58e4220c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954892"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="a2060-103">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="a2060-103">event: dismissReminder</span></span>

<span data-ttu-id="a2060-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2060-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2060-105">Отклонить напоминание, запущенное для [события](../resources/event.md) в [календаре](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="a2060-105">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a2060-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2060-106">Permissions</span></span>
<span data-ttu-id="a2060-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2060-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2060-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2060-109">Permission type</span></span>      | <span data-ttu-id="a2060-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2060-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2060-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2060-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a2060-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2060-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a2060-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2060-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2060-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2060-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a2060-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2060-115">Application</span></span> | <span data-ttu-id="a2060-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2060-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2060-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2060-117">HTTP request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a2060-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2060-118">Request headers</span></span>

| <span data-ttu-id="a2060-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a2060-119">Name</span></span>       | <span data-ttu-id="a2060-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a2060-120">Type</span></span> | <span data-ttu-id="a2060-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a2060-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a2060-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2060-122">Authorization</span></span>  | <span data-ttu-id="a2060-123">string</span><span class="sxs-lookup"><span data-stu-id="a2060-123">string</span></span>  | <span data-ttu-id="a2060-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2060-p102">Bearer {token}. Required.</span></span> |


## <a name="response"></a><span data-ttu-id="a2060-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2060-126">Response</span></span>

<span data-ttu-id="a2060-p103">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a2060-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2060-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a2060-129">Example</span></span>

<span data-ttu-id="a2060-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a2060-130">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a2060-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2060-131">Request</span></span>
<span data-ttu-id="a2060-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2060-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a2060-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2060-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/dismissReminder
```
# <a name="c"></a>[<span data-ttu-id="a2060-134">C#</span><span class="sxs-lookup"><span data-stu-id="a2060-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-dismissreminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2060-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2060-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-dismissreminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2060-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2060-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-dismissreminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2060-137">Java</span><span class="sxs-lookup"><span data-stu-id="a2060-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-dismissreminder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a2060-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2060-138">Response</span></span>
<span data-ttu-id="a2060-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a2060-139">Here is an example of the response.</span></span>

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
  "suppressions": [
  ]
}
-->


