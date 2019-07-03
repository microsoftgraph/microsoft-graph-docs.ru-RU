---
title: 'event: dismissReminder'
description: Отклонить напоминание, запущенное для события в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f3b35c2528eae44f3657792fa201ee5ff130c66d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458292"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="bdcc6-103">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="bdcc6-103">event: dismissReminder</span></span>

<span data-ttu-id="bdcc6-104">Отклонить напоминание, запущенное для [события](../resources/event.md) в календаре пользователя [](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="bdcc6-104">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bdcc6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bdcc6-105">Permissions</span></span>
<span data-ttu-id="bdcc6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdcc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdcc6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdcc6-108">Permission type</span></span>      | <span data-ttu-id="bdcc6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdcc6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdcc6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdcc6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bdcc6-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdcc6-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bdcc6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdcc6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdcc6-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdcc6-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bdcc6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdcc6-114">Application</span></span> | <span data-ttu-id="bdcc6-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdcc6-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdcc6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdcc6-116">HTTP request</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="bdcc6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdcc6-117">Request headers</span></span>
| <span data-ttu-id="bdcc6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bdcc6-118">Name</span></span>       | <span data-ttu-id="bdcc6-119">Тип</span><span class="sxs-lookup"><span data-stu-id="bdcc6-119">Type</span></span> | <span data-ttu-id="bdcc6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bdcc6-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bdcc6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdcc6-121">Authorization</span></span>  | <span data-ttu-id="bdcc6-122">string</span><span class="sxs-lookup"><span data-stu-id="bdcc6-122">string</span></span>  | <span data-ttu-id="bdcc6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdcc6-p102">Bearer {token}. Required.</span></span> |

<br/>

## <a name="response"></a><span data-ttu-id="bdcc6-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdcc6-125">Response</span></span>

<span data-ttu-id="bdcc6-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bdcc6-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdcc6-128">Пример</span><span class="sxs-lookup"><span data-stu-id="bdcc6-128">Example</span></span>

<span data-ttu-id="bdcc6-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bdcc6-129">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="bdcc6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdcc6-130">Request</span></span>
<span data-ttu-id="bdcc6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdcc6-131">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bdcc6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="bdcc6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bdcc6-133">C#</span><span class="sxs-lookup"><span data-stu-id="bdcc6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-dismissreminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bdcc6-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="bdcc6-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-dismissreminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bdcc6-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bdcc6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-dismissreminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<br/>

### <a name="response"></a><span data-ttu-id="bdcc6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdcc6-136">Response</span></span>
<span data-ttu-id="bdcc6-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bdcc6-137">Here is an example of the response.</span></span>

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
