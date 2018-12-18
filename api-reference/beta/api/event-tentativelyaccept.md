---
title: 'event: tentativelyAccept'
description: Примите под вопросом события, указанного в календаре пользователя.
author: angelgolfer-ms
ms.openlocfilehash: 99e0060f087140869614737296c9684cf3f1c189
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318216"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="571ed-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="571ed-103">event: tentativelyAccept</span></span>

> <span data-ttu-id="571ed-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="571ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="571ed-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="571ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="571ed-106">Примите под вопросом указанного [события](../resources/event.md) в [Календарь](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="571ed-106">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="571ed-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="571ed-107">Permissions</span></span>
<span data-ttu-id="571ed-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="571ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="571ed-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="571ed-110">Permission type</span></span>      | <span data-ttu-id="571ed-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="571ed-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="571ed-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="571ed-112">Delegated (work or school account)</span></span> | <span data-ttu-id="571ed-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="571ed-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="571ed-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="571ed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="571ed-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="571ed-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="571ed-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="571ed-116">Application</span></span> | <span data-ttu-id="571ed-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="571ed-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="571ed-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="571ed-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="571ed-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="571ed-119">Request headers</span></span>
| <span data-ttu-id="571ed-120">Имя</span><span class="sxs-lookup"><span data-stu-id="571ed-120">Name</span></span>       | <span data-ttu-id="571ed-121">Тип</span><span class="sxs-lookup"><span data-stu-id="571ed-121">Type</span></span> | <span data-ttu-id="571ed-122">Описание</span><span class="sxs-lookup"><span data-stu-id="571ed-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="571ed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="571ed-123">Authorization</span></span>  | <span data-ttu-id="571ed-124">string</span><span class="sxs-lookup"><span data-stu-id="571ed-124">string</span></span>  | <span data-ttu-id="571ed-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="571ed-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="571ed-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="571ed-127">Content-Type</span></span> | <span data-ttu-id="571ed-128">string</span><span class="sxs-lookup"><span data-stu-id="571ed-128">string</span></span>  | <span data-ttu-id="571ed-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="571ed-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="571ed-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="571ed-131">Request body</span></span>
<span data-ttu-id="571ed-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="571ed-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="571ed-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="571ed-133">Parameter</span></span>    | <span data-ttu-id="571ed-134">Тип</span><span class="sxs-lookup"><span data-stu-id="571ed-134">Type</span></span>   |<span data-ttu-id="571ed-135">Описание</span><span class="sxs-lookup"><span data-stu-id="571ed-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="571ed-136">comment</span><span class="sxs-lookup"><span data-stu-id="571ed-136">comment</span></span>|<span data-ttu-id="571ed-137">Строка</span><span class="sxs-lookup"><span data-stu-id="571ed-137">String</span></span>|<span data-ttu-id="571ed-p105">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="571ed-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="571ed-140">sendResponse</span><span class="sxs-lookup"><span data-stu-id="571ed-140">sendResponse</span></span>|<span data-ttu-id="571ed-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="571ed-141">Boolean</span></span>|<span data-ttu-id="571ed-p106">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="571ed-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="571ed-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="571ed-145">Response</span></span>

<span data-ttu-id="571ed-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="571ed-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="571ed-148">Пример</span><span class="sxs-lookup"><span data-stu-id="571ed-148">Example</span></span>
<span data-ttu-id="571ed-149">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="571ed-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="571ed-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="571ed-150">Request</span></span>
<span data-ttu-id="571ed-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="571ed-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/tentativelyAccept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="571ed-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="571ed-152">Response</span></span>
##### <a name="response"></a><span data-ttu-id="571ed-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="571ed-153">Response</span></span>
<span data-ttu-id="571ed-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="571ed-154">Here is an example of the response.</span></span>
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
