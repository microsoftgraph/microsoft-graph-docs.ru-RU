---
title: 'события: вперед'
description: 'Это действие позволяет Организатор или участник собрания события для пересылки '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 6567c8c030fa838e83a7428399151b41e6747625
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887831"
---
# <a name="event-forward"></a><span data-ttu-id="4c69c-103">события: вперед</span><span class="sxs-lookup"><span data-stu-id="4c69c-103">event: forward</span></span>

> <span data-ttu-id="4c69c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4c69c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c69c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c69c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4c69c-106">Это действие позволяет Организатор или участник собрания [события](../resources/event.md) пересылать запрос на собрание на нового получателя.</span><span class="sxs-lookup"><span data-stu-id="4c69c-106">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="4c69c-107">Если событие собрания пересылается из почтового ящика Office 365 участника другому получателю, это действие также отправляет сообщение для уведомления Организатор переадресации и добавляет получателя копии организатора собрания события.</span><span class="sxs-lookup"><span data-stu-id="4c69c-107">If the meeting event is forwarded from an attendee's Office 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="4c69c-108">В этом удобства недоступна при пересылке из учетной записи Outlook.com.</span><span class="sxs-lookup"><span data-stu-id="4c69c-108">This convenience is not available when forwarding from an Outlook.com account.</span></span>


## <a name="permissions"></a><span data-ttu-id="4c69c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c69c-109">Permissions</span></span>
<span data-ttu-id="4c69c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c69c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c69c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c69c-112">Permission type</span></span>      | <span data-ttu-id="4c69c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c69c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c69c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c69c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4c69c-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4c69c-115">Calendars.Read</span></span>    |
|<span data-ttu-id="4c69c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c69c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c69c-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4c69c-117">Calendars.Read</span></span>    |
|<span data-ttu-id="4c69c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c69c-118">Application</span></span> | <span data-ttu-id="4c69c-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4c69c-119">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c69c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c69c-120">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="4c69c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c69c-121">Request headers</span></span>
| <span data-ttu-id="4c69c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4c69c-122">Name</span></span>       | <span data-ttu-id="4c69c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="4c69c-123">Type</span></span> | <span data-ttu-id="4c69c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4c69c-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4c69c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c69c-125">Authorization</span></span>  | <span data-ttu-id="4c69c-126">string</span><span class="sxs-lookup"><span data-stu-id="4c69c-126">string</span></span>  | <span data-ttu-id="4c69c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c69c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4c69c-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c69c-129">Content-Type</span></span> | <span data-ttu-id="4c69c-130">string</span><span class="sxs-lookup"><span data-stu-id="4c69c-130">string</span></span>  | <span data-ttu-id="4c69c-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c69c-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c69c-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c69c-133">Request body</span></span>
<span data-ttu-id="4c69c-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4c69c-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4c69c-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="4c69c-135">Parameter</span></span>    | <span data-ttu-id="4c69c-136">Тип</span><span class="sxs-lookup"><span data-stu-id="4c69c-136">Type</span></span>   |<span data-ttu-id="4c69c-137">Описание</span><span class="sxs-lookup"><span data-stu-id="4c69c-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c69c-138">Comment</span><span class="sxs-lookup"><span data-stu-id="4c69c-138">Comment</span></span>|<span data-ttu-id="4c69c-139">String</span><span class="sxs-lookup"><span data-stu-id="4c69c-139">String</span></span>|<span data-ttu-id="4c69c-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="4c69c-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="4c69c-142">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="4c69c-142">ToRecipients</span></span>|<span data-ttu-id="4c69c-143">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="4c69c-143">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="4c69c-144">Список получателей пересылать события.</span><span class="sxs-lookup"><span data-stu-id="4c69c-144">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="4c69c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c69c-145">Response</span></span>

<span data-ttu-id="4c69c-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4c69c-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c69c-148">Пример</span><span class="sxs-lookup"><span data-stu-id="4c69c-148">Example</span></span>
<span data-ttu-id="4c69c-149">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4c69c-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4c69c-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c69c-150">Request</span></span>
<span data-ttu-id="4c69c-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c69c-151">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="4c69c-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c69c-152">Response</span></span>
<span data-ttu-id="4c69c-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c69c-153">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
