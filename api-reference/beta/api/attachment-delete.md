---
title: Удаление вложения
description: Удаление вложения из события календаря, сообщения, задачи Outlook или post.
ms.openlocfilehash: dbabde6b1783e477e3a15db3ea4d138be6e41b12
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771788"
---
# <a name="delete-attachment"></a><span data-ttu-id="947b6-103">Удаление вложения</span><span class="sxs-lookup"><span data-stu-id="947b6-103">Delete attachment</span></span>

> <span data-ttu-id="947b6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="947b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="947b6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="947b6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="947b6-106">Удаление вложения из календаря [события](../resources/event.md), [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [публикации](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="947b6-106">Delete an attachment from a calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="947b6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="947b6-107">Permissions</span></span>

<span data-ttu-id="947b6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="947b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="947b6-110">Если доступ к вложений в сообщениях: Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="947b6-110">If accessing attachments in messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="947b6-111">Если доступ к вложениям в события: Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="947b6-111">If accessing attachments in events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="947b6-112">Если доступ к вложениям с задачами Outlook: Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="947b6-112">If accessing attachments in Outlook tasks: Tasks.ReadWrite</span></span>
* <span data-ttu-id="947b6-113">Если доступ к вложениям в группу публикации: Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="947b6-113">If accessing attachments in group posts: Group.ReadWrite.All</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="947b6-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="947b6-114">HTTP request</span></span>

<span data-ttu-id="947b6-115">Вложения для [события](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="947b6-115">Attachments for an [event](../resources/event.md).</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="947b6-116">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="947b6-116">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="947b6-117">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="947b6-117">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="947b6-118">Вложения для [сообщений](../resources/message.md) , содержащихся в дочерней папкой [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="947b6-118">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="947b6-119">В приведенном ниже примере показана один уровень вложения, но сообщение может быть найдена в дочерних дочернего и т. д.</span><span class="sxs-lookup"><span data-stu-id="947b6-119">The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="947b6-120">Вложения для [задач Outlook](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="947b6-120">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}
```

<span data-ttu-id="947b6-121">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="947b6-121">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="947b6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="947b6-122">Request headers</span></span>

| <span data-ttu-id="947b6-123">Имя</span><span class="sxs-lookup"><span data-stu-id="947b6-123">Name</span></span>       | <span data-ttu-id="947b6-124">Тип</span><span class="sxs-lookup"><span data-stu-id="947b6-124">Type</span></span> | <span data-ttu-id="947b6-125">Описание</span><span class="sxs-lookup"><span data-stu-id="947b6-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="947b6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="947b6-126">Authorization</span></span>  | <span data-ttu-id="947b6-127">string</span><span class="sxs-lookup"><span data-stu-id="947b6-127">string</span></span>  | <span data-ttu-id="947b6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="947b6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="947b6-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="947b6-130">Request body</span></span>

<span data-ttu-id="947b6-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="947b6-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="947b6-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="947b6-132">Response</span></span>

<span data-ttu-id="947b6-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="947b6-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="947b6-135">Пример</span><span class="sxs-lookup"><span data-stu-id="947b6-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="947b6-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="947b6-136">Request</span></span>

<span data-ttu-id="947b6-137">Ниже приведен пример запроса на удаление вложения из данных, касающихся события.</span><span class="sxs-lookup"><span data-stu-id="947b6-137">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```

### <a name="response"></a><span data-ttu-id="947b6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="947b6-138">Response</span></span>

<span data-ttu-id="947b6-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="947b6-139">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->
