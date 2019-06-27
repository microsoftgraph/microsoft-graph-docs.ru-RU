---
title: 'event: decline'
description: Отклонение приглашения на указанное событие в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 3b6f648d5bbe3adbff5fcfd4f852a2b1c5e75a79
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259236"
---
# <a name="event-decline"></a><span data-ttu-id="485fc-103">event: decline</span><span class="sxs-lookup"><span data-stu-id="485fc-103">event: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="485fc-104">Отклонить приглашение для указанного [события](../resources/event.md) в [календаре](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="485fc-104">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="485fc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="485fc-105">Permissions</span></span>
<span data-ttu-id="485fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="485fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="485fc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="485fc-108">Permission type</span></span>      | <span data-ttu-id="485fc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="485fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="485fc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="485fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="485fc-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="485fc-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="485fc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="485fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="485fc-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="485fc-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="485fc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="485fc-114">Application</span></span> | <span data-ttu-id="485fc-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="485fc-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="485fc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="485fc-116">HTTP request</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="485fc-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="485fc-117">Request headers</span></span>

| <span data-ttu-id="485fc-118">Имя</span><span class="sxs-lookup"><span data-stu-id="485fc-118">Name</span></span>       | <span data-ttu-id="485fc-119">Тип</span><span class="sxs-lookup"><span data-stu-id="485fc-119">Type</span></span> | <span data-ttu-id="485fc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="485fc-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="485fc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="485fc-121">Authorization</span></span>  | <span data-ttu-id="485fc-122">string</span><span class="sxs-lookup"><span data-stu-id="485fc-122">string</span></span>  | <span data-ttu-id="485fc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="485fc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="485fc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="485fc-125">Content-Type</span></span> | <span data-ttu-id="485fc-126">string</span><span class="sxs-lookup"><span data-stu-id="485fc-126">string</span></span>  | <span data-ttu-id="485fc-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="485fc-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="485fc-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="485fc-129">Request body</span></span>

<span data-ttu-id="485fc-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="485fc-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="485fc-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="485fc-131">Parameter</span></span>    | <span data-ttu-id="485fc-132">Тип</span><span class="sxs-lookup"><span data-stu-id="485fc-132">Type</span></span>   |<span data-ttu-id="485fc-133">Описание</span><span class="sxs-lookup"><span data-stu-id="485fc-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="485fc-134">comment</span><span class="sxs-lookup"><span data-stu-id="485fc-134">comment</span></span>|<span data-ttu-id="485fc-135">String</span><span class="sxs-lookup"><span data-stu-id="485fc-135">String</span></span>|<span data-ttu-id="485fc-p104">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="485fc-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="485fc-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="485fc-138">sendResponse</span></span>|<span data-ttu-id="485fc-139">Логическое</span><span class="sxs-lookup"><span data-stu-id="485fc-139">Boolean</span></span>|<span data-ttu-id="485fc-p105">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="485fc-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="485fc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="485fc-143">Response</span></span>

<span data-ttu-id="485fc-p106">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="485fc-p106">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="485fc-146">Пример</span><span class="sxs-lookup"><span data-stu-id="485fc-146">Example</span></span>

<span data-ttu-id="485fc-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="485fc-147">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="485fc-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="485fc-148">Request</span></span>

<span data-ttu-id="485fc-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="485fc-149">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="485fc-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="485fc-150">Response</span></span>

<span data-ttu-id="485fc-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="485fc-151">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="485fc-152">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="485fc-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="485fc-153">C#</span><span class="sxs-lookup"><span data-stu-id="485fc-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/event_decline-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="485fc-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="485fc-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/event_decline-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="485fc-155">Цель — C</span><span class="sxs-lookup"><span data-stu-id="485fc-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/event_decline-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/event-decline.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/event-decline.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-decline.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
