---
title: 'event: accept'
description: Принятие указанного события в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2f8f33ff835a99d3a72c55bbcc95ea53db1fd51b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887488"
---
# <a name="event-accept"></a><span data-ttu-id="846ec-103">event: accept</span><span class="sxs-lookup"><span data-stu-id="846ec-103">event: accept</span></span>

<span data-ttu-id="846ec-104">Принять указанное [событие](../resources/event.md) в календаре пользователя [](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="846ec-104">Accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="846ec-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="846ec-105">Permissions</span></span>
<span data-ttu-id="846ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="846ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="846ec-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="846ec-108">Permission type</span></span>      | <span data-ttu-id="846ec-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="846ec-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="846ec-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="846ec-110">Delegated (work or school account)</span></span> | <span data-ttu-id="846ec-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="846ec-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="846ec-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="846ec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="846ec-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="846ec-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="846ec-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="846ec-114">Application</span></span> | <span data-ttu-id="846ec-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="846ec-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="846ec-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="846ec-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="846ec-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="846ec-117">Request headers</span></span>
| <span data-ttu-id="846ec-118">Имя</span><span class="sxs-lookup"><span data-stu-id="846ec-118">Name</span></span>       | <span data-ttu-id="846ec-119">Тип</span><span class="sxs-lookup"><span data-stu-id="846ec-119">Type</span></span> | <span data-ttu-id="846ec-120">Описание</span><span class="sxs-lookup"><span data-stu-id="846ec-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="846ec-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="846ec-121">Authorization</span></span>  | <span data-ttu-id="846ec-122">string</span><span class="sxs-lookup"><span data-stu-id="846ec-122">string</span></span>  | <span data-ttu-id="846ec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="846ec-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="846ec-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="846ec-125">Content-Type</span></span> | <span data-ttu-id="846ec-126">string</span><span class="sxs-lookup"><span data-stu-id="846ec-126">string</span></span>  | <span data-ttu-id="846ec-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="846ec-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="846ec-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="846ec-129">Request body</span></span>
<span data-ttu-id="846ec-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="846ec-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="846ec-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="846ec-131">Parameter</span></span>    | <span data-ttu-id="846ec-132">Тип</span><span class="sxs-lookup"><span data-stu-id="846ec-132">Type</span></span>   |<span data-ttu-id="846ec-133">Описание</span><span class="sxs-lookup"><span data-stu-id="846ec-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="846ec-134">comment</span><span class="sxs-lookup"><span data-stu-id="846ec-134">comment</span></span>|<span data-ttu-id="846ec-135">String</span><span class="sxs-lookup"><span data-stu-id="846ec-135">String</span></span>|<span data-ttu-id="846ec-p104">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="846ec-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="846ec-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="846ec-138">sendResponse</span></span>|<span data-ttu-id="846ec-139">Логическое</span><span class="sxs-lookup"><span data-stu-id="846ec-139">Boolean</span></span>|<span data-ttu-id="846ec-p105">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="846ec-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="846ec-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="846ec-143">Response</span></span>

<span data-ttu-id="846ec-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="846ec-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="846ec-146">Пример</span><span class="sxs-lookup"><span data-stu-id="846ec-146">Example</span></span>
<span data-ttu-id="846ec-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="846ec-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="846ec-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="846ec-148">Request</span></span>
<span data-ttu-id="846ec-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="846ec-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="846ec-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="846ec-150">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="846ec-151">C#</span><span class="sxs-lookup"><span data-stu-id="846ec-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-accept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="846ec-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="846ec-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-accept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="846ec-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="846ec-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-accept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="846ec-154">Java</span><span class="sxs-lookup"><span data-stu-id="846ec-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-accept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="846ec-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="846ec-155">Response</span></span>
<span data-ttu-id="846ec-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="846ec-156">Here is an example of the response.</span></span>
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
  "description": "event: accept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
