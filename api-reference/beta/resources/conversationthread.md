---
title: Тип ресурса conversationThread
description: conversationThread — это коллекция экземпляров post.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: d541d4ac47272c2825602b28526b2b7c9d5f3fcb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933556"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="7a5d1-103">Тип ресурса conversationThread</span><span class="sxs-lookup"><span data-stu-id="7a5d1-103">conversationThread resource type</span></span>

> <span data-ttu-id="7a5d1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a5d1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7a5d1-106">conversationThread — это коллекция экземпляров [post](post.md).</span><span class="sxs-lookup"><span data-stu-id="7a5d1-106">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="7a5d1-p102">Коллекция получателей последней записи — это все получатели для цепочки. Коллекция получателей для цепочки может увеличиваться. При удалении получателя из цепочки создается новая цепочка.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-p102">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="7a5d1-110">Методы</span><span class="sxs-lookup"><span data-stu-id="7a5d1-110">Methods</span></span>

| <span data-ttu-id="7a5d1-111">Метод</span><span class="sxs-lookup"><span data-stu-id="7a5d1-111">Method</span></span>       | <span data-ttu-id="7a5d1-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7a5d1-112">Return Type</span></span>  |<span data-ttu-id="7a5d1-113">Описание</span><span class="sxs-lookup"><span data-stu-id="7a5d1-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7a5d1-114">Список цепочек бесед</span><span class="sxs-lookup"><span data-stu-id="7a5d1-114">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="7a5d1-115">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="7a5d1-115">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="7a5d1-116">Получение всех цепочек группы.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-116">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="7a5d1-117">Создание цепочки</span><span class="sxs-lookup"><span data-stu-id="7a5d1-117">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="7a5d1-118">conversationThread</span><span class="sxs-lookup"><span data-stu-id="7a5d1-118">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="7a5d1-p103">Создание беседы путем создания цепочки. В группе создаются беседа, цепочка беседы и запись.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-p103">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="7a5d1-121">Получение conversationThread</span><span class="sxs-lookup"><span data-stu-id="7a5d1-121">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="7a5d1-122">conversationThread</span><span class="sxs-lookup"><span data-stu-id="7a5d1-122">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="7a5d1-123">Получение определенной цепочки, принадлежащей группе.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-123">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="7a5d1-124">Обновление</span><span class="sxs-lookup"><span data-stu-id="7a5d1-124">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="7a5d1-125">conversationThread</span><span class="sxs-lookup"><span data-stu-id="7a5d1-125">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="7a5d1-126">Обновление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-126">Update conversationThread object.</span></span> |
|[<span data-ttu-id="7a5d1-127">Удаление</span><span class="sxs-lookup"><span data-stu-id="7a5d1-127">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="7a5d1-128">Нет</span><span class="sxs-lookup"><span data-stu-id="7a5d1-128">None</span></span> |<span data-ttu-id="7a5d1-129">Удаление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-129">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="7a5d1-130">reply</span><span class="sxs-lookup"><span data-stu-id="7a5d1-130">reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="7a5d1-131">Нет</span><span class="sxs-lookup"><span data-stu-id="7a5d1-131">None</span></span>|<span data-ttu-id="7a5d1-132">Создание ответа для этой цепочки с помощью создания сущности Post.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-132">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="7a5d1-133">Список сущностей Post</span><span class="sxs-lookup"><span data-stu-id="7a5d1-133">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="7a5d1-134">Коллекция [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="7a5d1-134">[post](post.md) collection</span></span>| <span data-ttu-id="7a5d1-135">Получение записей для указанной цепочки.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-135">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="7a5d1-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a5d1-136">Properties</span></span>
| <span data-ttu-id="7a5d1-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a5d1-137">Property</span></span>     | <span data-ttu-id="7a5d1-138">Тип</span><span class="sxs-lookup"><span data-stu-id="7a5d1-138">Type</span></span>   |<span data-ttu-id="7a5d1-139">Описание</span><span class="sxs-lookup"><span data-stu-id="7a5d1-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a5d1-140">id</span><span class="sxs-lookup"><span data-stu-id="7a5d1-140">id</span></span>|<span data-ttu-id="7a5d1-141">String</span><span class="sxs-lookup"><span data-stu-id="7a5d1-141">String</span></span>| <span data-ttu-id="7a5d1-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-142">Read-only.</span></span>|
|<span data-ttu-id="7a5d1-143">toRecipients</span><span class="sxs-lookup"><span data-stu-id="7a5d1-143">toRecipients</span></span>|<span data-ttu-id="7a5d1-144">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="7a5d1-144">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="7a5d1-145">Получатели в поле "Кому" для цепочки.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-145">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="7a5d1-146">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="7a5d1-146">ccRecipients</span></span>|<span data-ttu-id="7a5d1-147">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="7a5d1-147">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="7a5d1-148">Получатели в поле "Копия" для цепочки.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-148">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="7a5d1-149">topic</span><span class="sxs-lookup"><span data-stu-id="7a5d1-149">topic</span></span>|<span data-ttu-id="7a5d1-150">String</span><span class="sxs-lookup"><span data-stu-id="7a5d1-150">String</span></span>|<span data-ttu-id="7a5d1-p104">Тема беседы. Это свойство можно задать при создании беседы, но его невозможно обновить.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-p104">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="7a5d1-153">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="7a5d1-153">hasAttachments</span></span>|<span data-ttu-id="7a5d1-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a5d1-154">Boolean</span></span>|<span data-ttu-id="7a5d1-155">Указывает, содержит ли какая-либо запись в этой цепочке хотя бы одно вложение.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-155">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="7a5d1-156">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="7a5d1-156">lastDeliveredDateTime</span></span>|<span data-ttu-id="7a5d1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a5d1-157">DateTimeOffset</span></span>|<span data-ttu-id="7a5d1-p105">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7a5d1-160">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="7a5d1-160">uniqueSenders</span></span>|<span data-ttu-id="7a5d1-161">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7a5d1-161">String collection</span></span>|<span data-ttu-id="7a5d1-162">Все пользователи, которые отправили сообщение в эту цепочку.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-162">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="7a5d1-163">preview</span><span class="sxs-lookup"><span data-stu-id="7a5d1-163">preview</span></span>|<span data-ttu-id="7a5d1-164">String</span><span class="sxs-lookup"><span data-stu-id="7a5d1-164">String</span></span>|<span data-ttu-id="7a5d1-165">Краткая сводка из текста последней записи в этой беседе.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-165">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="7a5d1-166">isLocked</span><span class="sxs-lookup"><span data-stu-id="7a5d1-166">isLocked</span></span>|<span data-ttu-id="7a5d1-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a5d1-167">Boolean</span></span>|<span data-ttu-id="7a5d1-168">Указывает, заблокирована ли цепочка.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-168">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a5d1-169">Отношения</span><span class="sxs-lookup"><span data-stu-id="7a5d1-169">Relationships</span></span>
| <span data-ttu-id="7a5d1-170">Связь</span><span class="sxs-lookup"><span data-stu-id="7a5d1-170">Relationship</span></span> | <span data-ttu-id="7a5d1-171">Тип</span><span class="sxs-lookup"><span data-stu-id="7a5d1-171">Type</span></span>   |<span data-ttu-id="7a5d1-172">Описание</span><span class="sxs-lookup"><span data-stu-id="7a5d1-172">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a5d1-173">posts</span><span class="sxs-lookup"><span data-stu-id="7a5d1-173">posts</span></span>|<span data-ttu-id="7a5d1-174">Коллекция [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="7a5d1-174">[post](post.md) collection</span></span>| <span data-ttu-id="7a5d1-p106">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a5d1-177">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a5d1-177">JSON representation</span></span>

<span data-ttu-id="7a5d1-178">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a5d1-178">Here is a JSON representation of the resource</span></span>

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
