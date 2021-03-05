---
title: 'event: tentativelyAccept'
description: Принятие под вопросом указанного события в календаре пользователя.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 17d7261c55af1290c1e67efe8f422f1f75c25d51
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448272"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="dd449-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="dd449-103">event: tentativelyAccept</span></span>

<span data-ttu-id="dd449-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd449-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd449-105">Предварительно принять указанное событие [в](../resources/event.md) пользовательском [календаре.](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="dd449-105">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

<span data-ttu-id="dd449-106">Если событие позволяет предложить предложения для нового времени при предварительном отклике на событие, приглашенный может выбрать альтернативное время, включив предложенный **параметрNewTime.**</span><span class="sxs-lookup"><span data-stu-id="dd449-106">If the event allows proposals for new times, on responding tentative to the event, an invitee can choose to suggest an alternative time by including the **proposedNewTime** parameter.</span></span> <span data-ttu-id="dd449-107">Дополнительные сведения о том, как предложить время, а также как получить и принять новое предложение времени, см. в дополнительных сведениях о том, как предложить [новое время собраний.](/graph/outlook-calendar-meeting-proposals)</span><span class="sxs-lookup"><span data-stu-id="dd449-107">For more information on how to propose a time, and how to receive and accept a new time proposal, see [Propose new meeting times](/graph/outlook-calendar-meeting-proposals).</span></span>

## <a name="permissions"></a><span data-ttu-id="dd449-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd449-108">Permissions</span></span>
<span data-ttu-id="dd449-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd449-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd449-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd449-111">Permission type</span></span>      | <span data-ttu-id="dd449-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd449-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd449-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd449-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dd449-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd449-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="dd449-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd449-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd449-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd449-116">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="dd449-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd449-117">Application</span></span> | <span data-ttu-id="dd449-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd449-118">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd449-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd449-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a><span data-ttu-id="dd449-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd449-120">Request headers</span></span>
| <span data-ttu-id="dd449-121">Имя</span><span class="sxs-lookup"><span data-stu-id="dd449-121">Name</span></span>       | <span data-ttu-id="dd449-122">Тип</span><span class="sxs-lookup"><span data-stu-id="dd449-122">Type</span></span> | <span data-ttu-id="dd449-123">Описание</span><span class="sxs-lookup"><span data-stu-id="dd449-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dd449-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd449-124">Authorization</span></span>  | <span data-ttu-id="dd449-125">string</span><span class="sxs-lookup"><span data-stu-id="dd449-125">string</span></span>  | <span data-ttu-id="dd449-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd449-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd449-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd449-128">Content-Type</span></span> | <span data-ttu-id="dd449-129">string</span><span class="sxs-lookup"><span data-stu-id="dd449-129">string</span></span>  | <span data-ttu-id="dd449-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd449-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd449-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd449-132">Request body</span></span>
<span data-ttu-id="dd449-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="dd449-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dd449-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="dd449-134">Parameter</span></span>    | <span data-ttu-id="dd449-135">Тип</span><span class="sxs-lookup"><span data-stu-id="dd449-135">Type</span></span>   |<span data-ttu-id="dd449-136">Описание</span><span class="sxs-lookup"><span data-stu-id="dd449-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd449-137">comment</span><span class="sxs-lookup"><span data-stu-id="dd449-137">comment</span></span>|<span data-ttu-id="dd449-138">String</span><span class="sxs-lookup"><span data-stu-id="dd449-138">String</span></span>|<span data-ttu-id="dd449-p105">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="dd449-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="dd449-141">proposedNewTime</span><span class="sxs-lookup"><span data-stu-id="dd449-141">proposedNewTime</span></span>|[<span data-ttu-id="dd449-142">timeSlot</span><span class="sxs-lookup"><span data-stu-id="dd449-142">timeSlot</span></span>](../resources/timeslot.md)|<span data-ttu-id="dd449-143">Альтернативные даты и времени, предлагаемые приглашенным для запроса на собрание, чтобы начать и закончить.</span><span class="sxs-lookup"><span data-stu-id="dd449-143">An alternate date/time proposed by an invitee for a meeting request to start and end.</span></span> <span data-ttu-id="dd449-144">Допустимо только для событий, которые позволяют новые предложения времени.</span><span class="sxs-lookup"><span data-stu-id="dd449-144">Valid only for events that allow new time proposals.</span></span> <span data-ttu-id="dd449-145">Для настройки этого параметра **необходимо установить sendResponse** для `true` .</span><span class="sxs-lookup"><span data-stu-id="dd449-145">Setting this parameter requires setting **sendResponse** to `true`.</span></span> <span data-ttu-id="dd449-146">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="dd449-146">Optional.</span></span>|
|<span data-ttu-id="dd449-147">sendResponse</span><span class="sxs-lookup"><span data-stu-id="dd449-147">sendResponse</span></span>|<span data-ttu-id="dd449-148">Логическое</span><span class="sxs-lookup"><span data-stu-id="dd449-148">Boolean</span></span>|<span data-ttu-id="dd449-p107">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="dd449-p107">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="dd449-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd449-152">Response</span></span>

<span data-ttu-id="dd449-p108">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dd449-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="dd449-155">Это действие возвращает HTTP 400, если происходит одно или оба из следующих действий:</span><span class="sxs-lookup"><span data-stu-id="dd449-155">This action returns HTTP 400 if one or both of the following occur:</span></span>

- <span data-ttu-id="dd449-156">Предлагаемый **параметрNewTime** включен, но свойство **allowNewTimeProposals** **события** `false` .</span><span class="sxs-lookup"><span data-stu-id="dd449-156">The **proposedNewTime** parameter is included but the **allowNewTimeProposals** property of the **event** is `false`.</span></span> 
- <span data-ttu-id="dd449-157">Предлагаемый **параметрNewTime** включен, но параметр **sendResponse** задан для `false` .</span><span class="sxs-lookup"><span data-stu-id="dd449-157">The **proposedNewTime** parameter is included but the **sendResponse** parameter is set to `false`.</span></span>

## <a name="example"></a><span data-ttu-id="dd449-158">Пример</span><span class="sxs-lookup"><span data-stu-id="dd449-158">Example</span></span>
<span data-ttu-id="dd449-159">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dd449-159">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="dd449-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd449-160">Request</span></span>
<span data-ttu-id="dd449-161">В следующем примере пользователь, во время записи, предварительно отвечает на указанное событие, задает параметр **sendResponse** для true и включает альтернативное время в предлагаемый **параметрNewTime.**</span><span class="sxs-lookup"><span data-stu-id="dd449-161">In the following example, the signed-in user responds tentative to the specified event, sets the **sendResponse** parameter to true, and includes an alternative time in the **proposedNewTime** parameter.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd449-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd449-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/tentativelyAccept
Content-type: application/json

{
  "comment": "I may not be able to make this week. How about next week?",
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
# <a name="c"></a>[<span data-ttu-id="dd449-163">C#</span><span class="sxs-lookup"><span data-stu-id="dd449-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-tentativelyaccept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd449-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd449-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-tentativelyaccept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd449-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd449-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-tentativelyaccept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd449-166">Java</span><span class="sxs-lookup"><span data-stu-id="dd449-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-tentativelyaccept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dd449-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd449-167">Response</span></span>
<span data-ttu-id="dd449-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dd449-168">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "event_tentativelyaccept",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

