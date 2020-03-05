---
title: 'event: tentativelyAccept'
description: Принятие под вопросом указанного события в календаре пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b3e9f5510499e1ab6d015cd58e1e97a8eabac995
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422686"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="7fff4-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="7fff4-103">event: tentativelyAccept</span></span>

<span data-ttu-id="7fff4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7fff4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fff4-105">Предварительно принять указанное [событие](../resources/event.md) в [календаре](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="7fff4-105">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

<span data-ttu-id="7fff4-106">Если событие позволяет создавать предложения для нового времени, при отклике на запрос о событии приглашение можно предложить альтернативное время, включив параметр **пропоседневтиме** .</span><span class="sxs-lookup"><span data-stu-id="7fff4-106">If the event allows proposals for new times, on responding tentative to the event, an invitee can choose to suggest an alternative time by including the **proposedNewTime** parameter.</span></span> <span data-ttu-id="7fff4-107">Дополнительные сведения о том, как предлагать время, а также как получать и принимать новое предложение по времени, приведены в разделе [предложение нового времени проведения собрания](/graph/outlook-calendar-meeting-proposals).</span><span class="sxs-lookup"><span data-stu-id="7fff4-107">For more information on how to propose a time, and how to receive and accept a new time proposal, see [Propose new meeting times](/graph/outlook-calendar-meeting-proposals).</span></span>

## <a name="permissions"></a><span data-ttu-id="7fff4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7fff4-108">Permissions</span></span>
<span data-ttu-id="7fff4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fff4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fff4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fff4-111">Permission type</span></span>      | <span data-ttu-id="7fff4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fff4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fff4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fff4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7fff4-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7fff4-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7fff4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fff4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fff4-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7fff4-116">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7fff4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fff4-117">Application</span></span> | <span data-ttu-id="7fff4-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7fff4-118">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fff4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fff4-119">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="7fff4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7fff4-120">Request headers</span></span>
| <span data-ttu-id="7fff4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="7fff4-121">Name</span></span>       | <span data-ttu-id="7fff4-122">Тип</span><span class="sxs-lookup"><span data-stu-id="7fff4-122">Type</span></span> | <span data-ttu-id="7fff4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7fff4-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7fff4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fff4-124">Authorization</span></span>  | <span data-ttu-id="7fff4-125">string</span><span class="sxs-lookup"><span data-stu-id="7fff4-125">string</span></span>  | <span data-ttu-id="7fff4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7fff4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7fff4-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7fff4-128">Content-Type</span></span> | <span data-ttu-id="7fff4-129">string</span><span class="sxs-lookup"><span data-stu-id="7fff4-129">string</span></span>  | <span data-ttu-id="7fff4-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7fff4-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7fff4-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7fff4-132">Request body</span></span>
<span data-ttu-id="7fff4-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7fff4-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7fff4-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="7fff4-134">Parameter</span></span>    | <span data-ttu-id="7fff4-135">Тип</span><span class="sxs-lookup"><span data-stu-id="7fff4-135">Type</span></span>   |<span data-ttu-id="7fff4-136">Описание</span><span class="sxs-lookup"><span data-stu-id="7fff4-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7fff4-137">comment</span><span class="sxs-lookup"><span data-stu-id="7fff4-137">comment</span></span>|<span data-ttu-id="7fff4-138">String</span><span class="sxs-lookup"><span data-stu-id="7fff4-138">String</span></span>|<span data-ttu-id="7fff4-p105">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="7fff4-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="7fff4-141">sendResponse</span><span class="sxs-lookup"><span data-stu-id="7fff4-141">sendResponse</span></span>|<span data-ttu-id="7fff4-142">Логическое</span><span class="sxs-lookup"><span data-stu-id="7fff4-142">Boolean</span></span>|<span data-ttu-id="7fff4-p106">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="7fff4-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|
|<span data-ttu-id="7fff4-146">пропоседневтиме</span><span class="sxs-lookup"><span data-stu-id="7fff4-146">proposedNewTime</span></span>|[<span data-ttu-id="7fff4-147">timeSlot</span><span class="sxs-lookup"><span data-stu-id="7fff4-147">timeSlot</span></span>](../resources/timeslot.md)|<span data-ttu-id="7fff4-148">Альтернативная дата/время, предлагаемые приглашению на собрание для начала и завершения.</span><span class="sxs-lookup"><span data-stu-id="7fff4-148">An alternate date/time proposed by an invitee for a meeting request to start and end.</span></span> <span data-ttu-id="7fff4-149">Действует только для событий, которые допускают новые предложения времени.</span><span class="sxs-lookup"><span data-stu-id="7fff4-149">Valid only for events that allow new time proposals.</span></span> <span data-ttu-id="7fff4-150">Для установки этого параметра необходимо \*\*\*\* задать для `true`параметра сендреспонсе значение.</span><span class="sxs-lookup"><span data-stu-id="7fff4-150">Setting this parameter requires setting **sendResponse** to `true`.</span></span> <span data-ttu-id="7fff4-151">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7fff4-151">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="7fff4-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fff4-152">Response</span></span>

<span data-ttu-id="7fff4-p108">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7fff4-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="7fff4-155">Это действие возвращает HTTP-400, если выполняется одно или оба следующих действия:</span><span class="sxs-lookup"><span data-stu-id="7fff4-155">This action returns HTTP 400 if one or both of the following occur:</span></span>

- <span data-ttu-id="7fff4-156">Параметр **пропоседневтиме** включен, но свойство **алловневтимепропосалс** **события** имеет `false`значение.</span><span class="sxs-lookup"><span data-stu-id="7fff4-156">The **proposedNewTime** parameter is included but the **allowNewTimeProposals** property of the **event** is `false`.</span></span> 
- <span data-ttu-id="7fff4-157">Параметр **пропоседневтиме** включен, но для `false`параметра **сендреспонсе** задано значение.</span><span class="sxs-lookup"><span data-stu-id="7fff4-157">The **proposedNewTime** parameter is included but the **sendResponse** parameter is set to `false`.</span></span>

## <a name="example"></a><span data-ttu-id="7fff4-158">Пример</span><span class="sxs-lookup"><span data-stu-id="7fff4-158">Example</span></span>
<span data-ttu-id="7fff4-159">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7fff4-159">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="7fff4-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fff4-160">Request</span></span>
<span data-ttu-id="7fff4-161">В следующем примере вошедшего в систему пользователя отвечает за заданное событие, задает для пареметер **сендреспонсе** значение true и включает альтернативное время в параметр **пропоседневтиме** .</span><span class="sxs-lookup"><span data-stu-id="7fff4-161">In the following example, the signed-in user responds tentative to the specified event, sets the **sendResponse** paremeter to true, and includes an alternative time in the **proposedNewTime** parameter.</span></span>

# <a name="http"></a>[<span data-ttu-id="7fff4-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fff4-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/tentativelyAccept
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
# <a name="c"></a>[<span data-ttu-id="7fff4-163">C#</span><span class="sxs-lookup"><span data-stu-id="7fff4-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-tentativelyaccept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7fff4-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fff4-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-tentativelyaccept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7fff4-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fff4-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-tentativelyaccept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="7fff4-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fff4-166">Response</span></span>
<span data-ttu-id="7fff4-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7fff4-167">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
