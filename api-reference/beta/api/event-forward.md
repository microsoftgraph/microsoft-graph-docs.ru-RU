---
title: 'события: вперед'
description: 'Это действие позволяет Организатор или участник собрания события для пересылки '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6f1b3e1f089d927aeb21ca80ff77edda63121c60
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510388"
---
# <a name="event-forward"></a><span data-ttu-id="b28ce-103">события: вперед</span><span class="sxs-lookup"><span data-stu-id="b28ce-103">event: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b28ce-104">Это действие позволяет Организатор или участник собрания [события](../resources/event.md) пересылать запрос на собрание на нового получателя.</span><span class="sxs-lookup"><span data-stu-id="b28ce-104">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="b28ce-105">Если событие собрания пересылается из почтового ящика Office 365 участника другому получателю, это действие также отправляет сообщение для уведомления Организатор переадресации и добавляет получателя копии организатора собрания события.</span><span class="sxs-lookup"><span data-stu-id="b28ce-105">If the meeting event is forwarded from an attendee's Office 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="b28ce-106">В этом удобства недоступна при пересылке из учетной записи Outlook.com.</span><span class="sxs-lookup"><span data-stu-id="b28ce-106">This convenience is not available when forwarding from an Outlook.com account.</span></span>


## <a name="permissions"></a><span data-ttu-id="b28ce-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b28ce-107">Permissions</span></span>
<span data-ttu-id="b28ce-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b28ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b28ce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b28ce-110">Permission type</span></span>      | <span data-ttu-id="b28ce-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b28ce-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b28ce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b28ce-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b28ce-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b28ce-113">Calendars.Read</span></span>    |
|<span data-ttu-id="b28ce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b28ce-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b28ce-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b28ce-115">Calendars.Read</span></span>    |
|<span data-ttu-id="b28ce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b28ce-116">Application</span></span> | <span data-ttu-id="b28ce-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b28ce-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="b28ce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b28ce-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="b28ce-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b28ce-119">Request headers</span></span>
| <span data-ttu-id="b28ce-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b28ce-120">Name</span></span>       | <span data-ttu-id="b28ce-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b28ce-121">Type</span></span> | <span data-ttu-id="b28ce-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b28ce-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b28ce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b28ce-123">Authorization</span></span>  | <span data-ttu-id="b28ce-124">string</span><span class="sxs-lookup"><span data-stu-id="b28ce-124">string</span></span>  | <span data-ttu-id="b28ce-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b28ce-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b28ce-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b28ce-127">Content-Type</span></span> | <span data-ttu-id="b28ce-128">string</span><span class="sxs-lookup"><span data-stu-id="b28ce-128">string</span></span>  | <span data-ttu-id="b28ce-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b28ce-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b28ce-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b28ce-131">Request body</span></span>
<span data-ttu-id="b28ce-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b28ce-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b28ce-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="b28ce-133">Parameter</span></span>    | <span data-ttu-id="b28ce-134">Тип</span><span class="sxs-lookup"><span data-stu-id="b28ce-134">Type</span></span>   |<span data-ttu-id="b28ce-135">Описание</span><span class="sxs-lookup"><span data-stu-id="b28ce-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b28ce-136">Comment</span><span class="sxs-lookup"><span data-stu-id="b28ce-136">Comment</span></span>|<span data-ttu-id="b28ce-137">String</span><span class="sxs-lookup"><span data-stu-id="b28ce-137">String</span></span>|<span data-ttu-id="b28ce-p105">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="b28ce-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="b28ce-140">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="b28ce-140">ToRecipients</span></span>|<span data-ttu-id="b28ce-141">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="b28ce-141">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="b28ce-142">Список получателей пересылать события.</span><span class="sxs-lookup"><span data-stu-id="b28ce-142">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="b28ce-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b28ce-143">Response</span></span>

<span data-ttu-id="b28ce-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b28ce-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b28ce-146">Пример</span><span class="sxs-lookup"><span data-stu-id="b28ce-146">Example</span></span>
<span data-ttu-id="b28ce-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b28ce-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b28ce-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="b28ce-148">Request</span></span>
<span data-ttu-id="b28ce-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b28ce-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b28ce-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="b28ce-150">Response</span></span>
<span data-ttu-id="b28ce-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b28ce-151">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/event-forward.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
