---
title: Удаление вложения
description: Удаление вложения из данных календаря о событии, сообщения почты или записи группы.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9ab10522c4f0f2a73c78ac12ddf2995aae89ae3a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046029"
---
# <a name="delete-attachment"></a><span data-ttu-id="f47ea-103">Удаление вложения</span><span class="sxs-lookup"><span data-stu-id="f47ea-103">Delete attachment</span></span>

<span data-ttu-id="f47ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f47ea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f47ea-105">Удаление вложения из события календаря пользователя, сообщения электронной почты или записи группы.</span><span class="sxs-lookup"><span data-stu-id="f47ea-105">Delete an attachment from a user calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="f47ea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f47ea-106">Permissions</span></span>
<span data-ttu-id="f47ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f47ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="f47ea-109">При доступе к вложениям в сообщениях: mail. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="f47ea-109">If accessing attachments in messages: Mail.ReadWrite.</span></span>
* <span data-ttu-id="f47ea-110">При доступе к вложениям в событиях: Calendars. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="f47ea-110">If accessing attachments in events: Calendars.ReadWrite.</span></span>
* <span data-ttu-id="f47ea-111">При доступе к вложениям в записях групп: Group. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="f47ea-111">If accessing attachments in group posts: Group.ReadWrite.All.</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All.
-->

## <a name="http-request"></a><span data-ttu-id="f47ea-112">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f47ea-112">HTTP request</span></span>
<span data-ttu-id="f47ea-113">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f47ea-113">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}

DELETE /me/calendar/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<span data-ttu-id="f47ea-114">Вложения для [события](../resources/event.md) в указанном [календаре](../resources/calendar.md) , принадлежащее пользователю.</span><span class="sxs-lookup"><span data-stu-id="f47ea-114">Attachments for an [event](../resources/event.md) in the specified [calendar](../resources/calendar.md) belonging to the user.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}
```

<!-- Tried adding and getting group event with attachment, event exists but without attachment. Assume group event attachment not supported.
DELETE /groups/{id}/events/{id}/attachments/{id}
DELETE /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="f47ea-115">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f47ea-115">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="f47ea-116">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="f47ea-116">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="f47ea-117">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="f47ea-117">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="f47ea-118">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="f47ea-118">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="f47ea-p102">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д. </span><span class="sxs-lookup"><span data-stu-id="f47ea-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="f47ea-121">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="f47ea-121">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f47ea-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f47ea-122">Request headers</span></span>
| <span data-ttu-id="f47ea-123">Имя</span><span class="sxs-lookup"><span data-stu-id="f47ea-123">Name</span></span>       | <span data-ttu-id="f47ea-124">Тип</span><span class="sxs-lookup"><span data-stu-id="f47ea-124">Type</span></span> | <span data-ttu-id="f47ea-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f47ea-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f47ea-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f47ea-126">Authorization</span></span>  | <span data-ttu-id="f47ea-127">string</span><span class="sxs-lookup"><span data-stu-id="f47ea-127">string</span></span>  | <span data-ttu-id="f47ea-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f47ea-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f47ea-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f47ea-130">Request body</span></span>
<span data-ttu-id="f47ea-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f47ea-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f47ea-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f47ea-132">Response</span></span>

<span data-ttu-id="f47ea-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f47ea-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f47ea-135">Пример</span><span class="sxs-lookup"><span data-stu-id="f47ea-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f47ea-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="f47ea-136">Request</span></span>
<span data-ttu-id="f47ea-137">Ниже приведен пример запроса на удаление вложения из данных, касающихся события.</span><span class="sxs-lookup"><span data-stu-id="f47ea-137">Here is an example of the request to delete an attachment on an event.</span></span>

# <a name="http"></a>[<span data-ttu-id="f47ea-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="f47ea-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
# <a name="c"></a>[<span data-ttu-id="f47ea-139">C#</span><span class="sxs-lookup"><span data-stu-id="f47ea-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f47ea-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f47ea-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f47ea-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f47ea-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f47ea-142">Java</span><span class="sxs-lookup"><span data-stu-id="f47ea-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f47ea-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f47ea-143">Response</span></span>
<span data-ttu-id="f47ea-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f47ea-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

