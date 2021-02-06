---
title: Удаление вложения
description: Удаление вложения из события календаря, сообщения, задачи Outlook или публикации.
localization_priority: Normal
doc_type: apiPageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 4df50de17e1926407545cb5e6b18ae6aa56af018
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128871"
---
# <a name="delete-attachment"></a><span data-ttu-id="05e9f-103">Удаление вложения</span><span class="sxs-lookup"><span data-stu-id="05e9f-103">Delete attachment</span></span>

<span data-ttu-id="05e9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05e9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="05e9f-105">Удаление вложения из события календаря [пользователя,](../resources/event.md) [сообщения,](../resources/message.md) [задачи Outlook](../resources/outlooktask.md)или [публикации.](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="05e9f-105">Delete an attachment from a user calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="05e9f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05e9f-106">Permissions</span></span>

<span data-ttu-id="05e9f-107">В зависимости от ресурса **(события,** **сообщения,**  **outlookTask** или post), к который вложено вложение, и типа запрашиваемого разрешения (делегирование или приложение), разрешение, указанное в следующей таблице, является наименее привилегированным для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="05e9f-107">Depending on the resource (**event**, **message**, **outlookTask**, or **post**) that the attachment is attached to and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="05e9f-108">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05e9f-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05e9f-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="05e9f-109">Supported resource</span></span> | <span data-ttu-id="05e9f-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05e9f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="05e9f-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05e9f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05e9f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05e9f-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="05e9f-113">event</span><span class="sxs-lookup"><span data-stu-id="05e9f-113">event</span></span>](../resources/event.md) | <span data-ttu-id="05e9f-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05e9f-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="05e9f-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05e9f-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="05e9f-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05e9f-116">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="05e9f-117">message</span><span class="sxs-lookup"><span data-stu-id="05e9f-117">message</span></span>](../resources/message.md) | <span data-ttu-id="05e9f-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05e9f-118">Mail.ReadWrite</span></span> | <span data-ttu-id="05e9f-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05e9f-119">Mail.ReadWrite</span></span> | <span data-ttu-id="05e9f-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05e9f-120">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="05e9f-121">outlookTask</span><span class="sxs-lookup"><span data-stu-id="05e9f-121">outlookTask</span></span>](../resources/outlooktask.md) |  <span data-ttu-id="05e9f-122">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05e9f-122">Tasks.ReadWrite</span></span> | <span data-ttu-id="05e9f-123">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05e9f-123">Tasks.ReadWrite</span></span> | <span data-ttu-id="05e9f-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="05e9f-124">Not supported</span></span> |
| [<span data-ttu-id="05e9f-125">post</span><span class="sxs-lookup"><span data-stu-id="05e9f-125">post</span></span>](../resources/post.md) | <span data-ttu-id="05e9f-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05e9f-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="05e9f-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="05e9f-127">Not supported</span></span> | <span data-ttu-id="05e9f-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="05e9f-128">Not supported</span></span> |


<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="05e9f-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05e9f-129">HTTP request</span></span>

<span data-ttu-id="05e9f-130">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="05e9f-130">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}

DELETE /me/calendar/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<span data-ttu-id="05e9f-131">Вложения для [события в](../resources/event.md) указанном календаре, принадлежащем пользователю. [](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="05e9f-131">Attachments for an [event](../resources/event.md) in the specified [calendar](../resources/calendar.md) belonging to the user.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}
```

<!-- Tried adding and getting group event with attachment, event exists but without attachment. Group event attachment not supported.
DELETE /groups/{id}/events/{id}/attachments/{id}
DELETE /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="05e9f-132">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="05e9f-132">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="05e9f-133">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="05e9f-133">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="05e9f-134">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="05e9f-134">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="05e9f-135">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="05e9f-135">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="05e9f-p102">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д. </span><span class="sxs-lookup"><span data-stu-id="05e9f-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="05e9f-138">Вложения для задачи [Outlook.](../resources/outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="05e9f-138">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}/attachments/{id}
DELETE /users/{id}/outlook/tasks/{id}/attachments/{id}
```

<span data-ttu-id="05e9f-139">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="05e9f-139">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="05e9f-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05e9f-140">Request headers</span></span>

| <span data-ttu-id="05e9f-141">Имя</span><span class="sxs-lookup"><span data-stu-id="05e9f-141">Name</span></span>       | <span data-ttu-id="05e9f-142">Тип</span><span class="sxs-lookup"><span data-stu-id="05e9f-142">Type</span></span> | <span data-ttu-id="05e9f-143">Описание</span><span class="sxs-lookup"><span data-stu-id="05e9f-143">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="05e9f-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="05e9f-144">Authorization</span></span>  | <span data-ttu-id="05e9f-145">string</span><span class="sxs-lookup"><span data-stu-id="05e9f-145">string</span></span>  | <span data-ttu-id="05e9f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05e9f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="05e9f-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05e9f-148">Request body</span></span>

<span data-ttu-id="05e9f-149">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="05e9f-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05e9f-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="05e9f-150">Response</span></span>

<span data-ttu-id="05e9f-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="05e9f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05e9f-153">Пример</span><span class="sxs-lookup"><span data-stu-id="05e9f-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="05e9f-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="05e9f-154">Request</span></span>

<span data-ttu-id="05e9f-155">Ниже приведен пример запроса на удаление вложения из данных, касающихся события.</span><span class="sxs-lookup"><span data-stu-id="05e9f-155">Here is an example of the request to delete an attachment on an event.</span></span>

# <a name="http"></a>[<span data-ttu-id="05e9f-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="05e9f-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```
# <a name="c"></a>[<span data-ttu-id="05e9f-157">C#</span><span class="sxs-lookup"><span data-stu-id="05e9f-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05e9f-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05e9f-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05e9f-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05e9f-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="05e9f-160">Java</span><span class="sxs-lookup"><span data-stu-id="05e9f-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="05e9f-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="05e9f-161">Response</span></span>

<span data-ttu-id="05e9f-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="05e9f-162">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


