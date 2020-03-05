---
title: Тип ресурса conversationThread
description: conversationThread — это коллекция экземпляров post.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 55a8b414022a338628264fe09e58559a52c3fbcd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507396"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="6880a-103">Тип ресурса conversationThread</span><span class="sxs-lookup"><span data-stu-id="6880a-103">conversationThread resource type</span></span>

<span data-ttu-id="6880a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6880a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6880a-105">conversationThread — это коллекция экземпляров [post](post.md).</span><span class="sxs-lookup"><span data-stu-id="6880a-105">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="6880a-p101">Коллекция получателей последней записи — это все получатели для цепочки. Коллекция получателей для цепочки может увеличиваться. При удалении получателя из цепочки создается новая цепочка.</span><span class="sxs-lookup"><span data-stu-id="6880a-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="6880a-109">Методы</span><span class="sxs-lookup"><span data-stu-id="6880a-109">Methods</span></span>

| <span data-ttu-id="6880a-110">Метод</span><span class="sxs-lookup"><span data-stu-id="6880a-110">Method</span></span>       | <span data-ttu-id="6880a-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6880a-111">Return Type</span></span>  |<span data-ttu-id="6880a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6880a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6880a-113">Перечисление цепочек</span><span class="sxs-lookup"><span data-stu-id="6880a-113">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="6880a-114">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="6880a-114">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="6880a-115">Получение всех цепочек группы.</span><span class="sxs-lookup"><span data-stu-id="6880a-115">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="6880a-116">Создание цепочки</span><span class="sxs-lookup"><span data-stu-id="6880a-116">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="6880a-117">conversationThread</span><span class="sxs-lookup"><span data-stu-id="6880a-117">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="6880a-p102">Создание беседы путем создания цепочки. В группе создаются беседа, цепочка беседы и запись.</span><span class="sxs-lookup"><span data-stu-id="6880a-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="6880a-120">Получение conversationThread</span><span class="sxs-lookup"><span data-stu-id="6880a-120">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="6880a-121">conversationThread</span><span class="sxs-lookup"><span data-stu-id="6880a-121">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="6880a-122">Получение определенной цепочки, принадлежащей группе.</span><span class="sxs-lookup"><span data-stu-id="6880a-122">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="6880a-123">Обновление</span><span class="sxs-lookup"><span data-stu-id="6880a-123">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="6880a-124">conversationThread</span><span class="sxs-lookup"><span data-stu-id="6880a-124">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="6880a-125">Обновление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="6880a-125">Update conversationThread object.</span></span> |
|<span data-ttu-id="6880a-126">[удаление](../api/conversationthread-delete.md);</span><span class="sxs-lookup"><span data-stu-id="6880a-126">[Delete](../api/conversationthread-delete.md)</span></span> | <span data-ttu-id="6880a-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="6880a-127">None</span></span> |<span data-ttu-id="6880a-128">Удаление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="6880a-128">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="6880a-129">reply</span><span class="sxs-lookup"><span data-stu-id="6880a-129">reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="6880a-130">Нет</span><span class="sxs-lookup"><span data-stu-id="6880a-130">None</span></span>|<span data-ttu-id="6880a-131">Создание ответа для этой цепочки с помощью создания сущности Post.</span><span class="sxs-lookup"><span data-stu-id="6880a-131">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="6880a-132">Список сущностей Post</span><span class="sxs-lookup"><span data-stu-id="6880a-132">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="6880a-133">Коллекция [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="6880a-133">[post](post.md) collection</span></span>| <span data-ttu-id="6880a-134">Получение записей для указанной цепочки.</span><span class="sxs-lookup"><span data-stu-id="6880a-134">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="6880a-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="6880a-135">Properties</span></span>
| <span data-ttu-id="6880a-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="6880a-136">Property</span></span>     | <span data-ttu-id="6880a-137">Тип</span><span class="sxs-lookup"><span data-stu-id="6880a-137">Type</span></span>   |<span data-ttu-id="6880a-138">Описание</span><span class="sxs-lookup"><span data-stu-id="6880a-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6880a-139">id</span><span class="sxs-lookup"><span data-stu-id="6880a-139">id</span></span>|<span data-ttu-id="6880a-140">String</span><span class="sxs-lookup"><span data-stu-id="6880a-140">String</span></span>| <span data-ttu-id="6880a-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6880a-141">Read-only.</span></span>|
|<span data-ttu-id="6880a-142">toRecipients</span><span class="sxs-lookup"><span data-stu-id="6880a-142">toRecipients</span></span>|<span data-ttu-id="6880a-143">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="6880a-143">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="6880a-144">Получатели в поле "Кому" для цепочки.</span><span class="sxs-lookup"><span data-stu-id="6880a-144">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="6880a-145">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="6880a-145">ccRecipients</span></span>|<span data-ttu-id="6880a-146">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="6880a-146">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="6880a-147">Получатели в поле "Копия" для цепочки.</span><span class="sxs-lookup"><span data-stu-id="6880a-147">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="6880a-148">topic</span><span class="sxs-lookup"><span data-stu-id="6880a-148">topic</span></span>|<span data-ttu-id="6880a-149">String</span><span class="sxs-lookup"><span data-stu-id="6880a-149">String</span></span>|<span data-ttu-id="6880a-p103">Тема беседы. Это свойство можно задать при создании беседы, но его невозможно обновить.</span><span class="sxs-lookup"><span data-stu-id="6880a-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="6880a-152">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="6880a-152">hasAttachments</span></span>|<span data-ttu-id="6880a-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="6880a-153">Boolean</span></span>|<span data-ttu-id="6880a-154">Указывает, содержит ли какая-либо запись в этой цепочке хотя бы одно вложение.</span><span class="sxs-lookup"><span data-stu-id="6880a-154">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="6880a-155">ластделивереддатетиме</span><span class="sxs-lookup"><span data-stu-id="6880a-155">lastDeliveredDateTime</span></span>|<span data-ttu-id="6880a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6880a-156">DateTimeOffset</span></span>|<span data-ttu-id="6880a-p104">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6880a-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6880a-159">уникуесендерс</span><span class="sxs-lookup"><span data-stu-id="6880a-159">uniqueSenders</span></span>|<span data-ttu-id="6880a-160">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6880a-160">String collection</span></span>|<span data-ttu-id="6880a-161">Все пользователи, которые отправили сообщение в эту цепочку.</span><span class="sxs-lookup"><span data-stu-id="6880a-161">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="6880a-162">preview</span><span class="sxs-lookup"><span data-stu-id="6880a-162">preview</span></span>|<span data-ttu-id="6880a-163">String</span><span class="sxs-lookup"><span data-stu-id="6880a-163">String</span></span>|<span data-ttu-id="6880a-164">Краткая сводка из текста последней записи в этой беседе.</span><span class="sxs-lookup"><span data-stu-id="6880a-164">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="6880a-165">isLocked</span><span class="sxs-lookup"><span data-stu-id="6880a-165">isLocked</span></span>|<span data-ttu-id="6880a-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="6880a-166">Boolean</span></span>|<span data-ttu-id="6880a-167">Указывает, заблокирована ли цепочка.</span><span class="sxs-lookup"><span data-stu-id="6880a-167">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6880a-168">Связи</span><span class="sxs-lookup"><span data-stu-id="6880a-168">Relationships</span></span>
| <span data-ttu-id="6880a-169">Связь</span><span class="sxs-lookup"><span data-stu-id="6880a-169">Relationship</span></span> | <span data-ttu-id="6880a-170">Тип</span><span class="sxs-lookup"><span data-stu-id="6880a-170">Type</span></span>   |<span data-ttu-id="6880a-171">Описание</span><span class="sxs-lookup"><span data-stu-id="6880a-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6880a-172">posts</span><span class="sxs-lookup"><span data-stu-id="6880a-172">posts</span></span>|<span data-ttu-id="6880a-173">Коллекция [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="6880a-173">[post](post.md) collection</span></span>| <span data-ttu-id="6880a-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6880a-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6880a-176">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6880a-176">JSON representation</span></span>

<span data-ttu-id="6880a-177">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6880a-177">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
