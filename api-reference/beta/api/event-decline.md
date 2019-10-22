---
title: 'event: decline'
description: Отклонение приглашения на указанное событие в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3e1e484bd3debc422890014aeb0df48806550e64
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621436"
---
# <a name="event-decline"></a><span data-ttu-id="c515c-103">event: decline</span><span class="sxs-lookup"><span data-stu-id="c515c-103">event: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c515c-104">Отклонить приглашение для указанного [события](../resources/event.md) в [календаре](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="c515c-104">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

<span data-ttu-id="c515c-105">Если событие разрешает предложения для нового времени, при отправке события приглашение можно предложить альтернативным способом, включив параметр **пропоседневтиме** .</span><span class="sxs-lookup"><span data-stu-id="c515c-105">If the event allows proposals for new times, on declining the event, an invitee can choose to suggest an alternative time by including the **proposedNewTime** parameter.</span></span> <span data-ttu-id="c515c-106">Дополнительные сведения о том, как предлагать время, а также как получать и принимать новое предложение по времени, приведены в разделе [предложение нового времени проведения собрания](/graph/outlook-calendar-meeting-proposals).</span><span class="sxs-lookup"><span data-stu-id="c515c-106">For more information on how to propose a time, and how to receive and accept a new time proposal, see [Propose new meeting times](/graph/outlook-calendar-meeting-proposals).</span></span>


## <a name="permissions"></a><span data-ttu-id="c515c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c515c-107">Permissions</span></span>
<span data-ttu-id="c515c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c515c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c515c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c515c-110">Permission type</span></span>      | <span data-ttu-id="c515c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c515c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c515c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c515c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c515c-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c515c-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c515c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c515c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c515c-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c515c-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c515c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c515c-116">Application</span></span> | <span data-ttu-id="c515c-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c515c-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c515c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c515c-118">HTTP request</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="c515c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c515c-119">Request headers</span></span>

| <span data-ttu-id="c515c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c515c-120">Name</span></span>       | <span data-ttu-id="c515c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c515c-121">Type</span></span> | <span data-ttu-id="c515c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c515c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c515c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c515c-123">Authorization</span></span>  | <span data-ttu-id="c515c-124">string</span><span class="sxs-lookup"><span data-stu-id="c515c-124">string</span></span>  | <span data-ttu-id="c515c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c515c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c515c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c515c-127">Content-Type</span></span> | <span data-ttu-id="c515c-128">string</span><span class="sxs-lookup"><span data-stu-id="c515c-128">string</span></span>  | <span data-ttu-id="c515c-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c515c-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c515c-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c515c-131">Request body</span></span>

<span data-ttu-id="c515c-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c515c-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c515c-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="c515c-133">Parameter</span></span>    | <span data-ttu-id="c515c-134">Тип</span><span class="sxs-lookup"><span data-stu-id="c515c-134">Type</span></span>   |<span data-ttu-id="c515c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="c515c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c515c-136">comment</span><span class="sxs-lookup"><span data-stu-id="c515c-136">comment</span></span>|<span data-ttu-id="c515c-137">String</span><span class="sxs-lookup"><span data-stu-id="c515c-137">String</span></span>|<span data-ttu-id="c515c-p105">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="c515c-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="c515c-140">sendResponse</span><span class="sxs-lookup"><span data-stu-id="c515c-140">sendResponse</span></span>|<span data-ttu-id="c515c-141">Логическое</span><span class="sxs-lookup"><span data-stu-id="c515c-141">Boolean</span></span>|<span data-ttu-id="c515c-p106">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="c515c-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|
|<span data-ttu-id="c515c-145">пропоседневтиме</span><span class="sxs-lookup"><span data-stu-id="c515c-145">proposedNewTime</span></span>|[<span data-ttu-id="c515c-146">timeSlot</span><span class="sxs-lookup"><span data-stu-id="c515c-146">timeSlot</span></span>](../resources/timeslot.md)|<span data-ttu-id="c515c-147">Альтернативная дата/время, предлагаемые приглашению на собрание для начала и завершения.</span><span class="sxs-lookup"><span data-stu-id="c515c-147">An alternate date/time proposed by an invitee for a meeting request to start and end.</span></span> <span data-ttu-id="c515c-148">Действует только для событий, которые допускают новые предложения времени.</span><span class="sxs-lookup"><span data-stu-id="c515c-148">Valid only for events that allow new time proposals.</span></span> <span data-ttu-id="c515c-149">Для установки этого параметра необходимо \*\*\*\* задать для `true`параметра сендреспонсе значение.</span><span class="sxs-lookup"><span data-stu-id="c515c-149">Setting this parameter requires setting **sendResponse** to `true`.</span></span> <span data-ttu-id="c515c-150">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c515c-150">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="c515c-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="c515c-151">Response</span></span>

<span data-ttu-id="c515c-p108">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c515c-p108">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="c515c-154">Это действие возвращает HTTP-400, если выполняется одно или оба следующих действия:</span><span class="sxs-lookup"><span data-stu-id="c515c-154">This action returns HTTP 400 if one or both of the following occur:</span></span>

- <span data-ttu-id="c515c-155">Параметр **пропоседневтиме** включен, но свойство **алловневтимепропосалс** **события** имеет `false`значение.</span><span class="sxs-lookup"><span data-stu-id="c515c-155">The **proposedNewTime** parameter is included but the **allowNewTimeProposals** property of the **event** is `false`.</span></span> 
- <span data-ttu-id="c515c-156">Параметр **пропоседневтиме** включен, но для `false`параметра **сендреспонсе** задано значение.</span><span class="sxs-lookup"><span data-stu-id="c515c-156">The **proposedNewTime** parameter is included but the **sendResponse** parameter is set to `false`.</span></span>

## <a name="example"></a><span data-ttu-id="c515c-157">Пример</span><span class="sxs-lookup"><span data-stu-id="c515c-157">Example</span></span>

<span data-ttu-id="c515c-158">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c515c-158">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c515c-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="c515c-159">Request</span></span>

<span data-ttu-id="c515c-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c515c-160">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c515c-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="c515c-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_decline"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/decline
Content-type: application/json

{
  "comment": "I won't be able to make this week. How about next week?",
  "sendResponse": true,
  "proposedNewTime": {
      "start": { 
          "dateTime": "2019-12-02T18:00:00", 
          "timeZone": "Pacific Standard Time" 
      }, 
      "end": { 
          "dateTime": "2019-12-02T19:00:00", 
          "timeZone": "Pacific Standard Time" 
      }     
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c515c-162">C#</span><span class="sxs-lookup"><span data-stu-id="c515c-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c515c-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c515c-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c515c-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c515c-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c515c-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="c515c-165">Response</span></span>

<span data-ttu-id="c515c-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c515c-166">Here is an example of the response.</span></span>

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
  ]
}
-->
