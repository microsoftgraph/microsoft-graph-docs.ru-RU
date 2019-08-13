---
title: 'event: decline'
description: Отклонение приглашения на указанное событие в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e4cd0994dbae08cf0d2e9240e1cde115edcc005a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326963"
---
# <a name="event-decline"></a><span data-ttu-id="130cd-103">event: decline</span><span class="sxs-lookup"><span data-stu-id="130cd-103">event: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="130cd-104">Отклонить приглашение для указанного [события](../resources/event.md) в [календаре](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="130cd-104">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="130cd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="130cd-105">Permissions</span></span>
<span data-ttu-id="130cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="130cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="130cd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="130cd-108">Permission type</span></span>      | <span data-ttu-id="130cd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="130cd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="130cd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="130cd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="130cd-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="130cd-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="130cd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="130cd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="130cd-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="130cd-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="130cd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="130cd-114">Application</span></span> | <span data-ttu-id="130cd-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="130cd-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="130cd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="130cd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/decline
POST /users/{id | userPrincipalName}/events/{id}/decline

POST /me/calendar/events/{id}/decline
POST /users/{id | userPrincipalName}/calendar/events/{id}/decline

POST /me/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/decline

POST /me/calendargroup/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/decline

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/decline
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="130cd-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="130cd-117">Request headers</span></span>

| <span data-ttu-id="130cd-118">Имя</span><span class="sxs-lookup"><span data-stu-id="130cd-118">Name</span></span>       | <span data-ttu-id="130cd-119">Тип</span><span class="sxs-lookup"><span data-stu-id="130cd-119">Type</span></span> | <span data-ttu-id="130cd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="130cd-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="130cd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="130cd-121">Authorization</span></span>  | <span data-ttu-id="130cd-122">string</span><span class="sxs-lookup"><span data-stu-id="130cd-122">string</span></span>  | <span data-ttu-id="130cd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="130cd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="130cd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="130cd-125">Content-Type</span></span> | <span data-ttu-id="130cd-126">string</span><span class="sxs-lookup"><span data-stu-id="130cd-126">string</span></span>  | <span data-ttu-id="130cd-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="130cd-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="130cd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="130cd-129">Request body</span></span>

<span data-ttu-id="130cd-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="130cd-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="130cd-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="130cd-131">Parameter</span></span>    | <span data-ttu-id="130cd-132">Тип</span><span class="sxs-lookup"><span data-stu-id="130cd-132">Type</span></span>   |<span data-ttu-id="130cd-133">Описание</span><span class="sxs-lookup"><span data-stu-id="130cd-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="130cd-134">comment</span><span class="sxs-lookup"><span data-stu-id="130cd-134">comment</span></span>|<span data-ttu-id="130cd-135">String</span><span class="sxs-lookup"><span data-stu-id="130cd-135">String</span></span>|<span data-ttu-id="130cd-p104">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="130cd-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="130cd-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="130cd-138">sendResponse</span></span>|<span data-ttu-id="130cd-139">Логическое</span><span class="sxs-lookup"><span data-stu-id="130cd-139">Boolean</span></span>|<span data-ttu-id="130cd-p105">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="130cd-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="130cd-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="130cd-143">Response</span></span>

<span data-ttu-id="130cd-p106">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="130cd-p106">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="130cd-146">Пример</span><span class="sxs-lookup"><span data-stu-id="130cd-146">Example</span></span>

<span data-ttu-id="130cd-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="130cd-147">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="130cd-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="130cd-148">Request</span></span>

<span data-ttu-id="130cd-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="130cd-149">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="130cd-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="130cd-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_decline"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/decline
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="130cd-151">C#</span><span class="sxs-lookup"><span data-stu-id="130cd-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="130cd-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="130cd-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="130cd-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="130cd-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="130cd-154">Java</span><span class="sxs-lookup"><span data-stu-id="130cd-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="130cd-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="130cd-155">Response</span></span>

<span data-ttu-id="130cd-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="130cd-156">Here is an example of the response.</span></span>

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
  "description": "event: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
