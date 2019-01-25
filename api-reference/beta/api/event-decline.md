---
title: 'event: decline'
description: Отклонить приглашение на события, указанного в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 27b29221c741c9aca9e42009d437b2559224d832
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522156"
---
# <a name="event-decline"></a><span data-ttu-id="2d6ce-103">event: decline</span><span class="sxs-lookup"><span data-stu-id="2d6ce-103">event: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d6ce-104">Отклонить приглашение для указанного [события](../resources/event.md) в [Календарь](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d6ce-104">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2d6ce-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d6ce-105">Permissions</span></span>
<span data-ttu-id="2d6ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d6ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d6ce-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d6ce-108">Permission type</span></span>      | <span data-ttu-id="2d6ce-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d6ce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d6ce-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d6ce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2d6ce-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d6ce-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2d6ce-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d6ce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d6ce-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d6ce-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2d6ce-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d6ce-114">Application</span></span> | <span data-ttu-id="2d6ce-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d6ce-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d6ce-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d6ce-116">HTTP request</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="2d6ce-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d6ce-117">Request headers</span></span>

| <span data-ttu-id="2d6ce-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2d6ce-118">Name</span></span>       | <span data-ttu-id="2d6ce-119">Тип</span><span class="sxs-lookup"><span data-stu-id="2d6ce-119">Type</span></span> | <span data-ttu-id="2d6ce-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2d6ce-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2d6ce-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d6ce-121">Authorization</span></span>  | <span data-ttu-id="2d6ce-122">string</span><span class="sxs-lookup"><span data-stu-id="2d6ce-122">string</span></span>  | <span data-ttu-id="2d6ce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d6ce-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2d6ce-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d6ce-125">Content-Type</span></span> | <span data-ttu-id="2d6ce-126">string</span><span class="sxs-lookup"><span data-stu-id="2d6ce-126">string</span></span>  | <span data-ttu-id="2d6ce-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d6ce-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d6ce-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d6ce-129">Request body</span></span>

<span data-ttu-id="2d6ce-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2d6ce-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2d6ce-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="2d6ce-131">Parameter</span></span>    | <span data-ttu-id="2d6ce-132">Тип</span><span class="sxs-lookup"><span data-stu-id="2d6ce-132">Type</span></span>   |<span data-ttu-id="2d6ce-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2d6ce-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d6ce-134">comment</span><span class="sxs-lookup"><span data-stu-id="2d6ce-134">comment</span></span>|<span data-ttu-id="2d6ce-135">String</span><span class="sxs-lookup"><span data-stu-id="2d6ce-135">String</span></span>|<span data-ttu-id="2d6ce-p104">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="2d6ce-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="2d6ce-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="2d6ce-138">sendResponse</span></span>|<span data-ttu-id="2d6ce-139">Логическое</span><span class="sxs-lookup"><span data-stu-id="2d6ce-139">Boolean</span></span>|<span data-ttu-id="2d6ce-p105">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="2d6ce-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="2d6ce-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d6ce-143">Response</span></span>

<span data-ttu-id="2d6ce-p106">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2d6ce-p106">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d6ce-146">Пример</span><span class="sxs-lookup"><span data-stu-id="2d6ce-146">Example</span></span>

<span data-ttu-id="2d6ce-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2d6ce-147">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="2d6ce-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d6ce-148">Request</span></span>

<span data-ttu-id="2d6ce-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d6ce-149">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="2d6ce-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="2d6ce-150">Response</span></span>

<span data-ttu-id="2d6ce-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2d6ce-151">Here is an example of the response.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/event-decline.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
