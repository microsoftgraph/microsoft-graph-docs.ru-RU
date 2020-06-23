---
title: Тип ресурса conversationThread
description: conversationThread — это коллекция экземпляров post.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: d1b274aa84299ae66d6385133ed7371a377d01e6
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845941"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="a4678-103">Тип ресурса conversationThread</span><span class="sxs-lookup"><span data-stu-id="a4678-103">conversationThread resource type</span></span>

<span data-ttu-id="a4678-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4678-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4678-105">conversationThread — это коллекция экземпляров [post](post.md).</span><span class="sxs-lookup"><span data-stu-id="a4678-105">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="a4678-106">The last post's recipients collection is the aggregated recipients of the entire thread.</span><span class="sxs-lookup"><span data-stu-id="a4678-106">The last post's recipients collection is the aggregated recipients of the entire thread.</span></span> <span data-ttu-id="a4678-107">A thread can have a growing collection of recipients.</span><span class="sxs-lookup"><span data-stu-id="a4678-107">A thread can have a growing collection of recipients.</span></span>
<span data-ttu-id="a4678-108">A new thread is created when a recipient is removed from the thread.</span><span class="sxs-lookup"><span data-stu-id="a4678-108">A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="a4678-109">Методы</span><span class="sxs-lookup"><span data-stu-id="a4678-109">Methods</span></span>

