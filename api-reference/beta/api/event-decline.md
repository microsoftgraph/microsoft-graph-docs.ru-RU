---
title: 'event: decline'
description: Отклонение приглашения на указанное событие в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 54c0f64bffa172ff8a4c9388bcf8f014bbf71e64
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325090"
---
# <a name="event-decline"></a><span data-ttu-id="59734-103">event: decline</span><span class="sxs-lookup"><span data-stu-id="59734-103">event: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59734-104">ОтКлонить приглашение для указанного [события](../resources/event.md) в [календаре](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="59734-104">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="59734-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59734-105">Permissions</span></span>
<span data-ttu-id="59734-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59734-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59734-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59734-108">Permission type</span></span>      | <span data-ttu-id="59734-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59734-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59734-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59734-110">Delegated (work or school account)</span></span> | <span data-ttu-id="59734-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59734-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="59734-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59734-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59734-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59734-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="59734-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59734-114">Application</span></span> | <span data-ttu-id="59734-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59734-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="59734-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59734-116">HTTP request</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="59734-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59734-117">Request headers</span></span>

| <span data-ttu-id="59734-118">Имя</span><span class="sxs-lookup"><span data-stu-id="59734-118">Name</span></span>       | <span data-ttu-id="59734-119">Тип</span><span class="sxs-lookup"><span data-stu-id="59734-119">Type</span></span> | <span data-ttu-id="59734-120">Описание</span><span class="sxs-lookup"><span data-stu-id="59734-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="59734-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="59734-121">Authorization</span></span>  | <span data-ttu-id="59734-122">string</span><span class="sxs-lookup"><span data-stu-id="59734-122">string</span></span>  | <span data-ttu-id="59734-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59734-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59734-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59734-125">Content-Type</span></span> | <span data-ttu-id="59734-126">string</span><span class="sxs-lookup"><span data-stu-id="59734-126">string</span></span>  | <span data-ttu-id="59734-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59734-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59734-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59734-129">Request body</span></span>

<span data-ttu-id="59734-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="59734-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="59734-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="59734-131">Parameter</span></span>    | <span data-ttu-id="59734-132">Тип</span><span class="sxs-lookup"><span data-stu-id="59734-132">Type</span></span>   |<span data-ttu-id="59734-133">Описание</span><span class="sxs-lookup"><span data-stu-id="59734-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59734-134">comment</span><span class="sxs-lookup"><span data-stu-id="59734-134">comment</span></span>|<span data-ttu-id="59734-135">String</span><span class="sxs-lookup"><span data-stu-id="59734-135">String</span></span>|<span data-ttu-id="59734-p104">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="59734-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="59734-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="59734-138">sendResponse</span></span>|<span data-ttu-id="59734-139">Логическое</span><span class="sxs-lookup"><span data-stu-id="59734-139">Boolean</span></span>|<span data-ttu-id="59734-p105">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="59734-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="59734-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="59734-143">Response</span></span>

<span data-ttu-id="59734-p106">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="59734-p106">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59734-146">Пример</span><span class="sxs-lookup"><span data-stu-id="59734-146">Example</span></span>

<span data-ttu-id="59734-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="59734-147">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="59734-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="59734-148">Request</span></span>

<span data-ttu-id="59734-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59734-149">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="59734-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="59734-150">Response</span></span>

<span data-ttu-id="59734-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="59734-151">Here is an example of the response.</span></span>

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
  "suppressions": []
}
-->
