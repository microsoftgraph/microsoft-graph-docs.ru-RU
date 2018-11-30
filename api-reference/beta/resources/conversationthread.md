---
title: Тип ресурса conversationThread
description: conversationThread — это коллекция экземпляров post.
ms.openlocfilehash: a63b208e30372c2cced1e440f3a46e605ea26589
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075115"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="1459d-103">Тип ресурса conversationThread</span><span class="sxs-lookup"><span data-stu-id="1459d-103">conversationThread resource type</span></span>

> <span data-ttu-id="1459d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1459d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1459d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1459d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1459d-106">conversationThread — это коллекция экземпляров [post](post.md).</span><span class="sxs-lookup"><span data-stu-id="1459d-106">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="1459d-p102">Коллекция получателей последней записи — это все получатели для цепочки. Коллекция получателей для цепочки может увеличиваться. При удалении получателя из цепочки создается новая цепочка.</span><span class="sxs-lookup"><span data-stu-id="1459d-p102">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="1459d-110">Методы</span><span class="sxs-lookup"><span data-stu-id="1459d-110">Methods</span></span>

| <span data-ttu-id="1459d-111">Метод</span><span class="sxs-lookup"><span data-stu-id="1459d-111">Method</span></span>       | <span data-ttu-id="1459d-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1459d-112">Return Type</span></span>  |<span data-ttu-id="1459d-113">Описание</span><span class="sxs-lookup"><span data-stu-id="1459d-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1459d-114">Список цепочек бесед</span><span class="sxs-lookup"><span data-stu-id="1459d-114">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="1459d-115">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="1459d-115">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="1459d-116">Получение всех цепочек группы.</span><span class="sxs-lookup"><span data-stu-id="1459d-116">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="1459d-117">Создание цепочки</span><span class="sxs-lookup"><span data-stu-id="1459d-117">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="1459d-118">conversationThread</span><span class="sxs-lookup"><span data-stu-id="1459d-118">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="1459d-p103">Создание беседы путем создания цепочки. В группе создаются беседа, цепочка беседы и запись.</span><span class="sxs-lookup"><span data-stu-id="1459d-p103">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="1459d-121">Получение conversationThread</span><span class="sxs-lookup"><span data-stu-id="1459d-121">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="1459d-122">conversationThread</span><span class="sxs-lookup"><span data-stu-id="1459d-122">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="1459d-123">Получение определенной цепочки, принадлежащей группе.</span><span class="sxs-lookup"><span data-stu-id="1459d-123">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="1459d-124">Обновление</span><span class="sxs-lookup"><span data-stu-id="1459d-124">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="1459d-125">conversationThread</span><span class="sxs-lookup"><span data-stu-id="1459d-125">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="1459d-126">Обновление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="1459d-126">Update conversationThread object.</span></span> |
|[<span data-ttu-id="1459d-127">Удаление</span><span class="sxs-lookup"><span data-stu-id="1459d-127">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="1459d-128">Нет</span><span class="sxs-lookup"><span data-stu-id="1459d-128">None</span></span> |<span data-ttu-id="1459d-129">Удаление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="1459d-129">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="1459d-130">reply</span><span class="sxs-lookup"><span data-stu-id="1459d-130">reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="1459d-131">Нет</span><span class="sxs-lookup"><span data-stu-id="1459d-131">None</span></span>|<span data-ttu-id="1459d-132">Создание ответа для этой цепочки с помощью создания сущности Post.</span><span class="sxs-lookup"><span data-stu-id="1459d-132">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="1459d-133">Список сущностей Post</span><span class="sxs-lookup"><span data-stu-id="1459d-133">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="1459d-134">Коллекция [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="1459d-134">[post](post.md) collection</span></span>| <span data-ttu-id="1459d-135">Получение записей для указанной цепочки.</span><span class="sxs-lookup"><span data-stu-id="1459d-135">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="1459d-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="1459d-136">Properties</span></span>
| <span data-ttu-id="1459d-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="1459d-137">Property</span></span>     | <span data-ttu-id="1459d-138">Тип</span><span class="sxs-lookup"><span data-stu-id="1459d-138">Type</span></span>   |<span data-ttu-id="1459d-139">Описание</span><span class="sxs-lookup"><span data-stu-id="1459d-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1459d-140">id</span><span class="sxs-lookup"><span data-stu-id="1459d-140">id</span></span>|<span data-ttu-id="1459d-141">String</span><span class="sxs-lookup"><span data-stu-id="1459d-141">String</span></span>| <span data-ttu-id="1459d-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1459d-142">Read-only.</span></span>|
|<span data-ttu-id="1459d-143">toRecipients</span><span class="sxs-lookup"><span data-stu-id="1459d-143">toRecipients</span></span>|<span data-ttu-id="1459d-144">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="1459d-144">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="1459d-145">Получатели в поле "Кому" для цепочки.</span><span class="sxs-lookup"><span data-stu-id="1459d-145">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="1459d-146">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="1459d-146">ccRecipients</span></span>|<span data-ttu-id="1459d-147">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="1459d-147">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="1459d-148">Получатели в поле "Копия" для цепочки.</span><span class="sxs-lookup"><span data-stu-id="1459d-148">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="1459d-149">topic</span><span class="sxs-lookup"><span data-stu-id="1459d-149">topic</span></span>|<span data-ttu-id="1459d-150">String</span><span class="sxs-lookup"><span data-stu-id="1459d-150">String</span></span>|<span data-ttu-id="1459d-p104">Тема беседы. Это свойство можно задать при создании беседы, но его невозможно обновить.</span><span class="sxs-lookup"><span data-stu-id="1459d-p104">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="1459d-153">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="1459d-153">hasAttachments</span></span>|<span data-ttu-id="1459d-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="1459d-154">Boolean</span></span>|<span data-ttu-id="1459d-155">Указывает, содержит ли какая-либо запись в этой цепочке хотя бы одно вложение.</span><span class="sxs-lookup"><span data-stu-id="1459d-155">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="1459d-156">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="1459d-156">lastDeliveredDateTime</span></span>|<span data-ttu-id="1459d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1459d-157">DateTimeOffset</span></span>|<span data-ttu-id="1459d-p105">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1459d-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1459d-160">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="1459d-160">uniqueSenders</span></span>|<span data-ttu-id="1459d-161">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1459d-161">String collection</span></span>|<span data-ttu-id="1459d-162">Все пользователи, которые отправили сообщение в эту цепочку.</span><span class="sxs-lookup"><span data-stu-id="1459d-162">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="1459d-163">preview</span><span class="sxs-lookup"><span data-stu-id="1459d-163">preview</span></span>|<span data-ttu-id="1459d-164">String</span><span class="sxs-lookup"><span data-stu-id="1459d-164">String</span></span>|<span data-ttu-id="1459d-165">Краткая сводка из текста последней записи в этой беседе.</span><span class="sxs-lookup"><span data-stu-id="1459d-165">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="1459d-166">isLocked</span><span class="sxs-lookup"><span data-stu-id="1459d-166">isLocked</span></span>|<span data-ttu-id="1459d-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="1459d-167">Boolean</span></span>|<span data-ttu-id="1459d-168">Указывает, заблокирована ли цепочка.</span><span class="sxs-lookup"><span data-stu-id="1459d-168">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1459d-169">Отношения</span><span class="sxs-lookup"><span data-stu-id="1459d-169">Relationships</span></span>
| <span data-ttu-id="1459d-170">Связь</span><span class="sxs-lookup"><span data-stu-id="1459d-170">Relationship</span></span> | <span data-ttu-id="1459d-171">Тип</span><span class="sxs-lookup"><span data-stu-id="1459d-171">Type</span></span>   |<span data-ttu-id="1459d-172">Описание</span><span class="sxs-lookup"><span data-stu-id="1459d-172">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1459d-173">posts</span><span class="sxs-lookup"><span data-stu-id="1459d-173">posts</span></span>|<span data-ttu-id="1459d-174">Коллекция [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="1459d-174">[post](post.md) collection</span></span>| <span data-ttu-id="1459d-p106">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1459d-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1459d-177">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1459d-177">JSON representation</span></span>

<span data-ttu-id="1459d-178">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1459d-178">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationThread"
}-->

```json
{
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": true,
  "id": "string (identifier)",
  "isLocked": true,
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
