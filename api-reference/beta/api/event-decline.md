---
title: 'event: decline'
description: Отклонение приглашения на указанное событие в календаре пользователя.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8d3aab12dcc48fc16a5d57fbc7a06f64c422c962
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436269"
---
# <a name="event-decline"></a><span data-ttu-id="deb0c-103">event: decline</span><span class="sxs-lookup"><span data-stu-id="deb0c-103">event: decline</span></span>

<span data-ttu-id="deb0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deb0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="deb0c-105">Отклонение приглашения на указанное [событие](../resources/event.md) в календаре [пользователей.](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="deb0c-105">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

<span data-ttu-id="deb0c-106">Если событие позволяет предложить предложения для нового времени при отклонении события, приглашенный может выбрать альтернативное время, включив предложенный **параметрNewTime.**</span><span class="sxs-lookup"><span data-stu-id="deb0c-106">If the event allows proposals for new times, on declining the event, an invitee can choose to suggest an alternative time by including the **proposedNewTime** parameter.</span></span> <span data-ttu-id="deb0c-107">Дополнительные сведения о том, как предложить время, а также как получить и принять новое предложение времени, см. в дополнительных сведениях о том, как предложить [новое время собраний.](/graph/outlook-calendar-meeting-proposals)</span><span class="sxs-lookup"><span data-stu-id="deb0c-107">For more information on how to propose a time, and how to receive and accept a new time proposal, see [Propose new meeting times](/graph/outlook-calendar-meeting-proposals).</span></span>


## <a name="permissions"></a><span data-ttu-id="deb0c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="deb0c-108">Permissions</span></span>
<span data-ttu-id="deb0c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="deb0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="deb0c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="deb0c-111">Permission type</span></span>      | <span data-ttu-id="deb0c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="deb0c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="deb0c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="deb0c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="deb0c-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="deb0c-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="deb0c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="deb0c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="deb0c-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="deb0c-116">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="deb0c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="deb0c-117">Application</span></span> | <span data-ttu-id="deb0c-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="deb0c-118">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="deb0c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="deb0c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/decline
POST /users/{id | userPrincipalName}/events/{id}/decline

POST /me/calendar/events/{id}/decline
POST /users/{id | userPrincipalName}/calendar/events/{id}/decline

POST /me/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/decline

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/decline
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="deb0c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="deb0c-120">Request headers</span></span>

| <span data-ttu-id="deb0c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="deb0c-121">Name</span></span>       | <span data-ttu-id="deb0c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="deb0c-122">Type</span></span> | <span data-ttu-id="deb0c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="deb0c-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="deb0c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="deb0c-124">Authorization</span></span>  | <span data-ttu-id="deb0c-125">string</span><span class="sxs-lookup"><span data-stu-id="deb0c-125">string</span></span>  | <span data-ttu-id="deb0c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="deb0c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="deb0c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="deb0c-128">Content-Type</span></span> | <span data-ttu-id="deb0c-129">string</span><span class="sxs-lookup"><span data-stu-id="deb0c-129">string</span></span>  | <span data-ttu-id="deb0c-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="deb0c-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="deb0c-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="deb0c-132">Request body</span></span>

<span data-ttu-id="deb0c-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="deb0c-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="deb0c-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="deb0c-134">Parameter</span></span>    | <span data-ttu-id="deb0c-135">Тип</span><span class="sxs-lookup"><span data-stu-id="deb0c-135">Type</span></span>   |<span data-ttu-id="deb0c-136">Описание</span><span class="sxs-lookup"><span data-stu-id="deb0c-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="deb0c-137">comment</span><span class="sxs-lookup"><span data-stu-id="deb0c-137">comment</span></span>|<span data-ttu-id="deb0c-138">String</span><span class="sxs-lookup"><span data-stu-id="deb0c-138">String</span></span>|<span data-ttu-id="deb0c-p105">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="deb0c-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="deb0c-141">sendResponse</span><span class="sxs-lookup"><span data-stu-id="deb0c-141">sendResponse</span></span>|<span data-ttu-id="deb0c-142">Логическое</span><span class="sxs-lookup"><span data-stu-id="deb0c-142">Boolean</span></span>|<span data-ttu-id="deb0c-p106">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="deb0c-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|
|<span data-ttu-id="deb0c-146">proposedNewTime</span><span class="sxs-lookup"><span data-stu-id="deb0c-146">proposedNewTime</span></span>|[<span data-ttu-id="deb0c-147">timeSlot</span><span class="sxs-lookup"><span data-stu-id="deb0c-147">timeSlot</span></span>](../resources/timeslot.md)|<span data-ttu-id="deb0c-148">Альтернативные даты и времени, предлагаемые приглашенным для запроса на собрание, чтобы начать и закончить.</span><span class="sxs-lookup"><span data-stu-id="deb0c-148">An alternate date/time proposed by an invitee for a meeting request to start and end.</span></span> <span data-ttu-id="deb0c-149">Допустимо только для событий, которые позволяют новые предложения времени.</span><span class="sxs-lookup"><span data-stu-id="deb0c-149">Valid only for events that allow new time proposals.</span></span> <span data-ttu-id="deb0c-150">Для настройки этого параметра **необходимо установить sendResponse** для `true` .</span><span class="sxs-lookup"><span data-stu-id="deb0c-150">Setting this parameter requires setting **sendResponse** to `true`.</span></span> <span data-ttu-id="deb0c-151">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="deb0c-151">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="deb0c-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="deb0c-152">Response</span></span>

<span data-ttu-id="deb0c-p108">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="deb0c-p108">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="deb0c-155">Это действие возвращает HTTP 400, если происходит одно или оба из следующих действий:</span><span class="sxs-lookup"><span data-stu-id="deb0c-155">This action returns HTTP 400 if one or both of the following occur:</span></span>

- <span data-ttu-id="deb0c-156">Предлагаемый **параметрNewTime** включен, но свойство **allowNewTimeProposals** **события** `false` .</span><span class="sxs-lookup"><span data-stu-id="deb0c-156">The **proposedNewTime** parameter is included but the **allowNewTimeProposals** property of the **event** is `false`.</span></span> 
- <span data-ttu-id="deb0c-157">Предлагаемый **параметрNewTime** включен, но параметр **sendResponse** задан для `false` .</span><span class="sxs-lookup"><span data-stu-id="deb0c-157">The **proposedNewTime** parameter is included but the **sendResponse** parameter is set to `false`.</span></span>

## <a name="example"></a><span data-ttu-id="deb0c-158">Пример</span><span class="sxs-lookup"><span data-stu-id="deb0c-158">Example</span></span>

<span data-ttu-id="deb0c-159">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="deb0c-159">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="deb0c-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="deb0c-160">Request</span></span>

<span data-ttu-id="deb0c-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="deb0c-161">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="deb0c-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="deb0c-162">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="deb0c-163">C#</span><span class="sxs-lookup"><span data-stu-id="deb0c-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="deb0c-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="deb0c-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="deb0c-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="deb0c-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="deb0c-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="deb0c-166">Response</span></span>

<span data-ttu-id="deb0c-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="deb0c-167">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
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


