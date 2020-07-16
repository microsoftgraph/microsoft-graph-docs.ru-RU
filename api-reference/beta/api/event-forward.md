---
title: 'событие: Forwarded'
description: 'Это действие позволяет Организатору или участнику события "собрание" пересылать '
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 03045c2b7fb438e1affa574e1db8682336ac43c3
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895736"
---
# <a name="event-forward"></a><span data-ttu-id="14ae2-103">событие: Forwarded</span><span class="sxs-lookup"><span data-stu-id="14ae2-103">event: forward</span></span>

<span data-ttu-id="14ae2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14ae2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14ae2-105">Это действие позволяет Организатору или участнику [события](../resources/event.md) "собрание" пересылать приглашение на собрание новому получателю.</span><span class="sxs-lookup"><span data-stu-id="14ae2-105">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="14ae2-106">Если событие "собрание" переадресовано от почтового ящика Microsoft 365 другому получателю, это действие также отправляет сообщение организатору переадресации и добавляет получателя к копии события собрания организатора.</span><span class="sxs-lookup"><span data-stu-id="14ae2-106">If the meeting event is forwarded from an attendee's Microsoft 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="14ae2-107">Это удобство недоступно при пересылке с учетной записи Outlook.com.</span><span class="sxs-lookup"><span data-stu-id="14ae2-107">This convenience is not available when forwarding from an Outlook.com account.</span></span>


## <a name="permissions"></a><span data-ttu-id="14ae2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14ae2-108">Permissions</span></span>
<span data-ttu-id="14ae2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14ae2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14ae2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14ae2-111">Permission type</span></span>      | <span data-ttu-id="14ae2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14ae2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14ae2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14ae2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="14ae2-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="14ae2-114">Calendars.Read</span></span>    |
|<span data-ttu-id="14ae2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14ae2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14ae2-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="14ae2-116">Calendars.Read</span></span>    |
|<span data-ttu-id="14ae2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14ae2-117">Application</span></span> | <span data-ttu-id="14ae2-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="14ae2-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="14ae2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14ae2-119">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="14ae2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14ae2-120">Request headers</span></span>
| <span data-ttu-id="14ae2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="14ae2-121">Name</span></span>       | <span data-ttu-id="14ae2-122">Тип</span><span class="sxs-lookup"><span data-stu-id="14ae2-122">Type</span></span> | <span data-ttu-id="14ae2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="14ae2-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="14ae2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="14ae2-124">Authorization</span></span>  | <span data-ttu-id="14ae2-125">string</span><span class="sxs-lookup"><span data-stu-id="14ae2-125">string</span></span>  | <span data-ttu-id="14ae2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14ae2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="14ae2-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="14ae2-128">Content-Type</span></span> | <span data-ttu-id="14ae2-129">string</span><span class="sxs-lookup"><span data-stu-id="14ae2-129">string</span></span>  | <span data-ttu-id="14ae2-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14ae2-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14ae2-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14ae2-132">Request body</span></span>
<span data-ttu-id="14ae2-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="14ae2-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="14ae2-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="14ae2-134">Parameter</span></span>    | <span data-ttu-id="14ae2-135">Тип</span><span class="sxs-lookup"><span data-stu-id="14ae2-135">Type</span></span>   |<span data-ttu-id="14ae2-136">Описание</span><span class="sxs-lookup"><span data-stu-id="14ae2-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14ae2-137">Comment</span><span class="sxs-lookup"><span data-stu-id="14ae2-137">Comment</span></span>|<span data-ttu-id="14ae2-138">String</span><span class="sxs-lookup"><span data-stu-id="14ae2-138">String</span></span>|<span data-ttu-id="14ae2-p105">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="14ae2-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="14ae2-141">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="14ae2-141">ToRecipients</span></span>|<span data-ttu-id="14ae2-142">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="14ae2-142">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="14ae2-143">Список получателей, на которые пересылается событие.</span><span class="sxs-lookup"><span data-stu-id="14ae2-143">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="14ae2-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="14ae2-144">Response</span></span>

<span data-ttu-id="14ae2-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="14ae2-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14ae2-147">Пример</span><span class="sxs-lookup"><span data-stu-id="14ae2-147">Example</span></span>
<span data-ttu-id="14ae2-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="14ae2-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="14ae2-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="14ae2-149">Request</span></span>
<span data-ttu-id="14ae2-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14ae2-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="14ae2-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="14ae2-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="14ae2-152">C#</span><span class="sxs-lookup"><span data-stu-id="14ae2-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14ae2-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14ae2-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14ae2-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14ae2-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="14ae2-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="14ae2-155">Response</span></span>
<span data-ttu-id="14ae2-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="14ae2-156">Here is an example of the response.</span></span>
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
  "description": "event: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
