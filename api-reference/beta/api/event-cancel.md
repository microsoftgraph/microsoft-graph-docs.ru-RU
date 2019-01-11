---
title: 'событие: Отмена'
description: 'Это действие позволяет организатора собрания отправить сообщение об отмене и отмены события. '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 482804d58078f148ed321a0c3489954fc9144f8e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864626"
---
# <a name="event-cancel"></a><span data-ttu-id="b168d-103">событие: Отмена</span><span class="sxs-lookup"><span data-stu-id="b168d-103">event: cancel</span></span>

> <span data-ttu-id="b168d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b168d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b168d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b168d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b168d-106">Это действие позволяет организатора собрания отправить сообщение об отмене и отмены события.</span><span class="sxs-lookup"><span data-stu-id="b168d-106">This action allows the organizer of a meeting to send a cancellation message and cancel the event.</span></span> 

<span data-ttu-id="b168d-107">Действие перемещает события папки "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="b168d-107">The action moves the event to the Deleted Items folder.</span></span> <span data-ttu-id="b168d-108">Организатор также можно отменить вхождения повторяющееся собрание с указанием событий с идентификатором вхождение.</span><span class="sxs-lookup"><span data-stu-id="b168d-108">The organizer can also cancel an occurrence of a recurring meeting by providing the occurrence event ID.</span></span> <span data-ttu-id="b168d-109">Участником вызов это действие получает сообщение об ошибке (HTTP 400 Bad Request), с следующее сообщение об ошибке:</span><span class="sxs-lookup"><span data-stu-id="b168d-109">An attendee calling this action gets an error (HTTP 400 Bad Request), with the following error message:</span></span>

<span data-ttu-id="b168d-110">«Не удается выполнить запрос.</span><span class="sxs-lookup"><span data-stu-id="b168d-110">"Your request can't be completed.</span></span> <span data-ttu-id="b168d-111">Вы должны быть Организатор может отменить собрание.»</span><span class="sxs-lookup"><span data-stu-id="b168d-111">You need to be an organizer to cancel a meeting."</span></span>

<span data-ttu-id="b168d-112">Это действие отличается от [удаления](event-delete.md) , **Отменить** доступна только организатора, а также позволяет отправить сообщение участникам об отмене организатора.</span><span class="sxs-lookup"><span data-stu-id="b168d-112">This action differs from [Delete](event-delete.md) in that **Cancel** is available to only the organizer, and lets the organizer send a custom message to the attendees about the cancellation.</span></span>

## <a name="permissions"></a><span data-ttu-id="b168d-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b168d-113">Permissions</span></span>
<span data-ttu-id="b168d-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b168d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b168d-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b168d-116">Permission type</span></span>      | <span data-ttu-id="b168d-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b168d-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b168d-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b168d-118">Delegated (work or school account)</span></span> | <span data-ttu-id="b168d-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b168d-119">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b168d-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b168d-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b168d-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b168d-121">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b168d-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b168d-122">Application</span></span> | <span data-ttu-id="b168d-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b168d-123">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b168d-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b168d-124">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="b168d-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b168d-125">Request headers</span></span>
| <span data-ttu-id="b168d-126">Имя</span><span class="sxs-lookup"><span data-stu-id="b168d-126">Name</span></span>       | <span data-ttu-id="b168d-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b168d-127">Type</span></span> | <span data-ttu-id="b168d-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b168d-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b168d-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="b168d-129">Authorization</span></span>  | <span data-ttu-id="b168d-130">string</span><span class="sxs-lookup"><span data-stu-id="b168d-130">string</span></span>  | <span data-ttu-id="b168d-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b168d-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b168d-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b168d-133">Content-Type</span></span> | <span data-ttu-id="b168d-134">string</span><span class="sxs-lookup"><span data-stu-id="b168d-134">string</span></span>  | <span data-ttu-id="b168d-p106">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b168d-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b168d-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b168d-137">Request body</span></span>
<span data-ttu-id="b168d-138">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b168d-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b168d-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="b168d-139">Parameter</span></span>    | <span data-ttu-id="b168d-140">Тип</span><span class="sxs-lookup"><span data-stu-id="b168d-140">Type</span></span>   |<span data-ttu-id="b168d-141">Описание</span><span class="sxs-lookup"><span data-stu-id="b168d-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b168d-142">comment</span><span class="sxs-lookup"><span data-stu-id="b168d-142">comment</span></span>|<span data-ttu-id="b168d-143">Строка</span><span class="sxs-lookup"><span data-stu-id="b168d-143">String</span></span>|<span data-ttu-id="b168d-144">Примечание об отмене, отправленных всем участникам.</span><span class="sxs-lookup"><span data-stu-id="b168d-144">A comment about the cancellation sent to all the attendees.</span></span> <span data-ttu-id="b168d-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="b168d-145">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="b168d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b168d-146">Response</span></span>

<span data-ttu-id="b168d-p108">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b168d-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b168d-149">Пример</span><span class="sxs-lookup"><span data-stu-id="b168d-149">Example</span></span>
<span data-ttu-id="b168d-150">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b168d-150">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b168d-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="b168d-151">Request</span></span>
<span data-ttu-id="b168d-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b168d-152">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b168d-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="b168d-153">Response</span></span>
<span data-ttu-id="b168d-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b168d-154">Here is an example of the response.</span></span>
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
  "description": "event: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
