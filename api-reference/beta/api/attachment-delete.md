---
title: Удаление вложения
description: Удаление вложения из события календаря, сообщения, задачи Outlook или POST.
localization_priority: Normal
ms.openlocfilehash: 8b9e70153c80371afcb147da6183a1f78135e283
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636410"
---
# <a name="delete-attachment"></a><span data-ttu-id="c5645-103">Удаление вложения</span><span class="sxs-lookup"><span data-stu-id="c5645-103">Delete attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5645-104">Удаление вложения из [события](../resources/event.md)календаря, [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [POST](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="c5645-104">Delete an attachment from a calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c5645-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5645-105">Permissions</span></span>

<span data-ttu-id="c5645-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5645-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="c5645-108">При доступе к вложениям в сообщениях: mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5645-108">If accessing attachments in messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="c5645-109">При доступе к вложениям в событиях: Calendars. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5645-109">If accessing attachments in events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="c5645-110">При доступе к вложениям в задачах Outlook: Tasks. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5645-110">If accessing attachments in Outlook tasks: Tasks.ReadWrite</span></span>
* <span data-ttu-id="c5645-111">При доступе к вложениям в записях групп: Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c5645-111">If accessing attachments in group posts: Group.ReadWrite.All</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="c5645-112">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5645-112">HTTP request</span></span>

<span data-ttu-id="c5645-113">Вложения для [события](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="c5645-113">Attachments for an [event](../resources/event.md).</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="c5645-114">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="c5645-114">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="c5645-115">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="c5645-115">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="c5645-p102">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д. </span><span class="sxs-lookup"><span data-stu-id="c5645-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="c5645-118">Вложения для [задачи Outlook](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="c5645-118">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}
```

<span data-ttu-id="c5645-119">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="c5645-119">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c5645-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5645-120">Request headers</span></span>

| <span data-ttu-id="c5645-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c5645-121">Name</span></span>       | <span data-ttu-id="c5645-122">Тип</span><span class="sxs-lookup"><span data-stu-id="c5645-122">Type</span></span> | <span data-ttu-id="c5645-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c5645-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c5645-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5645-124">Authorization</span></span>  | <span data-ttu-id="c5645-125">string</span><span class="sxs-lookup"><span data-stu-id="c5645-125">string</span></span>  | <span data-ttu-id="c5645-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5645-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5645-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5645-128">Request body</span></span>

<span data-ttu-id="c5645-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5645-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5645-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5645-130">Response</span></span>

<span data-ttu-id="c5645-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c5645-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5645-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c5645-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5645-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5645-134">Request</span></span>

<span data-ttu-id="c5645-135">Ниже приведен пример запроса на удаление вложения из данных, касающихся события.</span><span class="sxs-lookup"><span data-stu-id="c5645-135">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```

### <a name="response"></a><span data-ttu-id="c5645-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5645-136">Response</span></span>

<span data-ttu-id="c5645-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c5645-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c5645-138">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="c5645-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c5645-139">Языках</span><span class="sxs-lookup"><span data-stu-id="c5645-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_attachment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c5645-140">Язык</span><span class="sxs-lookup"><span data-stu-id="c5645-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_attachment-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/attachment-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/attachment-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
