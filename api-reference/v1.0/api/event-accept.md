---
title: 'event: accept'
description: Принятие указанного события в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ca84ede4aedf406bc2191221e30fb9976a80e97f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517399"
---
# <a name="event-accept"></a><span data-ttu-id="3c155-103">event: accept</span><span class="sxs-lookup"><span data-stu-id="3c155-103">event: accept</span></span>

<span data-ttu-id="3c155-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c155-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3c155-105">Принять указанное [событие](../resources/event.md) в [календаре](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="3c155-105">Accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c155-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c155-106">Permissions</span></span>
<span data-ttu-id="3c155-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c155-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c155-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c155-109">Permission type</span></span>      | <span data-ttu-id="3c155-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c155-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c155-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c155-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3c155-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c155-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="3c155-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c155-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c155-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c155-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="3c155-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c155-115">Application</span></span> | <span data-ttu-id="3c155-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c155-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c155-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c155-117">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="3c155-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c155-118">Request headers</span></span>
| <span data-ttu-id="3c155-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3c155-119">Name</span></span>       | <span data-ttu-id="3c155-120">Тип</span><span class="sxs-lookup"><span data-stu-id="3c155-120">Type</span></span> | <span data-ttu-id="3c155-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3c155-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3c155-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c155-122">Authorization</span></span>  | <span data-ttu-id="3c155-123">string</span><span class="sxs-lookup"><span data-stu-id="3c155-123">string</span></span>  | <span data-ttu-id="3c155-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c155-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3c155-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3c155-126">Content-Type</span></span> | <span data-ttu-id="3c155-127">string</span><span class="sxs-lookup"><span data-stu-id="3c155-127">string</span></span>  | <span data-ttu-id="3c155-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c155-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c155-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c155-130">Request body</span></span>
<span data-ttu-id="3c155-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3c155-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3c155-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="3c155-132">Parameter</span></span>    | <span data-ttu-id="3c155-133">Тип</span><span class="sxs-lookup"><span data-stu-id="3c155-133">Type</span></span>   |<span data-ttu-id="3c155-134">Описание</span><span class="sxs-lookup"><span data-stu-id="3c155-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c155-135">comment</span><span class="sxs-lookup"><span data-stu-id="3c155-135">comment</span></span>|<span data-ttu-id="3c155-136">String</span><span class="sxs-lookup"><span data-stu-id="3c155-136">String</span></span>|<span data-ttu-id="3c155-p104">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="3c155-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="3c155-139">sendResponse</span><span class="sxs-lookup"><span data-stu-id="3c155-139">sendResponse</span></span>|<span data-ttu-id="3c155-140">Логическое</span><span class="sxs-lookup"><span data-stu-id="3c155-140">Boolean</span></span>|<span data-ttu-id="3c155-p105">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="3c155-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="3c155-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c155-144">Response</span></span>

<span data-ttu-id="3c155-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3c155-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c155-147">Пример</span><span class="sxs-lookup"><span data-stu-id="3c155-147">Example</span></span>
<span data-ttu-id="3c155-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3c155-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3c155-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c155-149">Request</span></span>
<span data-ttu-id="3c155-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c155-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3c155-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c155-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_accept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/accept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```
# <a name="c"></a>[<span data-ttu-id="3c155-152">C#</span><span class="sxs-lookup"><span data-stu-id="3c155-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-accept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c155-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c155-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-accept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c155-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c155-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-accept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c155-155">Java</span><span class="sxs-lookup"><span data-stu-id="3c155-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-accept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3c155-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c155-156">Response</span></span>
<span data-ttu-id="3c155-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3c155-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: accept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
