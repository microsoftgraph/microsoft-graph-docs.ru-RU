---
title: Тип ресурса conversationThread
description: conversationThread — это коллекция экземпляров post.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: a8ac7efb08e498b45247119e995aae4c5b1fcb8e
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2020
ms.locfileid: "43511045"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="57af7-103">Тип ресурса conversationThread</span><span class="sxs-lookup"><span data-stu-id="57af7-103">conversationThread resource type</span></span>

<span data-ttu-id="57af7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57af7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="57af7-105">conversationThread — это коллекция экземпляров [post](post.md).</span><span class="sxs-lookup"><span data-stu-id="57af7-105">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="57af7-p101">Коллекция получателей последней записи — это все получатели для цепочки. Коллекция получателей для цепочки может увеличиваться. При удалении получателя из цепочки создается новая цепочка.</span><span class="sxs-lookup"><span data-stu-id="57af7-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="57af7-109">Методы</span><span class="sxs-lookup"><span data-stu-id="57af7-109">Methods</span></span>

| <span data-ttu-id="57af7-110">Метод</span><span class="sxs-lookup"><span data-stu-id="57af7-110">Method</span></span>       | <span data-ttu-id="57af7-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="57af7-111">Return Type</span></span>  |<span data-ttu-id="57af7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="57af7-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="57af7-113">Перечисление цепочек</span><span class="sxs-lookup"><span data-stu-id="57af7-113">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="57af7-114">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="57af7-114">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="57af7-115">Получение всех цепочек группы.</span><span class="sxs-lookup"><span data-stu-id="57af7-115">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="57af7-116">Создание цепочки</span><span class="sxs-lookup"><span data-stu-id="57af7-116">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="57af7-117">conversationThread</span><span class="sxs-lookup"><span data-stu-id="57af7-117">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="57af7-p102">Создание беседы путем создания цепочки. В группе создаются беседа, цепочка беседы и запись.</span><span class="sxs-lookup"><span data-stu-id="57af7-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="57af7-120">Получение conversationThread</span><span class="sxs-lookup"><span data-stu-id="57af7-120">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="57af7-121">conversationThread</span><span class="sxs-lookup"><span data-stu-id="57af7-121">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="57af7-122">Получение определенной цепочки, принадлежащей группе.</span><span class="sxs-lookup"><span data-stu-id="57af7-122">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="57af7-123">Обновление</span><span class="sxs-lookup"><span data-stu-id="57af7-123">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="57af7-124">conversationThread</span><span class="sxs-lookup"><span data-stu-id="57af7-124">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="57af7-125">Обновление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="57af7-125">Update conversationThread object.</span></span> |
|<span data-ttu-id="57af7-126">[удаление](../api/conversationthread-delete.md);</span><span class="sxs-lookup"><span data-stu-id="57af7-126">[Delete](../api/conversationthread-delete.md)</span></span> | <span data-ttu-id="57af7-127">Нет</span><span class="sxs-lookup"><span data-stu-id="57af7-127">None</span></span> |<span data-ttu-id="57af7-128">Удаление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="57af7-128">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="57af7-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="57af7-129">Reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="57af7-130">Нет</span><span class="sxs-lookup"><span data-stu-id="57af7-130">None</span></span>|<span data-ttu-id="57af7-131">Создание ответа для этой цепочки с помощью создания сущности Post.</span><span class="sxs-lookup"><span data-stu-id="57af7-131">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="57af7-132">Список сущностей Post</span><span class="sxs-lookup"><span data-stu-id="57af7-132">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="57af7-133">Коллекция [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="57af7-133">[post](post.md) collection</span></span>| <span data-ttu-id="57af7-134">Получение записей для указанной цепочки.</span><span class="sxs-lookup"><span data-stu-id="57af7-134">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="57af7-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="57af7-135">Properties</span></span>
| <span data-ttu-id="57af7-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="57af7-136">Property</span></span>     | <span data-ttu-id="57af7-137">Тип</span><span class="sxs-lookup"><span data-stu-id="57af7-137">Type</span></span>   |<span data-ttu-id="57af7-138">Описание</span><span class="sxs-lookup"><span data-stu-id="57af7-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57af7-139">id</span><span class="sxs-lookup"><span data-stu-id="57af7-139">id</span></span>|<span data-ttu-id="57af7-140">String</span><span class="sxs-lookup"><span data-stu-id="57af7-140">String</span></span>| <span data-ttu-id="57af7-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57af7-141">Read-only.</span></span>|
|<span data-ttu-id="57af7-142">toRecipients</span><span class="sxs-lookup"><span data-stu-id="57af7-142">toRecipients</span></span>|<span data-ttu-id="57af7-143">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="57af7-143">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="57af7-144">Получатели в поле "Кому" для цепочки.</span><span class="sxs-lookup"><span data-stu-id="57af7-144">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="57af7-145">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="57af7-145">ccRecipients</span></span>|<span data-ttu-id="57af7-146">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="57af7-146">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="57af7-147">Получатели в поле "Копия" для цепочки.</span><span class="sxs-lookup"><span data-stu-id="57af7-147">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="57af7-148">topic</span><span class="sxs-lookup"><span data-stu-id="57af7-148">topic</span></span>|<span data-ttu-id="57af7-149">String</span><span class="sxs-lookup"><span data-stu-id="57af7-149">String</span></span>|<span data-ttu-id="57af7-p103">Тема беседы. Это свойство можно задать при создании беседы, но его невозможно обновить.</span><span class="sxs-lookup"><span data-stu-id="57af7-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="57af7-152">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="57af7-152">hasAttachments</span></span>|<span data-ttu-id="57af7-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="57af7-153">Boolean</span></span>|<span data-ttu-id="57af7-154">Указывает, содержит ли какая-либо запись в этой цепочке хотя бы одно вложение.</span><span class="sxs-lookup"><span data-stu-id="57af7-154">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="57af7-155">ластделивереддатетиме</span><span class="sxs-lookup"><span data-stu-id="57af7-155">lastDeliveredDateTime</span></span>|<span data-ttu-id="57af7-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57af7-156">DateTimeOffset</span></span>|<span data-ttu-id="57af7-p104">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="57af7-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="57af7-159">уникуесендерс</span><span class="sxs-lookup"><span data-stu-id="57af7-159">uniqueSenders</span></span>|<span data-ttu-id="57af7-160">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="57af7-160">String collection</span></span>|<span data-ttu-id="57af7-161">Все пользователи, которые отправили сообщение в эту цепочку.</span><span class="sxs-lookup"><span data-stu-id="57af7-161">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="57af7-162">preview</span><span class="sxs-lookup"><span data-stu-id="57af7-162">preview</span></span>|<span data-ttu-id="57af7-163">String</span><span class="sxs-lookup"><span data-stu-id="57af7-163">String</span></span>|<span data-ttu-id="57af7-164">Краткая сводка из текста последней записи в этой беседе.</span><span class="sxs-lookup"><span data-stu-id="57af7-164">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="57af7-165">isLocked</span><span class="sxs-lookup"><span data-stu-id="57af7-165">isLocked</span></span>|<span data-ttu-id="57af7-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="57af7-166">Boolean</span></span>|<span data-ttu-id="57af7-167">Указывает, заблокирована ли цепочка.</span><span class="sxs-lookup"><span data-stu-id="57af7-167">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57af7-168">Связи</span><span class="sxs-lookup"><span data-stu-id="57af7-168">Relationships</span></span>
| <span data-ttu-id="57af7-169">Связь</span><span class="sxs-lookup"><span data-stu-id="57af7-169">Relationship</span></span> | <span data-ttu-id="57af7-170">Тип</span><span class="sxs-lookup"><span data-stu-id="57af7-170">Type</span></span>   |<span data-ttu-id="57af7-171">Описание</span><span class="sxs-lookup"><span data-stu-id="57af7-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57af7-172">posts</span><span class="sxs-lookup"><span data-stu-id="57af7-172">posts</span></span>|<span data-ttu-id="57af7-173">Коллекция [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="57af7-173">[post](post.md) collection</span></span>| <span data-ttu-id="57af7-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="57af7-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57af7-176">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57af7-176">JSON representation</span></span>

<span data-ttu-id="57af7-177">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57af7-177">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversationThread",
  "@odata.annotations": [
    {
      "property": "posts",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
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
