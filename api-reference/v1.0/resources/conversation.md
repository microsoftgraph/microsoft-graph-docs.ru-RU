---
title: Тип ресурса conversation
description: Беседа — коллекция цепочек, содержащих записи. Все цепочки и записи в беседе имеют одинаковую тему.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 0066a636d2b36e74443380598c2ca6e8daf826c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563793"
---
# <a name="conversation-resource-type"></a><span data-ttu-id="e5ebf-104">Тип ресурса conversation</span><span class="sxs-lookup"><span data-stu-id="e5ebf-104">conversation resource type</span></span>

<span data-ttu-id="e5ebf-p102">Беседа — коллекция [цепочек](conversationthread.md), содержащих записи. Все цепочки и записи в беседе имеют одинаковую тему.</span><span class="sxs-lookup"><span data-stu-id="e5ebf-p102">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="e5ebf-107">Этот ресурс поддерживает подписку на [уведомления об изменениях](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="e5ebf-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="e5ebf-108">Методы</span><span class="sxs-lookup"><span data-stu-id="e5ebf-108">Methods</span></span>

| <span data-ttu-id="e5ebf-109">Метод</span><span class="sxs-lookup"><span data-stu-id="e5ebf-109">Method</span></span>       | <span data-ttu-id="e5ebf-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e5ebf-110">Return Type</span></span>  |<span data-ttu-id="e5ebf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e5ebf-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e5ebf-112">Список бесед</span><span class="sxs-lookup"><span data-stu-id="e5ebf-112">List conversations</span></span>](../api/group-list-conversations.md) | <span data-ttu-id="e5ebf-113">Коллекция [conversation](conversation.md)</span><span class="sxs-lookup"><span data-stu-id="e5ebf-113">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="e5ebf-114">Получение списка бесед в этой группе.</span><span class="sxs-lookup"><span data-stu-id="e5ebf-114">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="e5ebf-115">Создание</span><span class="sxs-lookup"><span data-stu-id="e5ebf-115">Create</span></span>](../api/group-post-conversations.md) |[<span data-ttu-id="e5ebf-116">conversation</span><span class="sxs-lookup"><span data-stu-id="e5ebf-116">conversation</span></span>](conversation.md)| <span data-ttu-id="e5ebf-117">Создание беседы путем включения цепочки и записи.</span><span class="sxs-lookup"><span data-stu-id="e5ebf-117">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="e5ebf-118">Получение беседы</span><span class="sxs-lookup"><span data-stu-id="e5ebf-118">Get conversation</span></span>](../api/conversation-get.md) | [<span data-ttu-id="e5ebf-119">conversation</span><span class="sxs-lookup"><span data-stu-id="e5ebf-119">conversation</span></span>](conversation.md) |<span data-ttu-id="e5ebf-120">Считывание свойств и отношений объекта conversation.</span><span class="sxs-lookup"><span data-stu-id="e5ebf-120">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="e5ebf-121">Удаление</span><span class="sxs-lookup"><span data-stu-id="e5ebf-121">Delete</span></span>](../api/conversation-delete.md) | <span data-ttu-id="e5ebf-122">Нет</span><span class="sxs-lookup"><span data-stu-id="e5ebf-122">None</span></span> |<span data-ttu-id="e5ebf-123">Удаление объекта conversation.</span><span class="sxs-lookup"><span data-stu-id="e5ebf-123">Delete conversation object.</span></span> |
|[<span data-ttu-id="e5ebf-124">Список цепочек беседы</span><span class="sxs-lookup"><span data-stu-id="e5ebf-124">List conversation threads</span></span>](../api/conversation-list-threads.md) |<span data-ttu-id="e5ebf-125">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="e5ebf-125">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="e5ebf-126">Получение всех цепочек в групповой беседе.</span><span class="sxs-lookup"><span data-stu-id="e5ebf-126">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="e5ebf-127">Создание цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="e5ebf-127">Create conversation thread</span></span>](../api/conversation-post-threads.md) |<span data-ttu-id="e5ebf-128">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="e5ebf-128">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="e5ebf-129">Создание цепочки в указанной беседе.</span><span class="sxs-lookup"><span data-stu-id="e5ebf-129">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5ebf-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5ebf-130">Properties</span></span>
| <span data-ttu-id="e5ebf-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5ebf-131">Property</span></span>     | <span data-ttu-id="e5ebf-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e5ebf-132">Type</span></span>   |<span data-ttu-id="e5ebf-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e5ebf-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5ebf-134">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="e5ebf-134">hasAttachments</span></span>|<span data-ttu-id="e5ebf-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5ebf-135">Boolean</span></span>|<span data-ttu-id="e5ebf-136">Указывает, содержит ли какая-либо запись в этой беседе хотя бы одно вложение.</span><span class="sxs-lookup"><span data-stu-id="e5ebf-136">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="e5ebf-137">id</span><span class="sxs-lookup"><span data-stu-id="e5ebf-137">id</span></span>|<span data-ttu-id="e5ebf-138">String</span><span class="sxs-lookup"><span data-stu-id="e5ebf-138">String</span></span>|<span data-ttu-id="e5ebf-p103">Уникальный идентификатор беседы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e5ebf-p103">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="e5ebf-141">Ластделивереддатетиме</span><span class="sxs-lookup"><span data-stu-id="e5ebf-141">lastDeliveredDateTime</span></span>|<span data-ttu-id="e5ebf-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5ebf-142">DateTimeOffset</span></span>|<span data-ttu-id="e5ebf-p104">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e5ebf-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e5ebf-145">preview</span><span class="sxs-lookup"><span data-stu-id="e5ebf-145">preview</span></span>|<span data-ttu-id="e5ebf-146">String</span><span class="sxs-lookup"><span data-stu-id="e5ebf-146">String</span></span>|<span data-ttu-id="e5ebf-147">Краткая сводка из текста последней записи в этой беседе.</span><span class="sxs-lookup"><span data-stu-id="e5ebf-147">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="e5ebf-148">topic</span><span class="sxs-lookup"><span data-stu-id="e5ebf-148">topic</span></span>|<span data-ttu-id="e5ebf-149">String</span><span class="sxs-lookup"><span data-stu-id="e5ebf-149">String</span></span>|<span data-ttu-id="e5ebf-p105">Тема беседы. Это свойство можно задать при создании беседы, но его невозможно обновить.</span><span class="sxs-lookup"><span data-stu-id="e5ebf-p105">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="e5ebf-152">Уникуесендерс</span><span class="sxs-lookup"><span data-stu-id="e5ebf-152">uniqueSenders</span></span>|<span data-ttu-id="e5ebf-153">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e5ebf-153">String collection</span></span>|<span data-ttu-id="e5ebf-154">Все пользователи, которые отправили сообщение в эту беседу.</span><span class="sxs-lookup"><span data-stu-id="e5ebf-154">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5ebf-155">Связи</span><span class="sxs-lookup"><span data-stu-id="e5ebf-155">Relationships</span></span>
| <span data-ttu-id="e5ebf-156">Отношение</span><span class="sxs-lookup"><span data-stu-id="e5ebf-156">Relationship</span></span> | <span data-ttu-id="e5ebf-157">Тип</span><span class="sxs-lookup"><span data-stu-id="e5ebf-157">Type</span></span>   |<span data-ttu-id="e5ebf-158">Описание</span><span class="sxs-lookup"><span data-stu-id="e5ebf-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5ebf-159">threads</span><span class="sxs-lookup"><span data-stu-id="e5ebf-159">threads</span></span>|<span data-ttu-id="e5ebf-160">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="e5ebf-160">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="e5ebf-p106">Коллекция всех цепочек в беседе. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e5ebf-p106">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5ebf-165">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e5ebf-165">JSON representation</span></span>

<span data-ttu-id="e5ebf-166">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5ebf-166">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversation",
  "@odata.annotations": [
    {
      "property": "threads",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"],

  "threads": [{"@odata.type": "microsoft.graph.conversationThread"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
