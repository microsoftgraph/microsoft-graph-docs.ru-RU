---
title: Удаление вложения
description: Удаление вложения из данных календаря о событии, сообщения почты или записи группы.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: db7f6282644443d459bba1655ecd01bce1955382
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434932"
---
# <a name="delete-attachment"></a><span data-ttu-id="8b2e9-103">Удаление вложения</span><span class="sxs-lookup"><span data-stu-id="8b2e9-103">Delete attachment</span></span>

<span data-ttu-id="8b2e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b2e9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8b2e9-105">Удаление вложения из события календаря пользователя, сообщения электронной почты или группового сообщения.</span><span class="sxs-lookup"><span data-stu-id="8b2e9-105">Delete an attachment from a user calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b2e9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b2e9-106">Permissions</span></span>

<span data-ttu-id="8b2e9-107">В зависимости от **ресурса (события,** сообщения, **outlookTask** или **сообщения),** к который присоединено вложение и запрашиваемого типа разрешений (делегирован или приложения), разрешение, указанное в следующей таблице, является наименее привилегированным, требуемого для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8b2e9-107">Depending on the resource (**event**, **message**, **outlookTask**, or **post**) that the attachment is attached to and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="8b2e9-108">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b2e9-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b2e9-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="8b2e9-109">Supported resource</span></span> | <span data-ttu-id="8b2e9-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b2e9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8b2e9-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b2e9-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b2e9-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b2e9-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="8b2e9-113">event</span><span class="sxs-lookup"><span data-stu-id="8b2e9-113">event</span></span>](../resources/event.md) | <span data-ttu-id="8b2e9-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b2e9-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="8b2e9-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b2e9-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="8b2e9-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b2e9-116">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="8b2e9-117">message</span><span class="sxs-lookup"><span data-stu-id="8b2e9-117">message</span></span>](../resources/message.md) | <span data-ttu-id="8b2e9-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b2e9-118">Mail.ReadWrite</span></span> | <span data-ttu-id="8b2e9-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b2e9-119">Mail.ReadWrite</span></span> | <span data-ttu-id="8b2e9-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b2e9-120">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="8b2e9-121">post</span><span class="sxs-lookup"><span data-stu-id="8b2e9-121">post</span></span>](../resources/post.md) | <span data-ttu-id="8b2e9-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b2e9-122">Group.ReadWrite.All</span></span> | <span data-ttu-id="8b2e9-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b2e9-123">Not supported</span></span> | <span data-ttu-id="8b2e9-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b2e9-124">Not supported</span></span> |


<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All.
-->

## <a name="http-request"></a><span data-ttu-id="8b2e9-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b2e9-125">HTTP request</span></span>
<span data-ttu-id="8b2e9-126">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b2e9-126">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}

DELETE /me/calendar/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<span data-ttu-id="8b2e9-127">Вложения для [события](../resources/event.md) в указанном [календаре,](../resources/calendar.md) принадлежащем пользователю.</span><span class="sxs-lookup"><span data-stu-id="8b2e9-127">Attachments for an [event](../resources/event.md) in the specified [calendar](../resources/calendar.md) belonging to the user.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}
```

<!-- Tried adding and getting group event with attachment, event exists but without attachment. Assume group event attachment not supported.
DELETE /groups/{id}/events/{id}/attachments/{id}
DELETE /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="8b2e9-128">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b2e9-128">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="8b2e9-129">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b2e9-129">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="8b2e9-130">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b2e9-130">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="8b2e9-131">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b2e9-131">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="8b2e9-p102">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д. </span><span class="sxs-lookup"><span data-stu-id="8b2e9-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="8b2e9-134">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="8b2e9-134">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8b2e9-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b2e9-135">Request headers</span></span>
| <span data-ttu-id="8b2e9-136">Имя</span><span class="sxs-lookup"><span data-stu-id="8b2e9-136">Name</span></span>       | <span data-ttu-id="8b2e9-137">Тип</span><span class="sxs-lookup"><span data-stu-id="8b2e9-137">Type</span></span> | <span data-ttu-id="8b2e9-138">Описание</span><span class="sxs-lookup"><span data-stu-id="8b2e9-138">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8b2e9-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b2e9-139">Authorization</span></span>  | <span data-ttu-id="8b2e9-140">string</span><span class="sxs-lookup"><span data-stu-id="8b2e9-140">string</span></span>  | <span data-ttu-id="8b2e9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b2e9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b2e9-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b2e9-143">Request body</span></span>
<span data-ttu-id="8b2e9-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b2e9-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b2e9-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b2e9-145">Response</span></span>

<span data-ttu-id="8b2e9-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8b2e9-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b2e9-148">Пример</span><span class="sxs-lookup"><span data-stu-id="8b2e9-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b2e9-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b2e9-149">Request</span></span>
<span data-ttu-id="8b2e9-150">Ниже приведен пример запроса на удаление вложения из данных, касающихся события.</span><span class="sxs-lookup"><span data-stu-id="8b2e9-150">Here is an example of the request to delete an attachment on an event.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b2e9-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b2e9-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
# <a name="c"></a>[<span data-ttu-id="8b2e9-152">C#</span><span class="sxs-lookup"><span data-stu-id="8b2e9-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b2e9-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b2e9-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b2e9-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b2e9-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b2e9-155">Java</span><span class="sxs-lookup"><span data-stu-id="8b2e9-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8b2e9-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b2e9-156">Response</span></span>
<span data-ttu-id="8b2e9-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8b2e9-157">Here is an example of the response.</span></span>
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

