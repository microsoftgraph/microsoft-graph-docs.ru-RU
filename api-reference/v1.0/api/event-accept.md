---
title: 'event: accept'
description: Примите события, указанного в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 0ff048863f1e2077967c995e7e8806f6df7716ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814884"
---
# <a name="event-accept"></a><span data-ttu-id="317cc-103">event: accept</span><span class="sxs-lookup"><span data-stu-id="317cc-103">event: accept</span></span>

<span data-ttu-id="317cc-104">Примите указанного [события](../resources/event.md) в [Календарь](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="317cc-104">Accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="317cc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="317cc-105">Permissions</span></span>
<span data-ttu-id="317cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="317cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="317cc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="317cc-108">Permission type</span></span>      | <span data-ttu-id="317cc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="317cc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="317cc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="317cc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="317cc-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="317cc-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="317cc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="317cc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="317cc-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="317cc-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="317cc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="317cc-114">Application</span></span> | <span data-ttu-id="317cc-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="317cc-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="317cc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="317cc-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="317cc-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="317cc-117">Request headers</span></span>
| <span data-ttu-id="317cc-118">Имя</span><span class="sxs-lookup"><span data-stu-id="317cc-118">Name</span></span>       | <span data-ttu-id="317cc-119">Тип</span><span class="sxs-lookup"><span data-stu-id="317cc-119">Type</span></span> | <span data-ttu-id="317cc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="317cc-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="317cc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="317cc-121">Authorization</span></span>  | <span data-ttu-id="317cc-122">string</span><span class="sxs-lookup"><span data-stu-id="317cc-122">string</span></span>  | <span data-ttu-id="317cc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="317cc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="317cc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="317cc-125">Content-Type</span></span> | <span data-ttu-id="317cc-126">string</span><span class="sxs-lookup"><span data-stu-id="317cc-126">string</span></span>  | <span data-ttu-id="317cc-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="317cc-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="317cc-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="317cc-129">Request body</span></span>
<span data-ttu-id="317cc-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="317cc-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="317cc-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="317cc-131">Parameter</span></span>    | <span data-ttu-id="317cc-132">Тип</span><span class="sxs-lookup"><span data-stu-id="317cc-132">Type</span></span>   |<span data-ttu-id="317cc-133">Описание</span><span class="sxs-lookup"><span data-stu-id="317cc-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="317cc-134">comment</span><span class="sxs-lookup"><span data-stu-id="317cc-134">comment</span></span>|<span data-ttu-id="317cc-135">Строка</span><span class="sxs-lookup"><span data-stu-id="317cc-135">String</span></span>|<span data-ttu-id="317cc-p104">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="317cc-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="317cc-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="317cc-138">sendResponse</span></span>|<span data-ttu-id="317cc-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="317cc-139">Boolean</span></span>|<span data-ttu-id="317cc-p105">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="317cc-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="317cc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="317cc-143">Response</span></span>

<span data-ttu-id="317cc-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="317cc-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="317cc-146">Пример</span><span class="sxs-lookup"><span data-stu-id="317cc-146">Example</span></span>
<span data-ttu-id="317cc-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="317cc-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="317cc-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="317cc-148">Request</span></span>
<span data-ttu-id="317cc-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="317cc-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="317cc-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="317cc-150">Response</span></span>
<span data-ttu-id="317cc-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="317cc-151">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->
