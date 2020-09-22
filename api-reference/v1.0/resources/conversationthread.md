---
title: Тип ресурса conversationThread
description: conversationThread — это коллекция экземпляров post.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 981ff7ce5effe9faa2518d58b72de8d395d4cfd5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018853"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="f521e-103">Тип ресурса conversationThread</span><span class="sxs-lookup"><span data-stu-id="f521e-103">conversationThread resource type</span></span>

<span data-ttu-id="f521e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f521e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f521e-105">conversationThread — это коллекция экземпляров [post](post.md).</span><span class="sxs-lookup"><span data-stu-id="f521e-105">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="f521e-p101">Коллекция получателей последней записи — это все получатели для цепочки. Коллекция получателей для цепочки может увеличиваться. При удалении получателя из цепочки создается новая цепочка.</span><span class="sxs-lookup"><span data-stu-id="f521e-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="f521e-109">Методы</span><span class="sxs-lookup"><span data-stu-id="f521e-109">Methods</span></span>

| <span data-ttu-id="f521e-110">Метод</span><span class="sxs-lookup"><span data-stu-id="f521e-110">Method</span></span>       | <span data-ttu-id="f521e-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f521e-111">Return Type</span></span>  |<span data-ttu-id="f521e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f521e-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f521e-113">Перечисление цепочек</span><span class="sxs-lookup"><span data-stu-id="f521e-113">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="f521e-114">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="f521e-114">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="f521e-115">Получение всех цепочек группы.</span><span class="sxs-lookup"><span data-stu-id="f521e-115">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="f521e-116">Создание цепочки</span><span class="sxs-lookup"><span data-stu-id="f521e-116">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="f521e-117">conversationThread</span><span class="sxs-lookup"><span data-stu-id="f521e-117">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="f521e-p102">Создание беседы путем создания цепочки. В группе создаются беседа, цепочка беседы и запись.</span><span class="sxs-lookup"><span data-stu-id="f521e-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="f521e-120">Получение conversationThread</span><span class="sxs-lookup"><span data-stu-id="f521e-120">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="f521e-121">conversationThread</span><span class="sxs-lookup"><span data-stu-id="f521e-121">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="f521e-122">Получение определенной цепочки, принадлежащей группе.</span><span class="sxs-lookup"><span data-stu-id="f521e-122">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="f521e-123">Обновление</span><span class="sxs-lookup"><span data-stu-id="f521e-123">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="f521e-124">conversationThread</span><span class="sxs-lookup"><span data-stu-id="f521e-124">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="f521e-125">Обновление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="f521e-125">Update conversationThread object.</span></span> |
|<span data-ttu-id="f521e-126">[удаление](../api/conversationthread-delete.md);</span><span class="sxs-lookup"><span data-stu-id="f521e-126">[Delete](../api/conversationthread-delete.md)</span></span> | <span data-ttu-id="f521e-127">Нет</span><span class="sxs-lookup"><span data-stu-id="f521e-127">None</span></span> |<span data-ttu-id="f521e-128">Удаление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="f521e-128">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="f521e-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f521e-129">Reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="f521e-130">Нет</span><span class="sxs-lookup"><span data-stu-id="f521e-130">None</span></span>|<span data-ttu-id="f521e-131">Создание ответа для этой цепочки с помощью создания сущности Post.</span><span class="sxs-lookup"><span data-stu-id="f521e-131">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="f521e-132">Список сущностей Post</span><span class="sxs-lookup"><span data-stu-id="f521e-132">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="f521e-133">Коллекция [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="f521e-133">[post](post.md) collection</span></span>| <span data-ttu-id="f521e-134">Получение записей для указанной цепочки.</span><span class="sxs-lookup"><span data-stu-id="f521e-134">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="f521e-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="f521e-135">Properties</span></span>
| <span data-ttu-id="f521e-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="f521e-136">Property</span></span>              | <span data-ttu-id="f521e-137">Тип</span><span class="sxs-lookup"><span data-stu-id="f521e-137">Type</span></span>                                 | <span data-ttu-id="f521e-138">Описание</span><span class="sxs-lookup"><span data-stu-id="f521e-138">Description</span></span>                                                                                                                                                                                      |
|:----------------------|:-------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f521e-139">id</span><span class="sxs-lookup"><span data-stu-id="f521e-139">id</span></span>                    | <span data-ttu-id="f521e-140">String</span><span class="sxs-lookup"><span data-stu-id="f521e-140">String</span></span>                               | <span data-ttu-id="f521e-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f521e-141">Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="f521e-142">toRecipients</span><span class="sxs-lookup"><span data-stu-id="f521e-142">toRecipients</span></span>          | <span data-ttu-id="f521e-143">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="f521e-143">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="f521e-144">Получатели в поле "Кому" для цепочки.</span><span class="sxs-lookup"><span data-stu-id="f521e-144">The To: recipients for the thread.</span></span>                                                                                                                                                               |
| <span data-ttu-id="f521e-145">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="f521e-145">ccRecipients</span></span>          | <span data-ttu-id="f521e-146">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="f521e-146">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="f521e-147">Получатели в поле "Копия" для цепочки.</span><span class="sxs-lookup"><span data-stu-id="f521e-147">The Cc: recipients for the thread.</span></span>                                                                                                                                                               |
| <span data-ttu-id="f521e-148">topic</span><span class="sxs-lookup"><span data-stu-id="f521e-148">topic</span></span>                 | <span data-ttu-id="f521e-149">String</span><span class="sxs-lookup"><span data-stu-id="f521e-149">String</span></span>                               | <span data-ttu-id="f521e-p103">Тема беседы. Это свойство можно задать при создании беседы, но его невозможно обновить.</span><span class="sxs-lookup"><span data-stu-id="f521e-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>                                                                              |
| <span data-ttu-id="f521e-152">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="f521e-152">hasAttachments</span></span>        | <span data-ttu-id="f521e-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="f521e-153">Boolean</span></span>                              | <span data-ttu-id="f521e-154">Указывает, содержит ли какая-либо запись в этой цепочке хотя бы одно вложение.</span><span class="sxs-lookup"><span data-stu-id="f521e-154">Indicates whether any of the posts within this thread has at least one attachment.</span></span>                                                                                                               |
| <span data-ttu-id="f521e-155">ластделивереддатетиме</span><span class="sxs-lookup"><span data-stu-id="f521e-155">lastDeliveredDateTime</span></span> | <span data-ttu-id="f521e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f521e-156">DateTimeOffset</span></span>                       | <span data-ttu-id="f521e-p104">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f521e-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="f521e-159">уникуесендерс</span><span class="sxs-lookup"><span data-stu-id="f521e-159">uniqueSenders</span></span>         | <span data-ttu-id="f521e-160">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f521e-160">String collection</span></span>                    | <span data-ttu-id="f521e-161">Все пользователи, которые отправили сообщение в эту цепочку.</span><span class="sxs-lookup"><span data-stu-id="f521e-161">All the users that sent a message to this thread.</span></span>                                                                                                                                                |
| <span data-ttu-id="f521e-162">preview</span><span class="sxs-lookup"><span data-stu-id="f521e-162">preview</span></span>               | <span data-ttu-id="f521e-163">String</span><span class="sxs-lookup"><span data-stu-id="f521e-163">String</span></span>                               | <span data-ttu-id="f521e-164">Краткая сводка из тела последней публикации в этой беседе.</span><span class="sxs-lookup"><span data-stu-id="f521e-164">A short summary from the body of the latest post in this conversation.</span></span>                                                                                                                           |
| <span data-ttu-id="f521e-165">isLocked</span><span class="sxs-lookup"><span data-stu-id="f521e-165">isLocked</span></span>              | <span data-ttu-id="f521e-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="f521e-166">Boolean</span></span>                              | <span data-ttu-id="f521e-167">Указывает, заблокирована ли цепочка.</span><span class="sxs-lookup"><span data-stu-id="f521e-167">Indicates if the thread is locked.</span></span>                                                                                                                                                               |

## <a name="relationships"></a><span data-ttu-id="f521e-168">Связи</span><span class="sxs-lookup"><span data-stu-id="f521e-168">Relationships</span></span>
| <span data-ttu-id="f521e-169">Связь</span><span class="sxs-lookup"><span data-stu-id="f521e-169">Relationship</span></span> | <span data-ttu-id="f521e-170">Тип</span><span class="sxs-lookup"><span data-stu-id="f521e-170">Type</span></span>   |<span data-ttu-id="f521e-171">Описание</span><span class="sxs-lookup"><span data-stu-id="f521e-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f521e-172">posts</span><span class="sxs-lookup"><span data-stu-id="f521e-172">posts</span></span>|<span data-ttu-id="f521e-173">Коллекция [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="f521e-173">[post](post.md) collection</span></span>| <span data-ttu-id="f521e-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f521e-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f521e-176">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f521e-176">JSON representation</span></span>

<span data-ttu-id="f521e-177">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f521e-177">Here is a JSON representation of the resource</span></span>

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

