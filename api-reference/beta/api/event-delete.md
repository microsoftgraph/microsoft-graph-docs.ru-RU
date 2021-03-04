---
title: Удаление события
description: Удаление события.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b73bdae172fe87e91a5485aa786e7556157eb6f1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436262"
---
# <a name="delete-event"></a><span data-ttu-id="4605b-103">Удаление события</span><span class="sxs-lookup"><span data-stu-id="4605b-103">Delete event</span></span>

<span data-ttu-id="4605b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4605b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4605b-105">Удаляет указанное [событие](../resources/event.md) из содержащего его календаря.</span><span class="sxs-lookup"><span data-stu-id="4605b-105">Removes the specified [event](../resources/event.md) from the containing calendar.</span></span> 

<span data-ttu-id="4605b-106">Если событием является собрание, при удалении события в календаре организатора сообщение об отмене отправляется участникам собрания.</span><span class="sxs-lookup"><span data-stu-id="4605b-106">If the event is a meeting, deleting the event on the organizer's calendar sends a cancellation message to the meeting attendees.</span></span>

## <a name="permissions"></a><span data-ttu-id="4605b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4605b-107">Permissions</span></span>
<span data-ttu-id="4605b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4605b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4605b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4605b-110">Permission type</span></span>      | <span data-ttu-id="4605b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4605b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4605b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4605b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4605b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4605b-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4605b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4605b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4605b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4605b-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4605b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4605b-116">Application</span></span> | <span data-ttu-id="4605b-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4605b-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4605b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4605b-118">HTTP request</span></span>
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

DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4605b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4605b-119">Request headers</span></span>
| <span data-ttu-id="4605b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4605b-120">Name</span></span>       | <span data-ttu-id="4605b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4605b-121">Type</span></span> | <span data-ttu-id="4605b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4605b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4605b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4605b-123">Authorization</span></span>  | <span data-ttu-id="4605b-124">string</span><span class="sxs-lookup"><span data-stu-id="4605b-124">string</span></span>  | <span data-ttu-id="4605b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4605b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4605b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4605b-127">Request body</span></span>
<span data-ttu-id="4605b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4605b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4605b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4605b-129">Response</span></span>

<span data-ttu-id="4605b-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4605b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4605b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4605b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4605b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4605b-133">Request</span></span>
<span data-ttu-id="4605b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4605b-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4605b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4605b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/events/{id}
```
# <a name="c"></a>[<span data-ttu-id="4605b-136">C#</span><span class="sxs-lookup"><span data-stu-id="4605b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4605b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4605b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4605b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4605b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4605b-139">Java</span><span class="sxs-lookup"><span data-stu-id="4605b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4605b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4605b-140">Response</span></span>
<span data-ttu-id="4605b-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4605b-141">Here is an example of the response.</span></span> 
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