| <span data-ttu-id="a4678-110">Метод</span><span class="sxs-lookup"><span data-stu-id="a4678-110">Method</span></span>       | <span data-ttu-id="a4678-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a4678-111">Return Type</span></span>  |<span data-ttu-id="a4678-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a4678-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a4678-113">Перечисление цепочек</span><span class="sxs-lookup"><span data-stu-id="a4678-113">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="a4678-114">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="a4678-114">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="a4678-115">Получение всех цепочек группы.</span><span class="sxs-lookup"><span data-stu-id="a4678-115">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="a4678-116">Создание цепочки</span><span class="sxs-lookup"><span data-stu-id="a4678-116">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="a4678-117">conversationThread</span><span class="sxs-lookup"><span data-stu-id="a4678-117">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="a4678-118">Start a new conversation by first creating a thread.</span><span class="sxs-lookup"><span data-stu-id="a4678-118">Start a new conversation by first creating a thread.</span></span> <span data-ttu-id="a4678-119">A new conversation, conversation thread, and post are created in the group.</span><span class="sxs-lookup"><span data-stu-id="a4678-119">A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="a4678-120">Получение conversationThread</span><span class="sxs-lookup"><span data-stu-id="a4678-120">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="a4678-121">conversationThread</span><span class="sxs-lookup"><span data-stu-id="a4678-121">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="a4678-122">Получение определенной цепочки, принадлежащей группе.</span><span class="sxs-lookup"><span data-stu-id="a4678-122">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="a4678-123">Обновление</span><span class="sxs-lookup"><span data-stu-id="a4678-123">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="a4678-124">conversationThread</span><span class="sxs-lookup"><span data-stu-id="a4678-124">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="a4678-125">Обновление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="a4678-125">Update conversationThread object.</span></span> |
|[<span data-ttu-id="a4678-126">Удаление</span><span class="sxs-lookup"><span data-stu-id="a4678-126">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="a4678-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="a4678-127">None</span></span> |<span data-ttu-id="a4678-128">Удаление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="a4678-128">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="a4678-129">reply</span><span class="sxs-lookup"><span data-stu-id="a4678-129">reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="a4678-130">Нет</span><span class="sxs-lookup"><span data-stu-id="a4678-130">None</span></span>|<span data-ttu-id="a4678-131">Создание ответа для этой цепочки с помощью создания сущности Post.</span><span class="sxs-lookup"><span data-stu-id="a4678-131">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="a4678-132">Список сущностей Post</span><span class="sxs-lookup"><span data-stu-id="a4678-132">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="a4678-133">Коллекция [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="a4678-133">[post](post.md) collection</span></span>| <span data-ttu-id="a4678-134">Получение записей для указанной цепочки.</span><span class="sxs-lookup"><span data-stu-id="a4678-134">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="a4678-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4678-135">Properties</span></span>
| <span data-ttu-id="a4678-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4678-136">Property</span></span>              | <span data-ttu-id="a4678-137">Тип</span><span class="sxs-lookup"><span data-stu-id="a4678-137">Type</span></span>                                 | <span data-ttu-id="a4678-138">Описание</span><span class="sxs-lookup"><span data-stu-id="a4678-138">Description</span></span>                                                                                                                                                                                      |
|:----------------------|:-------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a4678-139">id</span><span class="sxs-lookup"><span data-stu-id="a4678-139">id</span></span>                    | <span data-ttu-id="a4678-140">String</span><span class="sxs-lookup"><span data-stu-id="a4678-140">String</span></span>                               | <span data-ttu-id="a4678-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4678-141">Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="a4678-142">toRecipients</span><span class="sxs-lookup"><span data-stu-id="a4678-142">toRecipients</span></span>          | <span data-ttu-id="a4678-143">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="a4678-143">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="a4678-144">Получатели в поле "Кому" для цепочки.</span><span class="sxs-lookup"><span data-stu-id="a4678-144">The To: recipients for the thread.</span></span>                                                                                                                                                               |
| <span data-ttu-id="a4678-145">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="a4678-145">ccRecipients</span></span>          | <span data-ttu-id="a4678-146">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="a4678-146">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="a4678-147">Получатели в поле "Копия" для цепочки.</span><span class="sxs-lookup"><span data-stu-id="a4678-147">The Cc: recipients for the thread.</span></span>                                                                                                                                                               |
| <span data-ttu-id="a4678-148">topic</span><span class="sxs-lookup"><span data-stu-id="a4678-148">topic</span></span>                 | <span data-ttu-id="a4678-149">String</span><span class="sxs-lookup"><span data-stu-id="a4678-149">String</span></span>                               | <span data-ttu-id="a4678-150">The topic of the conversation.</span><span class="sxs-lookup"><span data-stu-id="a4678-150">The topic of the conversation.</span></span> <span data-ttu-id="a4678-151">This property can be set when the conversation is created, but it cannot be updated.</span><span class="sxs-lookup"><span data-stu-id="a4678-151">This property can be set when the conversation is created, but it cannot be updated.</span></span>                                                                              |
| <span data-ttu-id="a4678-152">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="a4678-152">hasAttachments</span></span>        | <span data-ttu-id="a4678-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4678-153">Boolean</span></span>                              | <span data-ttu-id="a4678-154">Указывает, содержит ли какая-либо запись в этой цепочке хотя бы одно вложение.</span><span class="sxs-lookup"><span data-stu-id="a4678-154">Indicates whether any of the posts within this thread has at least one attachment.</span></span>                                                                                                               |
| <span data-ttu-id="a4678-155">ластделивереддатетиме</span><span class="sxs-lookup"><span data-stu-id="a4678-155">lastDeliveredDateTime</span></span> | <span data-ttu-id="a4678-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4678-156">DateTimeOffset</span></span>                       | <span data-ttu-id="a4678-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span><span class="sxs-lookup"><span data-stu-id="a4678-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a4678-158">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a4678-158">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="a4678-159">уникуесендерс</span><span class="sxs-lookup"><span data-stu-id="a4678-159">uniqueSenders</span></span>         | <span data-ttu-id="a4678-160">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a4678-160">String collection</span></span>                    | <span data-ttu-id="a4678-161">Все пользователи, которые отправили сообщение в эту цепочку.</span><span class="sxs-lookup"><span data-stu-id="a4678-161">All the users that sent a message to this thread.</span></span>                                                                                                                                                |
| <span data-ttu-id="a4678-162">preview</span><span class="sxs-lookup"><span data-stu-id="a4678-162">preview</span></span>               | <span data-ttu-id="a4678-163">String</span><span class="sxs-lookup"><span data-stu-id="a4678-163">String</span></span>                               | <span data-ttu-id="a4678-164">Краткая сводка из тела последней публикации в этой беседе.</span><span class="sxs-lookup"><span data-stu-id="a4678-164">A short summary from the body of the latest post in this conversation.</span></span>                                                                                                                           |
| <span data-ttu-id="a4678-165">isLocked</span><span class="sxs-lookup"><span data-stu-id="a4678-165">isLocked</span></span>              | <span data-ttu-id="a4678-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4678-166">Boolean</span></span>                              | <span data-ttu-id="a4678-167">Указывает, заблокирована ли цепочка.</span><span class="sxs-lookup"><span data-stu-id="a4678-167">Indicates if the thread is locked.</span></span>                                                                                                                                                               |

## <a name="relationships"></a><span data-ttu-id="a4678-168">Отношения</span><span class="sxs-lookup"><span data-stu-id="a4678-168">Relationships</span></span>
| <span data-ttu-id="a4678-169">Связь</span><span class="sxs-lookup"><span data-stu-id="a4678-169">Relationship</span></span> | <span data-ttu-id="a4678-170">Тип</span><span class="sxs-lookup"><span data-stu-id="a4678-170">Type</span></span>   |<span data-ttu-id="a4678-171">Описание</span><span class="sxs-lookup"><span data-stu-id="a4678-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4678-172">posts</span><span class="sxs-lookup"><span data-stu-id="a4678-172">posts</span></span>|<span data-ttu-id="a4678-173">Коллекция [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="a4678-173">[post](post.md) collection</span></span>| <span data-ttu-id="a4678-174">Read-only.</span><span class="sxs-lookup"><span data-stu-id="a4678-174">Read-only.</span></span> <span data-ttu-id="a4678-175">Nullable.</span><span class="sxs-lookup"><span data-stu-id="a4678-175">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4678-176">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4678-176">JSON representation</span></span>

<span data-ttu-id="a4678-177">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4678-177">Here is a JSON representation of the resource</span></span>

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
