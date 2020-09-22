---
title: 'event: accept'
description: Принятие указанного события в календаре пользователя.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4f73931055b84e7c4ac07d25bf14b9659a228c7d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981042"
---
# <a name="event-accept"></a><span data-ttu-id="a889d-103">event: accept</span><span class="sxs-lookup"><span data-stu-id="a889d-103">event: accept</span></span>

<span data-ttu-id="a889d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a889d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a889d-105">Принять указанное [событие](../resources/event.md) в [календаре](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="a889d-105">Accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a889d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a889d-106">Permissions</span></span>
<span data-ttu-id="a889d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a889d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a889d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a889d-109">Permission type</span></span>      | <span data-ttu-id="a889d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a889d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a889d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a889d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a889d-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a889d-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a889d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a889d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a889d-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a889d-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a889d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a889d-115">Application</span></span> | <span data-ttu-id="a889d-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a889d-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a889d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a889d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/accept
POST /users/{id | userPrincipalName}/events/{id}/accept

POST /me/calendar/events/{id}/accept
POST /users/{id | userPrincipalName}/calendar/events/{id}/accept

POST /me/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/accept

POST /me/calendargroup/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/accept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/accept
```
## <a name="request-headers"></a><span data-ttu-id="a889d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a889d-118">Request headers</span></span>
| <span data-ttu-id="a889d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a889d-119">Name</span></span>       | <span data-ttu-id="a889d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a889d-120">Type</span></span> | <span data-ttu-id="a889d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a889d-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a889d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a889d-122">Authorization</span></span>  | <span data-ttu-id="a889d-123">string</span><span class="sxs-lookup"><span data-stu-id="a889d-123">string</span></span>  | <span data-ttu-id="a889d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a889d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a889d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a889d-126">Content-Type</span></span> | <span data-ttu-id="a889d-127">string</span><span class="sxs-lookup"><span data-stu-id="a889d-127">string</span></span>  | <span data-ttu-id="a889d-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a889d-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a889d-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a889d-130">Request body</span></span>
<span data-ttu-id="a889d-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a889d-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a889d-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="a889d-132">Parameter</span></span>    | <span data-ttu-id="a889d-133">Тип</span><span class="sxs-lookup"><span data-stu-id="a889d-133">Type</span></span>   |<span data-ttu-id="a889d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a889d-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a889d-135">comment</span><span class="sxs-lookup"><span data-stu-id="a889d-135">comment</span></span>|<span data-ttu-id="a889d-136">String</span><span class="sxs-lookup"><span data-stu-id="a889d-136">String</span></span>|<span data-ttu-id="a889d-p104">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="a889d-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="a889d-139">sendResponse</span><span class="sxs-lookup"><span data-stu-id="a889d-139">sendResponse</span></span>|<span data-ttu-id="a889d-140">Логическое</span><span class="sxs-lookup"><span data-stu-id="a889d-140">Boolean</span></span>|<span data-ttu-id="a889d-p105">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="a889d-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="a889d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a889d-144">Response</span></span>

<span data-ttu-id="a889d-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a889d-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a889d-147">Пример</span><span class="sxs-lookup"><span data-stu-id="a889d-147">Example</span></span>
<span data-ttu-id="a889d-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a889d-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a889d-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="a889d-149">Request</span></span>
<span data-ttu-id="a889d-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a889d-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a889d-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="a889d-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_accept"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/accept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```
# <a name="c"></a>[<span data-ttu-id="a889d-152">C#</span><span class="sxs-lookup"><span data-stu-id="a889d-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-accept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a889d-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a889d-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-accept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a889d-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a889d-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-accept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a889d-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="a889d-155">Response</span></span>
<span data-ttu-id="a889d-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a889d-156">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: accept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


