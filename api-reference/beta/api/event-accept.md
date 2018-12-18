---
title: 'event: accept'
description: Примите события, указанного в календаре пользователя.
author: angelgolfer-ms
ms.openlocfilehash: 62ca800a118331ce36ca22cc26c26391d9f186c6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320963"
---
# <a name="event-accept"></a><span data-ttu-id="9b9d6-103">event: accept</span><span class="sxs-lookup"><span data-stu-id="9b9d6-103">event: accept</span></span>

> <span data-ttu-id="9b9d6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9b9d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b9d6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b9d6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b9d6-106">Примите указанного [события](../resources/event.md) в [Календарь](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="9b9d6-106">Accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9b9d6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9b9d6-107">Permissions</span></span>
<span data-ttu-id="9b9d6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b9d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b9d6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b9d6-110">Permission type</span></span>      | <span data-ttu-id="9b9d6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b9d6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b9d6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b9d6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9b9d6-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b9d6-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="9b9d6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b9d6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b9d6-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b9d6-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="9b9d6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b9d6-116">Application</span></span> | <span data-ttu-id="9b9d6-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b9d6-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b9d6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b9d6-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="9b9d6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b9d6-119">Request headers</span></span>
| <span data-ttu-id="9b9d6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9b9d6-120">Name</span></span>       | <span data-ttu-id="9b9d6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="9b9d6-121">Type</span></span> | <span data-ttu-id="9b9d6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9b9d6-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9b9d6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b9d6-123">Authorization</span></span>  | <span data-ttu-id="9b9d6-124">string</span><span class="sxs-lookup"><span data-stu-id="9b9d6-124">string</span></span>  | <span data-ttu-id="9b9d6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b9d6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9b9d6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9b9d6-127">Content-Type</span></span> | <span data-ttu-id="9b9d6-128">string</span><span class="sxs-lookup"><span data-stu-id="9b9d6-128">string</span></span>  | <span data-ttu-id="9b9d6-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b9d6-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b9d6-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b9d6-131">Request body</span></span>
<span data-ttu-id="9b9d6-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9b9d6-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9b9d6-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="9b9d6-133">Parameter</span></span>    | <span data-ttu-id="9b9d6-134">Тип</span><span class="sxs-lookup"><span data-stu-id="9b9d6-134">Type</span></span>   |<span data-ttu-id="9b9d6-135">Описание</span><span class="sxs-lookup"><span data-stu-id="9b9d6-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b9d6-136">comment</span><span class="sxs-lookup"><span data-stu-id="9b9d6-136">comment</span></span>|<span data-ttu-id="9b9d6-137">Строка</span><span class="sxs-lookup"><span data-stu-id="9b9d6-137">String</span></span>|<span data-ttu-id="9b9d6-p105">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="9b9d6-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="9b9d6-140">sendResponse</span><span class="sxs-lookup"><span data-stu-id="9b9d6-140">sendResponse</span></span>|<span data-ttu-id="9b9d6-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b9d6-141">Boolean</span></span>|<span data-ttu-id="9b9d6-p106">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="9b9d6-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="9b9d6-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b9d6-145">Response</span></span>

<span data-ttu-id="9b9d6-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9b9d6-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b9d6-148">Пример</span><span class="sxs-lookup"><span data-stu-id="9b9d6-148">Example</span></span>
<span data-ttu-id="9b9d6-149">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9b9d6-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9b9d6-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b9d6-150">Request</span></span>
<span data-ttu-id="9b9d6-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b9d6-151">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9b9d6-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="9b9d6-152">Response</span></span>
<span data-ttu-id="9b9d6-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9b9d6-153">Here is an example of the response.</span></span>
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
