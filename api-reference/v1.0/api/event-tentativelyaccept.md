---
title: 'event: tentativelyAccept'
description: Примите под вопросом события, указанного в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0ab714f4f80702dd99be0dde80c9caf307c5c14c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957678"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="f4fbc-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="f4fbc-103">event: tentativelyAccept</span></span>

<span data-ttu-id="f4fbc-104">Примите под вопросом указанного [события](../resources/event.md) в [Календарь](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4fbc-104">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f4fbc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4fbc-105">Permissions</span></span>
<span data-ttu-id="f4fbc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4fbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4fbc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4fbc-108">Permission type</span></span>      | <span data-ttu-id="f4fbc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4fbc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4fbc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4fbc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f4fbc-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4fbc-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f4fbc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4fbc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4fbc-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4fbc-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f4fbc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4fbc-114">Application</span></span> | <span data-ttu-id="f4fbc-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4fbc-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4fbc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4fbc-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="f4fbc-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4fbc-117">Request headers</span></span>
| <span data-ttu-id="f4fbc-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f4fbc-118">Name</span></span>       | <span data-ttu-id="f4fbc-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f4fbc-119">Type</span></span> | <span data-ttu-id="f4fbc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f4fbc-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f4fbc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4fbc-121">Authorization</span></span>  | <span data-ttu-id="f4fbc-122">string</span><span class="sxs-lookup"><span data-stu-id="f4fbc-122">string</span></span>  | <span data-ttu-id="f4fbc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4fbc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f4fbc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f4fbc-125">Content-Type</span></span> | <span data-ttu-id="f4fbc-126">string</span><span class="sxs-lookup"><span data-stu-id="f4fbc-126">string</span></span>  | <span data-ttu-id="f4fbc-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4fbc-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4fbc-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f4fbc-129">Request body</span></span>
<span data-ttu-id="f4fbc-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f4fbc-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f4fbc-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="f4fbc-131">Parameter</span></span>    | <span data-ttu-id="f4fbc-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f4fbc-132">Type</span></span>   |<span data-ttu-id="f4fbc-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f4fbc-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4fbc-134">comment</span><span class="sxs-lookup"><span data-stu-id="f4fbc-134">comment</span></span>|<span data-ttu-id="f4fbc-135">Строка</span><span class="sxs-lookup"><span data-stu-id="f4fbc-135">String</span></span>|<span data-ttu-id="f4fbc-p104">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="f4fbc-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="f4fbc-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="f4fbc-138">sendResponse</span></span>|<span data-ttu-id="f4fbc-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4fbc-139">Boolean</span></span>|<span data-ttu-id="f4fbc-p105">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="f4fbc-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="f4fbc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4fbc-143">Response</span></span>

<span data-ttu-id="f4fbc-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f4fbc-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4fbc-146">Пример</span><span class="sxs-lookup"><span data-stu-id="f4fbc-146">Example</span></span>
<span data-ttu-id="f4fbc-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f4fbc-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f4fbc-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4fbc-148">Request</span></span>
<span data-ttu-id="f4fbc-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4fbc-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f4fbc-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4fbc-150">Response</span></span>
##### <a name="response"></a><span data-ttu-id="f4fbc-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4fbc-151">Response</span></span>
<span data-ttu-id="f4fbc-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f4fbc-152">Here is an example of the response.</span></span>
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
