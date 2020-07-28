---
title: 'event: tentativelyAccept'
description: Принятие под вопросом указанного события в календаре пользователя.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 183742e6f6402b6ba00a749f80ae934a421ea1a4
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427111"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="5b0b7-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="5b0b7-103">event: tentativelyAccept</span></span>

<span data-ttu-id="5b0b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b0b7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5b0b7-105">Предварительно принять указанное [событие](../resources/event.md) в [календаре](../resources/calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="5b0b7-105">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

<span data-ttu-id="5b0b7-106">Если событие позволяет создавать предложения для нового времени, при отклике на запрос о событии приглашение можно предложить альтернативное время, включив параметр **пропоседневтиме** .</span><span class="sxs-lookup"><span data-stu-id="5b0b7-106">If the event allows proposals for new times, on responding tentative to the event, an invitee can choose to suggest an alternative time by including the **proposedNewTime** parameter.</span></span> <span data-ttu-id="5b0b7-107">Дополнительные сведения о том, как предлагать время, а также как получать и принимать новое предложение по времени, приведены в разделе [предложение нового времени проведения собрания](/graph/outlook-calendar-meeting-proposals).</span><span class="sxs-lookup"><span data-stu-id="5b0b7-107">For more information on how to propose a time, and how to receive and accept a new time proposal, see [Propose new meeting times](/graph/outlook-calendar-meeting-proposals).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b0b7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b0b7-108">Permissions</span></span>
<span data-ttu-id="5b0b7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b0b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b0b7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b0b7-111">Permission type</span></span>      | <span data-ttu-id="5b0b7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b0b7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b0b7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b0b7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5b0b7-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b0b7-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5b0b7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b0b7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b0b7-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b0b7-116">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5b0b7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b0b7-117">Application</span></span> | <span data-ttu-id="5b0b7-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b0b7-118">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b0b7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b0b7-119">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="5b0b7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b0b7-120">Request headers</span></span>
| <span data-ttu-id="5b0b7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5b0b7-121">Name</span></span>       | <span data-ttu-id="5b0b7-122">Тип</span><span class="sxs-lookup"><span data-stu-id="5b0b7-122">Type</span></span> | <span data-ttu-id="5b0b7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5b0b7-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5b0b7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b0b7-124">Authorization</span></span>  | <span data-ttu-id="5b0b7-125">string</span><span class="sxs-lookup"><span data-stu-id="5b0b7-125">string</span></span>  | <span data-ttu-id="5b0b7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b0b7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5b0b7-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b0b7-128">Content-Type</span></span> | <span data-ttu-id="5b0b7-129">string</span><span class="sxs-lookup"><span data-stu-id="5b0b7-129">string</span></span>  | <span data-ttu-id="5b0b7-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b0b7-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b0b7-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b0b7-132">Request body</span></span>
<span data-ttu-id="5b0b7-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5b0b7-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5b0b7-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="5b0b7-134">Parameter</span></span>    | <span data-ttu-id="5b0b7-135">Тип</span><span class="sxs-lookup"><span data-stu-id="5b0b7-135">Type</span></span>   |<span data-ttu-id="5b0b7-136">Описание</span><span class="sxs-lookup"><span data-stu-id="5b0b7-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b0b7-137">comment</span><span class="sxs-lookup"><span data-stu-id="5b0b7-137">comment</span></span>|<span data-ttu-id="5b0b7-138">String</span><span class="sxs-lookup"><span data-stu-id="5b0b7-138">String</span></span>|<span data-ttu-id="5b0b7-p105">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="5b0b7-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="5b0b7-141">пропоседневтиме</span><span class="sxs-lookup"><span data-stu-id="5b0b7-141">proposedNewTime</span></span>|[<span data-ttu-id="5b0b7-142">timeSlot</span><span class="sxs-lookup"><span data-stu-id="5b0b7-142">timeSlot</span></span>](../resources/timeslot.md)|<span data-ttu-id="5b0b7-143">Альтернативная дата/время, предлагаемые приглашению на собрание для начала и завершения.</span><span class="sxs-lookup"><span data-stu-id="5b0b7-143">An alternate date/time proposed by an invitee for a meeting request to start and end.</span></span> <span data-ttu-id="5b0b7-144">Действует только для событий, которые допускают новые предложения времени.</span><span class="sxs-lookup"><span data-stu-id="5b0b7-144">Valid only for events that allow new time proposals.</span></span> <span data-ttu-id="5b0b7-145">Для установки этого параметра необходимо задать для параметра **сендреспонсе** значение `true` .</span><span class="sxs-lookup"><span data-stu-id="5b0b7-145">Setting this parameter requires setting **sendResponse** to `true`.</span></span> <span data-ttu-id="5b0b7-146">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="5b0b7-146">Optional.</span></span>|
|<span data-ttu-id="5b0b7-147">sendResponse</span><span class="sxs-lookup"><span data-stu-id="5b0b7-147">sendResponse</span></span>|<span data-ttu-id="5b0b7-148">Логическое</span><span class="sxs-lookup"><span data-stu-id="5b0b7-148">Boolean</span></span>|<span data-ttu-id="5b0b7-p107">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="5b0b7-p107">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="5b0b7-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b0b7-152">Response</span></span>

<span data-ttu-id="5b0b7-p108">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5b0b7-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="5b0b7-155">Это действие возвращает HTTP-400, если выполняется одно или оба следующих действия:</span><span class="sxs-lookup"><span data-stu-id="5b0b7-155">This action returns HTTP 400 if one or both of the following occur:</span></span>

- <span data-ttu-id="5b0b7-156">Параметр **пропоседневтиме** включен, но свойство **алловневтимепропосалс** **события** имеет значение `false` .</span><span class="sxs-lookup"><span data-stu-id="5b0b7-156">The **proposedNewTime** parameter is included but the **allowNewTimeProposals** property of the **event** is `false`.</span></span> 
- <span data-ttu-id="5b0b7-157">Параметр **пропоседневтиме** включен, но для параметра **сендреспонсе** задано значение `false` .</span><span class="sxs-lookup"><span data-stu-id="5b0b7-157">The **proposedNewTime** parameter is included but the **sendResponse** parameter is set to `false`.</span></span>

## <a name="example"></a><span data-ttu-id="5b0b7-158">Пример</span><span class="sxs-lookup"><span data-stu-id="5b0b7-158">Example</span></span>
<span data-ttu-id="5b0b7-159">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5b0b7-159">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="5b0b7-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b0b7-160">Request</span></span>
<span data-ttu-id="5b0b7-161">В следующем примере вошедшего в систему пользователя отвечает за заданное событие, задает для пареметер **сендреспонсе** значение true и включает альтернативное время в параметр **пропоседневтиме** .</span><span class="sxs-lookup"><span data-stu-id="5b0b7-161">In the following example, the signed-in user responds tentative to the specified event, sets the **sendResponse** paremeter to true, and includes an alternative time in the **proposedNewTime** parameter.</span></span>

# <a name="http"></a>[<span data-ttu-id="5b0b7-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b0b7-162">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5b0b7-163">C#</span><span class="sxs-lookup"><span data-stu-id="5b0b7-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-tentativelyaccept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b0b7-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b0b7-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-tentativelyaccept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b0b7-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b0b7-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-tentativelyaccept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5b0b7-166">Java</span><span class="sxs-lookup"><span data-stu-id="5b0b7-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-tentativelyaccept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5b0b7-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b0b7-167">Response</span></span>
<span data-ttu-id="5b0b7-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5b0b7-168">Here is an example of the response.</span></span>
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
