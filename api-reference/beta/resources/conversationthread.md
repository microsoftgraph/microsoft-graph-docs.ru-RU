---
title: Тип ресурса conversationThread
description: conversationThread — это коллекция экземпляров post.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: a44234c2ec82b0b28df6c9bbf57b8d8069f129f8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973951"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="956cb-103">Тип ресурса conversationThread</span><span class="sxs-lookup"><span data-stu-id="956cb-103">conversationThread resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="956cb-104">conversationThread — это коллекция экземпляров [post](post.md).</span><span class="sxs-lookup"><span data-stu-id="956cb-104">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="956cb-p101">Коллекция получателей последней записи — это все получатели для цепочки. Коллекция получателей для цепочки может увеличиваться. При удалении получателя из цепочки создается новая цепочка.</span><span class="sxs-lookup"><span data-stu-id="956cb-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="956cb-108">Методы</span><span class="sxs-lookup"><span data-stu-id="956cb-108">Methods</span></span>

| <span data-ttu-id="956cb-109">Метод</span><span class="sxs-lookup"><span data-stu-id="956cb-109">Method</span></span>       | <span data-ttu-id="956cb-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="956cb-110">Return Type</span></span>  |<span data-ttu-id="956cb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="956cb-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="956cb-112">Перечисление цепочек</span><span class="sxs-lookup"><span data-stu-id="956cb-112">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="956cb-113">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="956cb-113">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="956cb-114">Получение всех цепочек группы.</span><span class="sxs-lookup"><span data-stu-id="956cb-114">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="956cb-115">Создание цепочки</span><span class="sxs-lookup"><span data-stu-id="956cb-115">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="956cb-116">conversationThread</span><span class="sxs-lookup"><span data-stu-id="956cb-116">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="956cb-p102">Создание беседы путем создания цепочки. В группе создаются беседа, цепочка беседы и запись.</span><span class="sxs-lookup"><span data-stu-id="956cb-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="956cb-119">Получение conversationThread</span><span class="sxs-lookup"><span data-stu-id="956cb-119">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="956cb-120">conversationThread</span><span class="sxs-lookup"><span data-stu-id="956cb-120">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="956cb-121">Получение определенной цепочки, принадлежащей группе.</span><span class="sxs-lookup"><span data-stu-id="956cb-121">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="956cb-122">Обновление</span><span class="sxs-lookup"><span data-stu-id="956cb-122">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="956cb-123">conversationThread</span><span class="sxs-lookup"><span data-stu-id="956cb-123">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="956cb-124">Обновление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="956cb-124">Update conversationThread object.</span></span> |
|[<span data-ttu-id="956cb-125">Удаление</span><span class="sxs-lookup"><span data-stu-id="956cb-125">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="956cb-126">Нет.</span><span class="sxs-lookup"><span data-stu-id="956cb-126">None</span></span> |<span data-ttu-id="956cb-127">Удаление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="956cb-127">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="956cb-128">reply</span><span class="sxs-lookup"><span data-stu-id="956cb-128">reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="956cb-129">Нет</span><span class="sxs-lookup"><span data-stu-id="956cb-129">None</span></span>|<span data-ttu-id="956cb-130">Создание ответа для этой цепочки с помощью создания сущности Post.</span><span class="sxs-lookup"><span data-stu-id="956cb-130">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="956cb-131">Список сущностей Post</span><span class="sxs-lookup"><span data-stu-id="956cb-131">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="956cb-132">Коллекция [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="956cb-132">[post](post.md) collection</span></span>| <span data-ttu-id="956cb-133">Получение записей для указанной цепочки.</span><span class="sxs-lookup"><span data-stu-id="956cb-133">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="956cb-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="956cb-134">Properties</span></span>
| <span data-ttu-id="956cb-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="956cb-135">Property</span></span>     | <span data-ttu-id="956cb-136">Тип</span><span class="sxs-lookup"><span data-stu-id="956cb-136">Type</span></span>   |<span data-ttu-id="956cb-137">Описание</span><span class="sxs-lookup"><span data-stu-id="956cb-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="956cb-138">id</span><span class="sxs-lookup"><span data-stu-id="956cb-138">id</span></span>|<span data-ttu-id="956cb-139">String</span><span class="sxs-lookup"><span data-stu-id="956cb-139">String</span></span>| <span data-ttu-id="956cb-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="956cb-140">Read-only.</span></span>|
|<span data-ttu-id="956cb-141">toRecipients</span><span class="sxs-lookup"><span data-stu-id="956cb-141">toRecipients</span></span>|<span data-ttu-id="956cb-142">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="956cb-142">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="956cb-143">Получатели в поле "Кому" для цепочки.</span><span class="sxs-lookup"><span data-stu-id="956cb-143">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="956cb-144">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="956cb-144">ccRecipients</span></span>|<span data-ttu-id="956cb-145">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="956cb-145">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="956cb-146">Получатели в поле "Копия" для цепочки.</span><span class="sxs-lookup"><span data-stu-id="956cb-146">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="956cb-147">topic</span><span class="sxs-lookup"><span data-stu-id="956cb-147">topic</span></span>|<span data-ttu-id="956cb-148">String</span><span class="sxs-lookup"><span data-stu-id="956cb-148">String</span></span>|<span data-ttu-id="956cb-p103">Тема беседы. Это свойство можно задать при создании беседы, но его невозможно обновить.</span><span class="sxs-lookup"><span data-stu-id="956cb-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="956cb-151">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="956cb-151">hasAttachments</span></span>|<span data-ttu-id="956cb-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="956cb-152">Boolean</span></span>|<span data-ttu-id="956cb-153">Указывает, содержит ли какая-либо запись в этой цепочке хотя бы одно вложение.</span><span class="sxs-lookup"><span data-stu-id="956cb-153">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="956cb-154">Ластделивереддатетиме</span><span class="sxs-lookup"><span data-stu-id="956cb-154">lastDeliveredDateTime</span></span>|<span data-ttu-id="956cb-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="956cb-155">DateTimeOffset</span></span>|<span data-ttu-id="956cb-p104">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="956cb-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="956cb-158">Уникуесендерс</span><span class="sxs-lookup"><span data-stu-id="956cb-158">uniqueSenders</span></span>|<span data-ttu-id="956cb-159">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="956cb-159">String collection</span></span>|<span data-ttu-id="956cb-160">Все пользователи, которые отправили сообщение в эту цепочку.</span><span class="sxs-lookup"><span data-stu-id="956cb-160">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="956cb-161">preview</span><span class="sxs-lookup"><span data-stu-id="956cb-161">preview</span></span>|<span data-ttu-id="956cb-162">String</span><span class="sxs-lookup"><span data-stu-id="956cb-162">String</span></span>|<span data-ttu-id="956cb-163">Краткая сводка из текста последней записи в этой беседе.</span><span class="sxs-lookup"><span data-stu-id="956cb-163">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="956cb-164">isLocked</span><span class="sxs-lookup"><span data-stu-id="956cb-164">isLocked</span></span>|<span data-ttu-id="956cb-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="956cb-165">Boolean</span></span>|<span data-ttu-id="956cb-166">Указывает, заблокирована ли цепочка.</span><span class="sxs-lookup"><span data-stu-id="956cb-166">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="956cb-167">Отношения</span><span class="sxs-lookup"><span data-stu-id="956cb-167">Relationships</span></span>
| <span data-ttu-id="956cb-168">Отношение</span><span class="sxs-lookup"><span data-stu-id="956cb-168">Relationship</span></span> | <span data-ttu-id="956cb-169">Тип</span><span class="sxs-lookup"><span data-stu-id="956cb-169">Type</span></span>   |<span data-ttu-id="956cb-170">Описание</span><span class="sxs-lookup"><span data-stu-id="956cb-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="956cb-171">posts</span><span class="sxs-lookup"><span data-stu-id="956cb-171">posts</span></span>|<span data-ttu-id="956cb-172">Коллекция [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="956cb-172">[post](post.md) collection</span></span>| <span data-ttu-id="956cb-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="956cb-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="956cb-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="956cb-175">JSON representation</span></span>

<span data-ttu-id="956cb-176">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="956cb-176">Here is a JSON representation of the resource</span></span>

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
