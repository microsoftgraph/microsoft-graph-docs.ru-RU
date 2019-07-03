---
title: Удаление события
description: Удаление события.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: c8fe926b262019b33645e6ba809fedff04d59d0c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448446"
---
# <a name="delete-event"></a><span data-ttu-id="80f66-103">Удаление события</span><span class="sxs-lookup"><span data-stu-id="80f66-103">Delete event</span></span>

<span data-ttu-id="80f66-104">Удаление события.</span><span class="sxs-lookup"><span data-stu-id="80f66-104">Delete event.</span></span>
## <a name="permissions"></a><span data-ttu-id="80f66-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80f66-105">Permissions</span></span>
<span data-ttu-id="80f66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80f66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80f66-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80f66-108">Permission type</span></span>      | <span data-ttu-id="80f66-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80f66-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80f66-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80f66-110">Delegated (work or school account)</span></span> | <span data-ttu-id="80f66-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80f66-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="80f66-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80f66-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80f66-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80f66-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="80f66-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80f66-114">Application</span></span> | <span data-ttu-id="80f66-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80f66-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="80f66-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80f66-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}
DELETE /users/{id | userPrincipalName}/events/{id}
DELETE /groups/{id}/events/{id}

DELETE /me/calendar/events/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}
DELETE /groups/{id}/calendar/events/{id}/

DELETE /me/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="80f66-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80f66-117">Request headers</span></span>
| <span data-ttu-id="80f66-118">Имя</span><span class="sxs-lookup"><span data-stu-id="80f66-118">Name</span></span>       | <span data-ttu-id="80f66-119">Тип</span><span class="sxs-lookup"><span data-stu-id="80f66-119">Type</span></span> | <span data-ttu-id="80f66-120">Описание</span><span class="sxs-lookup"><span data-stu-id="80f66-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="80f66-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="80f66-121">Authorization</span></span>  | <span data-ttu-id="80f66-122">string</span><span class="sxs-lookup"><span data-stu-id="80f66-122">string</span></span>  | <span data-ttu-id="80f66-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80f66-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80f66-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80f66-125">Request body</span></span>
<span data-ttu-id="80f66-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="80f66-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80f66-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="80f66-127">Response</span></span>

<span data-ttu-id="80f66-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="80f66-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80f66-130">Пример</span><span class="sxs-lookup"><span data-stu-id="80f66-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80f66-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="80f66-131">Request</span></span>
<span data-ttu-id="80f66-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80f66-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="80f66-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="80f66-133">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="80f66-134">C#</span><span class="sxs-lookup"><span data-stu-id="80f66-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="80f66-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80f66-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="80f66-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80f66-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="80f66-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="80f66-137">Response</span></span>
<span data-ttu-id="80f66-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="80f66-138">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
