---
title: 'event: dismissReminder'
description: Отклонять напоминание, которое было вызвано событием в календаре пользователей.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7b2a33e199a7add86c494a48da5b519119279732
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448321"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="caa02-103">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="caa02-103">event: dismissReminder</span></span>

<span data-ttu-id="caa02-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="caa02-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="caa02-105">Отклонять напоминание, которое было вызвано [событием](../resources/event.md) в календаре [пользователей.](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="caa02-105">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="caa02-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="caa02-106">Permissions</span></span>
<span data-ttu-id="caa02-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caa02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caa02-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="caa02-109">Permission type</span></span>      | <span data-ttu-id="caa02-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="caa02-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="caa02-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="caa02-111">Delegated (work or school account)</span></span> | <span data-ttu-id="caa02-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="caa02-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="caa02-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="caa02-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="caa02-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="caa02-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="caa02-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="caa02-115">Application</span></span> | <span data-ttu-id="caa02-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="caa02-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="caa02-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="caa02-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/events/{id}/dismissReminder

POST /me/calendar/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/dismissReminder

POST /me/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="caa02-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="caa02-118">Request headers</span></span>
| <span data-ttu-id="caa02-119">Имя</span><span class="sxs-lookup"><span data-stu-id="caa02-119">Name</span></span>       | <span data-ttu-id="caa02-120">Тип</span><span class="sxs-lookup"><span data-stu-id="caa02-120">Type</span></span> | <span data-ttu-id="caa02-121">Описание</span><span class="sxs-lookup"><span data-stu-id="caa02-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="caa02-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="caa02-122">Authorization</span></span>  | <span data-ttu-id="caa02-123">string</span><span class="sxs-lookup"><span data-stu-id="caa02-123">string</span></span>  | <span data-ttu-id="caa02-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="caa02-p102">Bearer {token}. Required.</span></span> |

<br/>

## <a name="response"></a><span data-ttu-id="caa02-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="caa02-126">Response</span></span>

<span data-ttu-id="caa02-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="caa02-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caa02-129">Пример</span><span class="sxs-lookup"><span data-stu-id="caa02-129">Example</span></span>

<span data-ttu-id="caa02-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="caa02-130">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="caa02-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="caa02-131">Request</span></span>
<span data-ttu-id="caa02-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="caa02-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="caa02-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="caa02-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```
# <a name="c"></a>[<span data-ttu-id="caa02-134">C#</span><span class="sxs-lookup"><span data-stu-id="caa02-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-dismissreminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="caa02-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="caa02-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-dismissreminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="caa02-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="caa02-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-dismissreminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="caa02-137">Java</span><span class="sxs-lookup"><span data-stu-id="caa02-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-dismissreminder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<br/>

### <a name="response"></a><span data-ttu-id="caa02-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="caa02-138">Response</span></span>
<span data-ttu-id="caa02-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="caa02-139">Here is an example of the response.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->

