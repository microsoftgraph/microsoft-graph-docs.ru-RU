---
title: 'event: cancel'
description: 'Это действие позволяет организатору собрания отправить сообщение об отмене и отменить событие. '
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 549d5f4e30f288b82d5637da50241c895373f8fe
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754261"
---
# <a name="event-cancel"></a><span data-ttu-id="f151a-103">event: cancel</span><span class="sxs-lookup"><span data-stu-id="f151a-103">event: cancel</span></span>

<span data-ttu-id="f151a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f151a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f151a-105">Это действие позволяет организатору собрания отправить сообщение об отмене и отменить событие.</span><span class="sxs-lookup"><span data-stu-id="f151a-105">This action allows the organizer of a meeting to send a cancellation message and cancel the event.</span></span> 

<span data-ttu-id="f151a-106">Действие перемещает событие в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="f151a-106">The action moves the event to the Deleted Items folder.</span></span> <span data-ttu-id="f151a-107">Организатор также может отменить повторяющиеся собрания, предоставив ид события повторения.</span><span class="sxs-lookup"><span data-stu-id="f151a-107">The organizer can also cancel an occurrence of a recurring meeting by providing the occurrence event ID.</span></span> <span data-ttu-id="f151a-108">Участник, который вызывает это действие, получает ошибку (HTTP 400 Bad Request) со следующим сообщением об ошибке:</span><span class="sxs-lookup"><span data-stu-id="f151a-108">An attendee calling this action gets an error (HTTP 400 Bad Request), with the following error message:</span></span>

<span data-ttu-id="f151a-109">"Ваш запрос не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="f151a-109">"Your request can't be completed.</span></span> <span data-ttu-id="f151a-110">Для отмены собрания необходимо быть организатором".</span><span class="sxs-lookup"><span data-stu-id="f151a-110">You need to be an organizer to cancel a meeting."</span></span>

<span data-ttu-id="f151a-111">Это действие отличается от  [удаления](event-delete.md) тем, что "Отмена" доступна только организатору, и позволяет организатору отправлять участникам настраиваемые сообщения об отмене.</span><span class="sxs-lookup"><span data-stu-id="f151a-111">This action differs from [Delete](event-delete.md) in that **Cancel** is available to only the organizer, and lets the organizer send a custom message to the attendees about the cancellation.</span></span>

## <a name="permissions"></a><span data-ttu-id="f151a-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f151a-112">Permissions</span></span>
<span data-ttu-id="f151a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f151a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f151a-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f151a-115">Permission type</span></span>      | <span data-ttu-id="f151a-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f151a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f151a-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f151a-117">Delegated (work or school account)</span></span> | <span data-ttu-id="f151a-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f151a-118">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f151a-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f151a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f151a-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f151a-120">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f151a-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f151a-121">Application</span></span> | <span data-ttu-id="f151a-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f151a-122">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f151a-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f151a-123">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="f151a-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f151a-124">Request headers</span></span>
| <span data-ttu-id="f151a-125">Имя</span><span class="sxs-lookup"><span data-stu-id="f151a-125">Name</span></span>       | <span data-ttu-id="f151a-126">Тип</span><span class="sxs-lookup"><span data-stu-id="f151a-126">Type</span></span> | <span data-ttu-id="f151a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="f151a-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f151a-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="f151a-128">Authorization</span></span>  | <span data-ttu-id="f151a-129">string</span><span class="sxs-lookup"><span data-stu-id="f151a-129">string</span></span>  | <span data-ttu-id="f151a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f151a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f151a-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f151a-132">Content-Type</span></span> | <span data-ttu-id="f151a-133">string</span><span class="sxs-lookup"><span data-stu-id="f151a-133">string</span></span>  | <span data-ttu-id="f151a-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f151a-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f151a-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f151a-136">Request body</span></span>
<span data-ttu-id="f151a-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f151a-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f151a-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="f151a-138">Parameter</span></span>    | <span data-ttu-id="f151a-139">Тип</span><span class="sxs-lookup"><span data-stu-id="f151a-139">Type</span></span>   |<span data-ttu-id="f151a-140">Описание</span><span class="sxs-lookup"><span data-stu-id="f151a-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f151a-141">comment</span><span class="sxs-lookup"><span data-stu-id="f151a-141">comment</span></span>|<span data-ttu-id="f151a-142">String</span><span class="sxs-lookup"><span data-stu-id="f151a-142">String</span></span>|<span data-ttu-id="f151a-143">Комментарий об отмене, отправленный всем участникам.</span><span class="sxs-lookup"><span data-stu-id="f151a-143">A comment about the cancellation sent to all the attendees.</span></span> <span data-ttu-id="f151a-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f151a-144">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="f151a-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="f151a-145">Response</span></span>

<span data-ttu-id="f151a-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f151a-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f151a-148">Пример</span><span class="sxs-lookup"><span data-stu-id="f151a-148">Example</span></span>
<span data-ttu-id="f151a-149">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f151a-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f151a-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="f151a-150">Request</span></span>
<span data-ttu-id="f151a-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f151a-151">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f151a-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="f151a-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_cancel"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/cancel
Content-type: application/json

{
  "Comment": "Cancelling for this week due to all hands"
}
```
# <a name="c"></a>[<span data-ttu-id="f151a-153">C#</span><span class="sxs-lookup"><span data-stu-id="f151a-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f151a-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f151a-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f151a-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f151a-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f151a-156">Java</span><span class="sxs-lookup"><span data-stu-id="f151a-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="f151a-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="f151a-157">Response</span></span>
<span data-ttu-id="f151a-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f151a-158">Here is an example of the response.</span></span>
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
  "description": "event: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
