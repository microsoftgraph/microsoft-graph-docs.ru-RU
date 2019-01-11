---
title: 'event: decline'
description: Отклонить приглашение на события, указанного в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 218ca79b05507fc63ba6f45e2fcb5dd4a0835361
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866957"
---
# <a name="event-decline"></a><span data-ttu-id="35e6e-103">event: decline</span><span class="sxs-lookup"><span data-stu-id="35e6e-103">event: decline</span></span>

> <span data-ttu-id="35e6e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="35e6e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35e6e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35e6e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35e6e-106">Отклонить приглашение для указанного [события](../resources/event.md) в [Календарь](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="35e6e-106">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="35e6e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35e6e-107">Permissions</span></span>
<span data-ttu-id="35e6e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35e6e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35e6e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35e6e-110">Permission type</span></span>      | <span data-ttu-id="35e6e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35e6e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35e6e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35e6e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="35e6e-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35e6e-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="35e6e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35e6e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35e6e-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35e6e-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="35e6e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35e6e-116">Application</span></span> | <span data-ttu-id="35e6e-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35e6e-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="35e6e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35e6e-118">HTTP request</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="35e6e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35e6e-119">Request headers</span></span>

| <span data-ttu-id="35e6e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="35e6e-120">Name</span></span>       | <span data-ttu-id="35e6e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="35e6e-121">Type</span></span> | <span data-ttu-id="35e6e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="35e6e-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="35e6e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="35e6e-123">Authorization</span></span>  | <span data-ttu-id="35e6e-124">string</span><span class="sxs-lookup"><span data-stu-id="35e6e-124">string</span></span>  | <span data-ttu-id="35e6e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35e6e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="35e6e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35e6e-127">Content-Type</span></span> | <span data-ttu-id="35e6e-128">string</span><span class="sxs-lookup"><span data-stu-id="35e6e-128">string</span></span>  | <span data-ttu-id="35e6e-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35e6e-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35e6e-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="35e6e-131">Request body</span></span>

<span data-ttu-id="35e6e-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="35e6e-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="35e6e-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="35e6e-133">Parameter</span></span>    | <span data-ttu-id="35e6e-134">Тип</span><span class="sxs-lookup"><span data-stu-id="35e6e-134">Type</span></span>   |<span data-ttu-id="35e6e-135">Описание</span><span class="sxs-lookup"><span data-stu-id="35e6e-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35e6e-136">comment</span><span class="sxs-lookup"><span data-stu-id="35e6e-136">comment</span></span>|<span data-ttu-id="35e6e-137">Строка</span><span class="sxs-lookup"><span data-stu-id="35e6e-137">String</span></span>|<span data-ttu-id="35e6e-p105">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="35e6e-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="35e6e-140">sendResponse</span><span class="sxs-lookup"><span data-stu-id="35e6e-140">sendResponse</span></span>|<span data-ttu-id="35e6e-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="35e6e-141">Boolean</span></span>|<span data-ttu-id="35e6e-p106">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="35e6e-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="35e6e-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="35e6e-145">Response</span></span>

<span data-ttu-id="35e6e-p107">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="35e6e-p107">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35e6e-148">Пример</span><span class="sxs-lookup"><span data-stu-id="35e6e-148">Example</span></span>

<span data-ttu-id="35e6e-149">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="35e6e-149">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="35e6e-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="35e6e-150">Request</span></span>

<span data-ttu-id="35e6e-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35e6e-151">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="35e6e-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="35e6e-152">Response</span></span>

<span data-ttu-id="35e6e-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="35e6e-153">Here is an example of the response.</span></span>

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
  "description": "event: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
