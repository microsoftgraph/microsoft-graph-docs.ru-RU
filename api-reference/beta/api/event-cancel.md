---
title: 'событие: Cancel (Отмена)'
description: 'Это действие позволяет организатору собрания отправить сообщение об отмене и отменить событие. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9ca4dc47472b444aea757deff10930f1242db075
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587154"
---
# <a name="event-cancel"></a><span data-ttu-id="2304d-103">событие: Cancel (Отмена)</span><span class="sxs-lookup"><span data-stu-id="2304d-103">event: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2304d-104">Это действие позволяет организатору собрания отправить сообщение об отмене и отменить событие.</span><span class="sxs-lookup"><span data-stu-id="2304d-104">This action allows the organizer of a meeting to send a cancellation message and cancel the event.</span></span> 

<span data-ttu-id="2304d-105">Действие перемещает событие в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="2304d-105">The action moves the event to the Deleted Items folder.</span></span> <span data-ttu-id="2304d-106">Организатор также может отменить вхождение повторяющегося собрания, указав идентификатор события.</span><span class="sxs-lookup"><span data-stu-id="2304d-106">The organizer can also cancel an occurrence of a recurring meeting by providing the occurrence event ID.</span></span> <span data-ttu-id="2304d-107">Участник, вызывающий это действие, получает ошибку (ошибочный запрос HTTP 400) со следующим сообщением об ошибке:</span><span class="sxs-lookup"><span data-stu-id="2304d-107">An attendee calling this action gets an error (HTTP 400 Bad Request), with the following error message:</span></span>

<span data-ttu-id="2304d-108">"Ваш запрос не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="2304d-108">"Your request can't be completed.</span></span> <span data-ttu-id="2304d-109">Для отмены собрания необходимо быть организатором. "</span><span class="sxs-lookup"><span data-stu-id="2304d-109">You need to be an organizer to cancel a meeting."</span></span>

<span data-ttu-id="2304d-110">Это действие отличается от [удаления](event-delete.md) в этой **отмене** , доступной только организатору, и позволяет Организатору отправлять настраиваемое сообщение участникам об отмене.</span><span class="sxs-lookup"><span data-stu-id="2304d-110">This action differs from [Delete](event-delete.md) in that **Cancel** is available to only the organizer, and lets the organizer send a custom message to the attendees about the cancellation.</span></span>

## <a name="permissions"></a><span data-ttu-id="2304d-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2304d-111">Permissions</span></span>
<span data-ttu-id="2304d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2304d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2304d-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2304d-114">Permission type</span></span>      | <span data-ttu-id="2304d-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2304d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2304d-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2304d-116">Delegated (work or school account)</span></span> | <span data-ttu-id="2304d-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2304d-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2304d-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2304d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2304d-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2304d-119">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2304d-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2304d-120">Application</span></span> | <span data-ttu-id="2304d-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2304d-121">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2304d-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2304d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/cancel
POST /users/{id | userPrincipalName}/events/{id}/cancel
POST /groups/{id}/events/{id}/cancel

POST /me/calendar/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendar/events/{id}/cancel
POST /groups/{id}/calendar/events/{id}/cancel

POST /me/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/cancel

POST /me/calendargroup/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/cancel

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/cancel
```
## <a name="request-headers"></a><span data-ttu-id="2304d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2304d-123">Request headers</span></span>
| <span data-ttu-id="2304d-124">Имя</span><span class="sxs-lookup"><span data-stu-id="2304d-124">Name</span></span>       | <span data-ttu-id="2304d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="2304d-125">Type</span></span> | <span data-ttu-id="2304d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="2304d-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2304d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="2304d-127">Authorization</span></span>  | <span data-ttu-id="2304d-128">string</span><span class="sxs-lookup"><span data-stu-id="2304d-128">string</span></span>  | <span data-ttu-id="2304d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2304d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2304d-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2304d-131">Content-Type</span></span> | <span data-ttu-id="2304d-132">string</span><span class="sxs-lookup"><span data-stu-id="2304d-132">string</span></span>  | <span data-ttu-id="2304d-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2304d-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2304d-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2304d-135">Request body</span></span>
<span data-ttu-id="2304d-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2304d-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2304d-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="2304d-137">Parameter</span></span>    | <span data-ttu-id="2304d-138">Тип</span><span class="sxs-lookup"><span data-stu-id="2304d-138">Type</span></span>   |<span data-ttu-id="2304d-139">Описание</span><span class="sxs-lookup"><span data-stu-id="2304d-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2304d-140">comment</span><span class="sxs-lookup"><span data-stu-id="2304d-140">comment</span></span>|<span data-ttu-id="2304d-141">String</span><span class="sxs-lookup"><span data-stu-id="2304d-141">String</span></span>|<span data-ttu-id="2304d-142">Комментарий об отмене, отправленном всем участникам.</span><span class="sxs-lookup"><span data-stu-id="2304d-142">A comment about the cancellation sent to all the attendees.</span></span> <span data-ttu-id="2304d-143">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="2304d-143">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="2304d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="2304d-144">Response</span></span>

<span data-ttu-id="2304d-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2304d-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2304d-147">Пример</span><span class="sxs-lookup"><span data-stu-id="2304d-147">Example</span></span>
<span data-ttu-id="2304d-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2304d-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2304d-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="2304d-149">Request</span></span>
<span data-ttu-id="2304d-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2304d-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_cancel"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/cancel
Content-type: application/json

{
  "Comment": "Cancelling for this week due to all hands"
}
```

##### <a name="response"></a><span data-ttu-id="2304d-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="2304d-151">Response</span></span>
<span data-ttu-id="2304d-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2304d-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2304d-153">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="2304d-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2304d-154">Языках</span><span class="sxs-lookup"><span data-stu-id="2304d-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/event_cancel-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2304d-155">Язык</span><span class="sxs-lookup"><span data-stu-id="2304d-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/event_cancel-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-cancel.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-cancel.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
