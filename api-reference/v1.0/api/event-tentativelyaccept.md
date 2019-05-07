---
title: 'event: tentativelyAccept'
description: Принятие под вопросом указанного события в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4fbac7d01f95fda42dac579cb3cd43ed1aa29f93
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33615098"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="20dd9-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="20dd9-103">event: tentativelyAccept</span></span>

<span data-ttu-id="20dd9-104">Предварительно принять указанное [событие](../resources/event.md) в календаре пользователя [](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="20dd9-104">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="20dd9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20dd9-105">Permissions</span></span>
<span data-ttu-id="20dd9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20dd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20dd9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20dd9-108">Permission type</span></span>      | <span data-ttu-id="20dd9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20dd9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20dd9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20dd9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="20dd9-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20dd9-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="20dd9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20dd9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20dd9-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20dd9-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="20dd9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20dd9-114">Application</span></span> | <span data-ttu-id="20dd9-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20dd9-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="20dd9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20dd9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroup/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a><span data-ttu-id="20dd9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20dd9-117">Request headers</span></span>
| <span data-ttu-id="20dd9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="20dd9-118">Name</span></span>       | <span data-ttu-id="20dd9-119">Тип</span><span class="sxs-lookup"><span data-stu-id="20dd9-119">Type</span></span> | <span data-ttu-id="20dd9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="20dd9-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="20dd9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="20dd9-121">Authorization</span></span>  | <span data-ttu-id="20dd9-122">string</span><span class="sxs-lookup"><span data-stu-id="20dd9-122">string</span></span>  | <span data-ttu-id="20dd9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20dd9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20dd9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="20dd9-125">Content-Type</span></span> | <span data-ttu-id="20dd9-126">string</span><span class="sxs-lookup"><span data-stu-id="20dd9-126">string</span></span>  | <span data-ttu-id="20dd9-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20dd9-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20dd9-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20dd9-129">Request body</span></span>
<span data-ttu-id="20dd9-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="20dd9-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="20dd9-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="20dd9-131">Parameter</span></span>    | <span data-ttu-id="20dd9-132">Тип</span><span class="sxs-lookup"><span data-stu-id="20dd9-132">Type</span></span>   |<span data-ttu-id="20dd9-133">Описание</span><span class="sxs-lookup"><span data-stu-id="20dd9-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20dd9-134">comment</span><span class="sxs-lookup"><span data-stu-id="20dd9-134">comment</span></span>|<span data-ttu-id="20dd9-135">String</span><span class="sxs-lookup"><span data-stu-id="20dd9-135">String</span></span>|<span data-ttu-id="20dd9-p104">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="20dd9-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="20dd9-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="20dd9-138">sendResponse</span></span>|<span data-ttu-id="20dd9-139">Логическое</span><span class="sxs-lookup"><span data-stu-id="20dd9-139">Boolean</span></span>|<span data-ttu-id="20dd9-p105">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="20dd9-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="20dd9-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="20dd9-143">Response</span></span>

<span data-ttu-id="20dd9-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="20dd9-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20dd9-146">Пример</span><span class="sxs-lookup"><span data-stu-id="20dd9-146">Example</span></span>
<span data-ttu-id="20dd9-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="20dd9-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="20dd9-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="20dd9-148">Request</span></span>
<span data-ttu-id="20dd9-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20dd9-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/tentativelyAccept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="20dd9-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="20dd9-150">Response</span></span>
##### <a name="response"></a><span data-ttu-id="20dd9-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="20dd9-151">Response</span></span>
<span data-ttu-id="20dd9-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="20dd9-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="20dd9-153">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="20dd9-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="20dd9-154">Языках</span><span class="sxs-lookup"><span data-stu-id="20dd9-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/event_tentativelyaccept-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20dd9-155">Язык</span><span class="sxs-lookup"><span data-stu-id="20dd9-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/event_tentativelyaccept-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/event-tentativelyaccept.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/event-tentativelyaccept.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
