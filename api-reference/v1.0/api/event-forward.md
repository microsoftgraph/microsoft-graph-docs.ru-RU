---
title: 'event: forward'
description: 'Это действие позволяет организатору или участнику собрания перенаад '
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 624312256cbca37529eb55eececa136df04d69fe
ms.sourcegitcommit: 0cde389d4d6dbec1568dab14490f0fd6297d5aa4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720753"
---
# <a name="event-forward"></a><span data-ttu-id="302d2-103">event: forward</span><span class="sxs-lookup"><span data-stu-id="302d2-103">event: forward</span></span>

<span data-ttu-id="302d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="302d2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="302d2-105">Это действие позволяет организатору или [](../resources/event.md) участнику собрания перенаададовыть запрос на собрание новому получателю.</span><span class="sxs-lookup"><span data-stu-id="302d2-105">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="302d2-106">Если событие собрания перенаправляется из почтового ящика участника Microsoft 365 другому получателю, это действие также отправляет сообщение для уведомления организатора о переадстройке и добавляет получателя в копию организатора события собрания.</span><span class="sxs-lookup"><span data-stu-id="302d2-106">If the meeting event is forwarded from an attendee's Microsoft 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="302d2-107">Это удобство недоступно при переадад записи Outlook.com учетной записи.</span><span class="sxs-lookup"><span data-stu-id="302d2-107">This convenience is not available when forwarding from an Outlook.com account.</span></span>

## <a name="permissions"></a><span data-ttu-id="302d2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="302d2-108">Permissions</span></span>
<span data-ttu-id="302d2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="302d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="302d2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="302d2-111">Permission type</span></span>      | <span data-ttu-id="302d2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="302d2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="302d2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="302d2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="302d2-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="302d2-114">Calendars.Read</span></span>    |
|<span data-ttu-id="302d2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="302d2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="302d2-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="302d2-116">Calendars.Read</span></span>    |
|<span data-ttu-id="302d2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="302d2-117">Application</span></span> | <span data-ttu-id="302d2-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="302d2-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="302d2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="302d2-119">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="302d2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="302d2-120">Request headers</span></span>
| <span data-ttu-id="302d2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="302d2-121">Name</span></span>       | <span data-ttu-id="302d2-122">Тип</span><span class="sxs-lookup"><span data-stu-id="302d2-122">Type</span></span> | <span data-ttu-id="302d2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="302d2-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="302d2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="302d2-124">Authorization</span></span>  | <span data-ttu-id="302d2-125">string</span><span class="sxs-lookup"><span data-stu-id="302d2-125">string</span></span>  | <span data-ttu-id="302d2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="302d2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="302d2-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="302d2-128">Content-Type</span></span> | <span data-ttu-id="302d2-129">string</span><span class="sxs-lookup"><span data-stu-id="302d2-129">string</span></span>  | <span data-ttu-id="302d2-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="302d2-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="302d2-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="302d2-132">Request body</span></span>
<span data-ttu-id="302d2-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="302d2-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="302d2-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="302d2-134">Parameter</span></span>    | <span data-ttu-id="302d2-135">Тип</span><span class="sxs-lookup"><span data-stu-id="302d2-135">Type</span></span>   |<span data-ttu-id="302d2-136">Описание</span><span class="sxs-lookup"><span data-stu-id="302d2-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="302d2-137">Comment</span><span class="sxs-lookup"><span data-stu-id="302d2-137">Comment</span></span>|<span data-ttu-id="302d2-138">String</span><span class="sxs-lookup"><span data-stu-id="302d2-138">String</span></span>|<span data-ttu-id="302d2-p105">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="302d2-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="302d2-141">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="302d2-141">ToRecipients</span></span>|<span data-ttu-id="302d2-142">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="302d2-142">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="302d2-143">Список получателей, на которые необходимо перенаадентить событие.</span><span class="sxs-lookup"><span data-stu-id="302d2-143">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="302d2-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="302d2-144">Response</span></span>

<span data-ttu-id="302d2-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="302d2-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="302d2-147">Пример</span><span class="sxs-lookup"><span data-stu-id="302d2-147">Example</span></span>
<span data-ttu-id="302d2-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="302d2-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="302d2-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="302d2-149">Request</span></span>
<span data-ttu-id="302d2-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="302d2-150">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/forward
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


##### <a name="response"></a><span data-ttu-id="302d2-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="302d2-151">Response</span></span>
<span data-ttu-id="302d2-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="302d2-152">Here is an example of the response.</span></span>
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
