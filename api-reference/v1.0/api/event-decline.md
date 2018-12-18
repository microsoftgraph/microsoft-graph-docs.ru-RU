---
title: 'event: decline'
description: Отклонить приглашение на события, указанного в календаре пользователя.
author: angelgolfer-ms
ms.openlocfilehash: 22051dc7f27a99a71748d20877cff6b562da6335
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322346"
---
# <a name="event-decline"></a><span data-ttu-id="cfe66-103">event: decline</span><span class="sxs-lookup"><span data-stu-id="cfe66-103">event: decline</span></span>

<span data-ttu-id="cfe66-104">Отклонить приглашение для указанного [события](../resources/event.md) в [Календарь](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="cfe66-104">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cfe66-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cfe66-105">Permissions</span></span>

<span data-ttu-id="cfe66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfe66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfe66-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cfe66-108">Permission type</span></span>      | <span data-ttu-id="cfe66-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cfe66-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfe66-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cfe66-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cfe66-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfe66-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cfe66-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cfe66-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfe66-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfe66-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cfe66-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cfe66-114">Application</span></span> | <span data-ttu-id="cfe66-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfe66-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfe66-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cfe66-116">HTTP request</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="cfe66-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cfe66-117">Request headers</span></span>

| <span data-ttu-id="cfe66-118">Имя</span><span class="sxs-lookup"><span data-stu-id="cfe66-118">Name</span></span>       | <span data-ttu-id="cfe66-119">Тип</span><span class="sxs-lookup"><span data-stu-id="cfe66-119">Type</span></span> | <span data-ttu-id="cfe66-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cfe66-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cfe66-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfe66-121">Authorization</span></span>  | <span data-ttu-id="cfe66-122">string</span><span class="sxs-lookup"><span data-stu-id="cfe66-122">string</span></span>  | <span data-ttu-id="cfe66-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfe66-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cfe66-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cfe66-125">Content-Type</span></span> | <span data-ttu-id="cfe66-126">string</span><span class="sxs-lookup"><span data-stu-id="cfe66-126">string</span></span>  | <span data-ttu-id="cfe66-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfe66-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfe66-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cfe66-129">Request body</span></span>

<span data-ttu-id="cfe66-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="cfe66-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cfe66-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="cfe66-131">Parameter</span></span>    | <span data-ttu-id="cfe66-132">Тип</span><span class="sxs-lookup"><span data-stu-id="cfe66-132">Type</span></span>   |<span data-ttu-id="cfe66-133">Описание</span><span class="sxs-lookup"><span data-stu-id="cfe66-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfe66-134">comment</span><span class="sxs-lookup"><span data-stu-id="cfe66-134">comment</span></span>|<span data-ttu-id="cfe66-135">Строка</span><span class="sxs-lookup"><span data-stu-id="cfe66-135">String</span></span>|<span data-ttu-id="cfe66-p104">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="cfe66-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="cfe66-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="cfe66-138">sendResponse</span></span>|<span data-ttu-id="cfe66-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfe66-139">Boolean</span></span>|<span data-ttu-id="cfe66-p105">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="cfe66-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="cfe66-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfe66-143">Response</span></span>

<span data-ttu-id="cfe66-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cfe66-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfe66-146">Пример</span><span class="sxs-lookup"><span data-stu-id="cfe66-146">Example</span></span>

<span data-ttu-id="cfe66-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cfe66-147">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="cfe66-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfe66-148">Request</span></span>

<span data-ttu-id="cfe66-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cfe66-149">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/decline
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

<br/>

### <a name="response"></a><span data-ttu-id="cfe66-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="cfe66-150">Response</span></span>

<span data-ttu-id="cfe66-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cfe66-151">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
