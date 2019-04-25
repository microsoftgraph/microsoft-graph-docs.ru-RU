---
title: 'event: tentativelyAccept'
description: Принятие под вопросом указанного события в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0ab714f4f80702dd99be0dde80c9caf307c5c14c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584329"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="4a27a-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="4a27a-103">event: tentativelyAccept</span></span>

<span data-ttu-id="4a27a-104">Предварительно принять указанное [событие](../resources/event.md) в календаре пользователя [](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="4a27a-104">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a27a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a27a-105">Permissions</span></span>
<span data-ttu-id="4a27a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a27a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a27a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a27a-108">Permission type</span></span>      | <span data-ttu-id="4a27a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a27a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a27a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a27a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4a27a-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a27a-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4a27a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a27a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a27a-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a27a-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4a27a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a27a-114">Application</span></span> | <span data-ttu-id="4a27a-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a27a-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a27a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a27a-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="4a27a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a27a-117">Request headers</span></span>
| <span data-ttu-id="4a27a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4a27a-118">Name</span></span>       | <span data-ttu-id="4a27a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="4a27a-119">Type</span></span> | <span data-ttu-id="4a27a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4a27a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4a27a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a27a-121">Authorization</span></span>  | <span data-ttu-id="4a27a-122">string</span><span class="sxs-lookup"><span data-stu-id="4a27a-122">string</span></span>  | <span data-ttu-id="4a27a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a27a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a27a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4a27a-125">Content-Type</span></span> | <span data-ttu-id="4a27a-126">string</span><span class="sxs-lookup"><span data-stu-id="4a27a-126">string</span></span>  | <span data-ttu-id="4a27a-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a27a-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a27a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a27a-129">Request body</span></span>
<span data-ttu-id="4a27a-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4a27a-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4a27a-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="4a27a-131">Parameter</span></span>    | <span data-ttu-id="4a27a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4a27a-132">Type</span></span>   |<span data-ttu-id="4a27a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4a27a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a27a-134">comment</span><span class="sxs-lookup"><span data-stu-id="4a27a-134">comment</span></span>|<span data-ttu-id="4a27a-135">String</span><span class="sxs-lookup"><span data-stu-id="4a27a-135">String</span></span>|<span data-ttu-id="4a27a-p104">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="4a27a-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="4a27a-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="4a27a-138">sendResponse</span></span>|<span data-ttu-id="4a27a-139">Логическое</span><span class="sxs-lookup"><span data-stu-id="4a27a-139">Boolean</span></span>|<span data-ttu-id="4a27a-p105">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="4a27a-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="4a27a-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a27a-143">Response</span></span>

<span data-ttu-id="4a27a-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4a27a-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a27a-146">Пример</span><span class="sxs-lookup"><span data-stu-id="4a27a-146">Example</span></span>
<span data-ttu-id="4a27a-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4a27a-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4a27a-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a27a-148">Request</span></span>
<span data-ttu-id="4a27a-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a27a-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="4a27a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a27a-150">Response</span></span>
##### <a name="response"></a><span data-ttu-id="4a27a-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a27a-151">Response</span></span>
<span data-ttu-id="4a27a-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a27a-152">Here is an example of the response.</span></span>
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
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
