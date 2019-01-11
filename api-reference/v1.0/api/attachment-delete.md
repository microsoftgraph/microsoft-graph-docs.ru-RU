---
title: Удаление вложения
description: Удаление вложения из данных календаря о событии, сообщения почты или записи группы.
localization_priority: Normal
ms.openlocfilehash: f6ac2e60c9fdc8a224e22a49e6928cdc41e9730b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816998"
---
# <a name="delete-attachment"></a><span data-ttu-id="5bc03-103">Удаление вложения</span><span class="sxs-lookup"><span data-stu-id="5bc03-103">Delete attachment</span></span>

<span data-ttu-id="5bc03-104">Удаление вложения из данных календаря о событии, сообщения почты или записи группы.</span><span class="sxs-lookup"><span data-stu-id="5bc03-104">Delete an attachment from a calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="5bc03-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5bc03-105">Permissions</span></span>
<span data-ttu-id="5bc03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bc03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="5bc03-108">Если доступ к вложений в сообщениях: Mail.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="5bc03-108">If accessing attachments in messages: Mail.ReadWrite.</span></span>
* <span data-ttu-id="5bc03-109">Если доступ к вложениям в события: Calendars.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="5bc03-109">If accessing attachments in events: Calendars.ReadWrite.</span></span>
* <span data-ttu-id="5bc03-110">Если доступ к вложениям в группу публикации: Group.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="5bc03-110">If accessing attachments in group posts: Group.ReadWrite.All.</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All.
-->

## <a name="http-request"></a><span data-ttu-id="5bc03-111">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bc03-111">HTTP request</span></span>
<span data-ttu-id="5bc03-112">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md) по умолчанию для пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="5bc03-112">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}

DELETE /me/calendar/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
DELETE /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="5bc03-113">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bc03-113">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="5bc03-114">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bc03-114">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="5bc03-115">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bc03-115">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="5bc03-116">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bc03-116">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="5bc03-117">Вложения для [сообщений](../resources/message.md) , содержащихся в дочерней папкой [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bc03-117">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="5bc03-118">В приведенном ниже примере показана один уровень вложения, но сообщение может быть найдена в дочерних дочернего и т. д.</span><span class="sxs-lookup"><span data-stu-id="5bc03-118">The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="5bc03-119">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="5bc03-119">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5bc03-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5bc03-120">Request headers</span></span>
| <span data-ttu-id="5bc03-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5bc03-121">Name</span></span>       | <span data-ttu-id="5bc03-122">Тип</span><span class="sxs-lookup"><span data-stu-id="5bc03-122">Type</span></span> | <span data-ttu-id="5bc03-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5bc03-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5bc03-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bc03-124">Authorization</span></span>  | <span data-ttu-id="5bc03-125">string</span><span class="sxs-lookup"><span data-stu-id="5bc03-125">string</span></span>  | <span data-ttu-id="5bc03-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bc03-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bc03-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5bc03-128">Request body</span></span>
<span data-ttu-id="5bc03-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5bc03-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bc03-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bc03-130">Response</span></span>

<span data-ttu-id="5bc03-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5bc03-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bc03-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5bc03-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5bc03-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bc03-134">Request</span></span>
<span data-ttu-id="5bc03-135">Ниже приведен пример запроса на удаление вложения из данных, касающихся события.</span><span class="sxs-lookup"><span data-stu-id="5bc03-135">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="5bc03-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bc03-136">Response</span></span>
<span data-ttu-id="5bc03-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5bc03-137">Here is an example of the response.</span></span>
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
