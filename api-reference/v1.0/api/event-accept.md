---
title: 'event: accept'
description: Принятие указанного события в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0c75f000021e18f2d8b76cb99c7dfc308a7310ee
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33615601"
---
# <a name="event-accept"></a><span data-ttu-id="34a3e-103">event: accept</span><span class="sxs-lookup"><span data-stu-id="34a3e-103">event: accept</span></span>

<span data-ttu-id="34a3e-104">Принять указанное [событие](../resources/event.md) в календаре пользователя [](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="34a3e-104">Accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="34a3e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34a3e-105">Permissions</span></span>
<span data-ttu-id="34a3e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34a3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34a3e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34a3e-108">Permission type</span></span>      | <span data-ttu-id="34a3e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34a3e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34a3e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34a3e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="34a3e-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34a3e-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="34a3e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34a3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34a3e-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34a3e-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="34a3e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34a3e-114">Application</span></span> | <span data-ttu-id="34a3e-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34a3e-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="34a3e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34a3e-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="34a3e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34a3e-117">Request headers</span></span>
| <span data-ttu-id="34a3e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="34a3e-118">Name</span></span>       | <span data-ttu-id="34a3e-119">Тип</span><span class="sxs-lookup"><span data-stu-id="34a3e-119">Type</span></span> | <span data-ttu-id="34a3e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="34a3e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="34a3e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="34a3e-121">Authorization</span></span>  | <span data-ttu-id="34a3e-122">string</span><span class="sxs-lookup"><span data-stu-id="34a3e-122">string</span></span>  | <span data-ttu-id="34a3e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34a3e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34a3e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="34a3e-125">Content-Type</span></span> | <span data-ttu-id="34a3e-126">string</span><span class="sxs-lookup"><span data-stu-id="34a3e-126">string</span></span>  | <span data-ttu-id="34a3e-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34a3e-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34a3e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34a3e-129">Request body</span></span>
<span data-ttu-id="34a3e-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="34a3e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="34a3e-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="34a3e-131">Parameter</span></span>    | <span data-ttu-id="34a3e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="34a3e-132">Type</span></span>   |<span data-ttu-id="34a3e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="34a3e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34a3e-134">comment</span><span class="sxs-lookup"><span data-stu-id="34a3e-134">comment</span></span>|<span data-ttu-id="34a3e-135">String</span><span class="sxs-lookup"><span data-stu-id="34a3e-135">String</span></span>|<span data-ttu-id="34a3e-p104">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="34a3e-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="34a3e-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="34a3e-138">sendResponse</span></span>|<span data-ttu-id="34a3e-139">Логическое</span><span class="sxs-lookup"><span data-stu-id="34a3e-139">Boolean</span></span>|<span data-ttu-id="34a3e-p105">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="34a3e-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="34a3e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="34a3e-143">Response</span></span>

<span data-ttu-id="34a3e-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="34a3e-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34a3e-146">Пример</span><span class="sxs-lookup"><span data-stu-id="34a3e-146">Example</span></span>
<span data-ttu-id="34a3e-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="34a3e-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="34a3e-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="34a3e-148">Request</span></span>
<span data-ttu-id="34a3e-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34a3e-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="34a3e-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="34a3e-150">Response</span></span>
<span data-ttu-id="34a3e-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="34a3e-151">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="34a3e-152">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="34a3e-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="34a3e-153">Языках</span><span class="sxs-lookup"><span data-stu-id="34a3e-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/event_accept-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="34a3e-154">Язык</span><span class="sxs-lookup"><span data-stu-id="34a3e-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/event_accept-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: accept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/event-accept.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/event-accept.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
