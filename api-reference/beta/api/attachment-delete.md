---
title: Удаление вложения
description: Удаление вложения из события календаря, сообщения, задачи Outlook или POST.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3ae0c24fdcfd8d433300f20459c85ece28b97acb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945335"
---
# <a name="delete-attachment"></a><span data-ttu-id="964d1-103">Удаление вложения</span><span class="sxs-lookup"><span data-stu-id="964d1-103">Delete attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="964d1-104">Удаление вложения из [события](../resources/event.md)календаря, [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [POST](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="964d1-104">Delete an attachment from a calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="964d1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="964d1-105">Permissions</span></span>

<span data-ttu-id="964d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="964d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="964d1-108">При доступе к вложениям в сообщениях: mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="964d1-108">If accessing attachments in messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="964d1-109">При доступе к вложениям в событиях: Calendars. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="964d1-109">If accessing attachments in events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="964d1-110">При доступе к вложениям в задачах Outlook: Tasks. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="964d1-110">If accessing attachments in Outlook tasks: Tasks.ReadWrite</span></span>
* <span data-ttu-id="964d1-111">При доступе к вложениям в записях групп: Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="964d1-111">If accessing attachments in group posts: Group.ReadWrite.All</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="964d1-112">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="964d1-112">HTTP request</span></span>

<span data-ttu-id="964d1-113">Вложения для [события](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="964d1-113">Attachments for an [event](../resources/event.md).</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="964d1-114">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="964d1-114">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="964d1-115">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="964d1-115">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="964d1-p102">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д.</span><span class="sxs-lookup"><span data-stu-id="964d1-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="964d1-118">Вложения для [задачи Outlook](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="964d1-118">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}
```

<span data-ttu-id="964d1-119">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="964d1-119">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="964d1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="964d1-120">Request headers</span></span>

| <span data-ttu-id="964d1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="964d1-121">Name</span></span>       | <span data-ttu-id="964d1-122">Тип</span><span class="sxs-lookup"><span data-stu-id="964d1-122">Type</span></span> | <span data-ttu-id="964d1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="964d1-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="964d1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="964d1-124">Authorization</span></span>  | <span data-ttu-id="964d1-125">string</span><span class="sxs-lookup"><span data-stu-id="964d1-125">string</span></span>  | <span data-ttu-id="964d1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="964d1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="964d1-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="964d1-128">Request body</span></span>

<span data-ttu-id="964d1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="964d1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="964d1-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="964d1-130">Response</span></span>

<span data-ttu-id="964d1-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="964d1-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="964d1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="964d1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="964d1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="964d1-134">Request</span></span>

<span data-ttu-id="964d1-135">Ниже приведен пример запроса на удаление вложения из данных, касающихся события.</span><span class="sxs-lookup"><span data-stu-id="964d1-135">Here is an example of the request to delete an attachment on an event.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="964d1-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="964d1-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="964d1-137">C#</span><span class="sxs-lookup"><span data-stu-id="964d1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="964d1-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="964d1-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="964d1-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="964d1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="964d1-140">Java</span><span class="sxs-lookup"><span data-stu-id="964d1-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="964d1-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="964d1-141">Response</span></span>

<span data-ttu-id="964d1-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="964d1-142">Here is an example of the response.</span></span>
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
