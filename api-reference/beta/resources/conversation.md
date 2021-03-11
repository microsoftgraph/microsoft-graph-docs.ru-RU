---
title: Тип ресурса conversation
description: Беседа — коллекция цепочек, содержащих записи. Все цепочки и записи в беседе имеют одинаковую тему.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: b3dd263a91552afc4db42cb2cc1791741dc24473
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721672"
---
# <a name="conversation-resource-type"></a><span data-ttu-id="5e97c-104">Тип ресурса conversation</span><span class="sxs-lookup"><span data-stu-id="5e97c-104">conversation resource type</span></span>

<span data-ttu-id="5e97c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e97c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e97c-p102">Беседа — коллекция [цепочек](conversationthread.md), содержащих записи. Все цепочки и записи в беседе имеют одинаковую тему.</span><span class="sxs-lookup"><span data-stu-id="5e97c-p102">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="5e97c-108">Этот ресурс поддерживает подписку на изменение [уведомлений.](/graph/webhooks)</span><span class="sxs-lookup"><span data-stu-id="5e97c-108">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="5e97c-109">Методы</span><span class="sxs-lookup"><span data-stu-id="5e97c-109">Methods</span></span>

| <span data-ttu-id="5e97c-110">Метод</span><span class="sxs-lookup"><span data-stu-id="5e97c-110">Method</span></span>       | <span data-ttu-id="5e97c-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5e97c-111">Return Type</span></span>  |<span data-ttu-id="5e97c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5e97c-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5e97c-113">Перечисление бесед</span><span class="sxs-lookup"><span data-stu-id="5e97c-113">List conversations</span></span>](../api/group-list-conversations.md) | <span data-ttu-id="5e97c-114">Коллекция [conversation](conversation.md)</span><span class="sxs-lookup"><span data-stu-id="5e97c-114">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="5e97c-115">Получение списка бесед в этой группе.</span><span class="sxs-lookup"><span data-stu-id="5e97c-115">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="5e97c-116">Создание</span><span class="sxs-lookup"><span data-stu-id="5e97c-116">Create</span></span>](../api/group-post-conversations.md) |[<span data-ttu-id="5e97c-117">conversation</span><span class="sxs-lookup"><span data-stu-id="5e97c-117">conversation</span></span>](conversation.md)| <span data-ttu-id="5e97c-118">Создание беседы путем включения цепочки и записи.</span><span class="sxs-lookup"><span data-stu-id="5e97c-118">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="5e97c-119">Получение беседы</span><span class="sxs-lookup"><span data-stu-id="5e97c-119">Get conversation</span></span>](../api/conversation-get.md) | [<span data-ttu-id="5e97c-120">conversation</span><span class="sxs-lookup"><span data-stu-id="5e97c-120">conversation</span></span>](conversation.md) |<span data-ttu-id="5e97c-121">Считывание свойств и отношений объекта conversation.</span><span class="sxs-lookup"><span data-stu-id="5e97c-121">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="5e97c-122">Удаление</span><span class="sxs-lookup"><span data-stu-id="5e97c-122">Delete</span></span>](../api/conversation-delete.md) | <span data-ttu-id="5e97c-123">Нет</span><span class="sxs-lookup"><span data-stu-id="5e97c-123">None</span></span> |<span data-ttu-id="5e97c-124">Удаление объекта conversation.</span><span class="sxs-lookup"><span data-stu-id="5e97c-124">Delete conversation object.</span></span> |
|[<span data-ttu-id="5e97c-125">Список цепочек беседы</span><span class="sxs-lookup"><span data-stu-id="5e97c-125">List conversation threads</span></span>](../api/conversation-list-threads.md) |<span data-ttu-id="5e97c-126">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="5e97c-126">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="5e97c-127">Получение всех цепочек в групповой беседе.</span><span class="sxs-lookup"><span data-stu-id="5e97c-127">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="5e97c-128">Создание цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="5e97c-128">Create conversation thread</span></span>](../api/conversation-post-threads.md) |<span data-ttu-id="5e97c-129">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="5e97c-129">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="5e97c-130">Создание цепочки в указанной беседе.</span><span class="sxs-lookup"><span data-stu-id="5e97c-130">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e97c-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e97c-131">Properties</span></span>
| <span data-ttu-id="5e97c-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e97c-132">Property</span></span>     | <span data-ttu-id="5e97c-133">Тип</span><span class="sxs-lookup"><span data-stu-id="5e97c-133">Type</span></span>   |<span data-ttu-id="5e97c-134">Описание</span><span class="sxs-lookup"><span data-stu-id="5e97c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e97c-135">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="5e97c-135">hasAttachments</span></span>|<span data-ttu-id="5e97c-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e97c-136">Boolean</span></span>|<span data-ttu-id="5e97c-137">Указывает, содержит ли какая-либо запись в этой беседе хотя бы одно вложение.</span><span class="sxs-lookup"><span data-stu-id="5e97c-137">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="5e97c-138">id</span><span class="sxs-lookup"><span data-stu-id="5e97c-138">id</span></span>|<span data-ttu-id="5e97c-139">String</span><span class="sxs-lookup"><span data-stu-id="5e97c-139">String</span></span>|<span data-ttu-id="5e97c-p103">Уникальный идентификатор беседы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e97c-p103">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="5e97c-142">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="5e97c-142">lastDeliveredDateTime</span></span>|<span data-ttu-id="5e97c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e97c-143">DateTimeOffset</span></span>|<span data-ttu-id="5e97c-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5e97c-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5e97c-145">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5e97c-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="5e97c-146">preview</span><span class="sxs-lookup"><span data-stu-id="5e97c-146">preview</span></span>|<span data-ttu-id="5e97c-147">String</span><span class="sxs-lookup"><span data-stu-id="5e97c-147">String</span></span>|<span data-ttu-id="5e97c-148">Краткая сводка из текста последней записи в этой беседе.</span><span class="sxs-lookup"><span data-stu-id="5e97c-148">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="5e97c-149">topic</span><span class="sxs-lookup"><span data-stu-id="5e97c-149">topic</span></span>|<span data-ttu-id="5e97c-150">String</span><span class="sxs-lookup"><span data-stu-id="5e97c-150">String</span></span>|<span data-ttu-id="5e97c-p105">Тема беседы. Это свойство можно задать при создании беседы, но его невозможно обновить.</span><span class="sxs-lookup"><span data-stu-id="5e97c-p105">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="5e97c-153">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="5e97c-153">uniqueSenders</span></span>|<span data-ttu-id="5e97c-154">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5e97c-154">String collection</span></span>|<span data-ttu-id="5e97c-155">Все пользователи, которые отправили сообщение в эту беседу.</span><span class="sxs-lookup"><span data-stu-id="5e97c-155">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e97c-156">Связи</span><span class="sxs-lookup"><span data-stu-id="5e97c-156">Relationships</span></span>
| <span data-ttu-id="5e97c-157">Связь</span><span class="sxs-lookup"><span data-stu-id="5e97c-157">Relationship</span></span> | <span data-ttu-id="5e97c-158">Тип</span><span class="sxs-lookup"><span data-stu-id="5e97c-158">Type</span></span>   |<span data-ttu-id="5e97c-159">Описание</span><span class="sxs-lookup"><span data-stu-id="5e97c-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e97c-160">threads</span><span class="sxs-lookup"><span data-stu-id="5e97c-160">threads</span></span>|<span data-ttu-id="5e97c-161">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="5e97c-161">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="5e97c-p106">Коллекция всех цепочек в беседе. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5e97c-p106">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e97c-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e97c-166">JSON representation</span></span>

<span data-ttu-id="5e97c-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e97c-167">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversation"
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


