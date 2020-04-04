---
title: Удаление события
description: Удаление события.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 04ec124393bb5925c4f1f8c4596c6320de3c1f7b
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144228"
---
# <a name="delete-event"></a><span data-ttu-id="b840e-103">Удаление события</span><span class="sxs-lookup"><span data-stu-id="b840e-103">Delete event</span></span>

<span data-ttu-id="b840e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b840e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b840e-105">Удаляет указанное [событие](../resources/event.md) из содержащегося календаря.</span><span class="sxs-lookup"><span data-stu-id="b840e-105">Removes the specified [event](../resources/event.md) from the containing calendar.</span></span> 

<span data-ttu-id="b840e-106">Если событие является собранием, удаление события в календаре организатора отправляет сообщение об отмене участникам собрания.</span><span class="sxs-lookup"><span data-stu-id="b840e-106">If the event is a meeting, deleting the event on the organizer's calendar sends a cancellation message to the meeting attendees.</span></span>

## <a name="permissions"></a><span data-ttu-id="b840e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b840e-107">Permissions</span></span>
<span data-ttu-id="b840e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b840e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b840e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b840e-110">Permission type</span></span>      | <span data-ttu-id="b840e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b840e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b840e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b840e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b840e-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b840e-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b840e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b840e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b840e-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b840e-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b840e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b840e-116">Application</span></span> | <span data-ttu-id="b840e-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b840e-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b840e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b840e-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="b840e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b840e-119">Request headers</span></span>
| <span data-ttu-id="b840e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b840e-120">Name</span></span>       | <span data-ttu-id="b840e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b840e-121">Type</span></span> | <span data-ttu-id="b840e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b840e-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b840e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b840e-123">Authorization</span></span>  | <span data-ttu-id="b840e-124">string</span><span class="sxs-lookup"><span data-stu-id="b840e-124">string</span></span>  | <span data-ttu-id="b840e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b840e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b840e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b840e-127">Request body</span></span>
<span data-ttu-id="b840e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b840e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b840e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b840e-129">Response</span></span>

<span data-ttu-id="b840e-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b840e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b840e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b840e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b840e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b840e-133">Request</span></span>
<span data-ttu-id="b840e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b840e-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b840e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b840e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/events/{id}
```
# <a name="c"></a>[<span data-ttu-id="b840e-136">C#</span><span class="sxs-lookup"><span data-stu-id="b840e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b840e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b840e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b840e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b840e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b840e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b840e-139">Response</span></span>
<span data-ttu-id="b840e-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b840e-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
