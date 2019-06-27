---
title: 'событие: Forwarded'
description: 'Это действие позволяет Организатору или участнику события "собрание" пересылать '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5da653eab0dd1d3ab97a3df8bf0de0ffd110c0e3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259159"
---
# <a name="event-forward"></a><span data-ttu-id="ea820-103">событие: Forwarded</span><span class="sxs-lookup"><span data-stu-id="ea820-103">event: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea820-104">Это действие позволяет Организатору или участнику [события](../resources/event.md) "собрание" пересылать приглашение на собрание новому получателю.</span><span class="sxs-lookup"><span data-stu-id="ea820-104">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="ea820-105">Если событие "собрание" переадресовано из почтового ящика Office 365 другому получателю, это действие также отправляет сообщение организатору переадресации и добавляет получателя к копии события собрания организатора.</span><span class="sxs-lookup"><span data-stu-id="ea820-105">If the meeting event is forwarded from an attendee's Office 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="ea820-106">Это удобство недоступно при пересылке с учетной записи Outlook.com.</span><span class="sxs-lookup"><span data-stu-id="ea820-106">This convenience is not available when forwarding from an Outlook.com account.</span></span>


## <a name="permissions"></a><span data-ttu-id="ea820-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea820-107">Permissions</span></span>
<span data-ttu-id="ea820-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea820-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea820-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea820-110">Permission type</span></span>      | <span data-ttu-id="ea820-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea820-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea820-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea820-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ea820-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ea820-113">Calendars.Read</span></span>    |
|<span data-ttu-id="ea820-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea820-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea820-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ea820-115">Calendars.Read</span></span>    |
|<span data-ttu-id="ea820-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea820-116">Application</span></span> | <span data-ttu-id="ea820-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ea820-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea820-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea820-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/forward
POST /users/{id | userPrincipalName}/events/{id}/forward
POST /groups/{id}/events/{id}/forward

POST /me/calendar/events/{id}/forward
POST /users/{id | userPrincipalName}/calendar/events/{id}/forward
POST /groups/{id}/calendar/events/{id}/forward

POST /me/calendars/{id}/events/{id}/forward
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/forward

POST /me/calendargroup/calendars/{id}/events/{id}/forward
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/forward

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/forward
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="ea820-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea820-119">Request headers</span></span>
| <span data-ttu-id="ea820-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ea820-120">Name</span></span>       | <span data-ttu-id="ea820-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ea820-121">Type</span></span> | <span data-ttu-id="ea820-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ea820-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ea820-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea820-123">Authorization</span></span>  | <span data-ttu-id="ea820-124">string</span><span class="sxs-lookup"><span data-stu-id="ea820-124">string</span></span>  | <span data-ttu-id="ea820-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea820-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ea820-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ea820-127">Content-Type</span></span> | <span data-ttu-id="ea820-128">string</span><span class="sxs-lookup"><span data-stu-id="ea820-128">string</span></span>  | <span data-ttu-id="ea820-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea820-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea820-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea820-131">Request body</span></span>
<span data-ttu-id="ea820-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ea820-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ea820-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="ea820-133">Parameter</span></span>    | <span data-ttu-id="ea820-134">Тип</span><span class="sxs-lookup"><span data-stu-id="ea820-134">Type</span></span>   |<span data-ttu-id="ea820-135">Описание</span><span class="sxs-lookup"><span data-stu-id="ea820-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea820-136">Комментарий</span><span class="sxs-lookup"><span data-stu-id="ea820-136">Comment</span></span>|<span data-ttu-id="ea820-137">String</span><span class="sxs-lookup"><span data-stu-id="ea820-137">String</span></span>|<span data-ttu-id="ea820-p105">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="ea820-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="ea820-140">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="ea820-140">ToRecipients</span></span>|<span data-ttu-id="ea820-141">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="ea820-141">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="ea820-142">Список получателей, на которые пересылается событие.</span><span class="sxs-lookup"><span data-stu-id="ea820-142">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="ea820-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea820-143">Response</span></span>

<span data-ttu-id="ea820-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ea820-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea820-146">Пример</span><span class="sxs-lookup"><span data-stu-id="ea820-146">Example</span></span>
<span data-ttu-id="ea820-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ea820-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ea820-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea820-148">Request</span></span>
<span data-ttu-id="ea820-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea820-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_forward"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/forward
Content-type: application/json
Content-length: 56

{
  "ToRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ],
  "Comment": "Dana, hope you can make this meeting." 
}

```

##### <a name="response"></a><span data-ttu-id="ea820-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea820-150">Response</span></span>
<span data-ttu-id="ea820-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ea820-151">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ea820-152">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="ea820-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ea820-153">C#</span><span class="sxs-lookup"><span data-stu-id="ea820-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/event_forward-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ea820-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="ea820-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/event_forward-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ea820-155">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ea820-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/event_forward-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-forward.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/event-forward.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-forward.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
