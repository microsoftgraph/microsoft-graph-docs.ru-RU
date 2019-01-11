---
title: Тип ресурса conversation
description: Беседа — коллекция цепочек, содержащих записи. Все цепочки и записи в беседе имеют одинаковую тему.
localization_priority: Normal
ms.openlocfilehash: 69ae0a8ca7d5040ae1701a52cec007e3ad55449e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815003"
---
# <a name="conversation-resource-type"></a><span data-ttu-id="138f2-104">Тип ресурса conversation</span><span class="sxs-lookup"><span data-stu-id="138f2-104">conversation resource type</span></span>

> <span data-ttu-id="138f2-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="138f2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="138f2-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="138f2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="138f2-p103">Беседа — коллекция [цепочек](conversationthread.md), содержащих записи. Все цепочки и записи в беседе имеют одинаковую тему.</span><span class="sxs-lookup"><span data-stu-id="138f2-p103">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="138f2-109">Этот ресурс поддерживает подписки на [уведомления об изменении](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="138f2-109">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="138f2-110">Методы</span><span class="sxs-lookup"><span data-stu-id="138f2-110">Methods</span></span>

| <span data-ttu-id="138f2-111">Метод</span><span class="sxs-lookup"><span data-stu-id="138f2-111">Method</span></span>       | <span data-ttu-id="138f2-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="138f2-112">Return Type</span></span>  |<span data-ttu-id="138f2-113">Описание</span><span class="sxs-lookup"><span data-stu-id="138f2-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="138f2-114">Список бесед</span><span class="sxs-lookup"><span data-stu-id="138f2-114">List conversations</span></span>](../api/group-list-conversations.md) | <span data-ttu-id="138f2-115">Коллекция [conversation](conversation.md)</span><span class="sxs-lookup"><span data-stu-id="138f2-115">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="138f2-116">Получение списка бесед в этой группе.</span><span class="sxs-lookup"><span data-stu-id="138f2-116">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="138f2-117">Создание</span><span class="sxs-lookup"><span data-stu-id="138f2-117">Create</span></span>](../api/group-post-conversations.md) |[<span data-ttu-id="138f2-118">conversation</span><span class="sxs-lookup"><span data-stu-id="138f2-118">conversation</span></span>](conversation.md)| <span data-ttu-id="138f2-119">Создание беседы путем включения цепочки и записи.</span><span class="sxs-lookup"><span data-stu-id="138f2-119">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="138f2-120">Получение беседы</span><span class="sxs-lookup"><span data-stu-id="138f2-120">Get conversation</span></span>](../api/conversation-get.md) | [<span data-ttu-id="138f2-121">conversation</span><span class="sxs-lookup"><span data-stu-id="138f2-121">conversation</span></span>](conversation.md) |<span data-ttu-id="138f2-122">Считывание свойств и отношений объекта conversation.</span><span class="sxs-lookup"><span data-stu-id="138f2-122">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="138f2-123">Удаление</span><span class="sxs-lookup"><span data-stu-id="138f2-123">Delete</span></span>](../api/conversation-delete.md) | <span data-ttu-id="138f2-124">Нет</span><span class="sxs-lookup"><span data-stu-id="138f2-124">None</span></span> |<span data-ttu-id="138f2-125">Удаление объекта conversation.</span><span class="sxs-lookup"><span data-stu-id="138f2-125">Delete conversation object.</span></span> |
|[<span data-ttu-id="138f2-126">Список цепочек беседы</span><span class="sxs-lookup"><span data-stu-id="138f2-126">List conversation threads</span></span>](../api/conversation-list-threads.md) |<span data-ttu-id="138f2-127">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="138f2-127">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="138f2-128">Получение всех цепочек в групповой беседе.</span><span class="sxs-lookup"><span data-stu-id="138f2-128">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="138f2-129">Создание цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="138f2-129">Create conversation thread</span></span>](../api/conversation-post-threads.md) |<span data-ttu-id="138f2-130">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="138f2-130">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="138f2-131">Создание цепочки в указанной беседе.</span><span class="sxs-lookup"><span data-stu-id="138f2-131">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="138f2-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="138f2-132">Properties</span></span>
| <span data-ttu-id="138f2-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="138f2-133">Property</span></span>     | <span data-ttu-id="138f2-134">Тип</span><span class="sxs-lookup"><span data-stu-id="138f2-134">Type</span></span>   |<span data-ttu-id="138f2-135">Описание</span><span class="sxs-lookup"><span data-stu-id="138f2-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="138f2-136">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="138f2-136">hasAttachments</span></span>|<span data-ttu-id="138f2-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="138f2-137">Boolean</span></span>|<span data-ttu-id="138f2-138">Указывает, содержит ли какая-либо запись в этой беседе хотя бы одно вложение.</span><span class="sxs-lookup"><span data-stu-id="138f2-138">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="138f2-139">id</span><span class="sxs-lookup"><span data-stu-id="138f2-139">id</span></span>|<span data-ttu-id="138f2-140">String</span><span class="sxs-lookup"><span data-stu-id="138f2-140">String</span></span>|<span data-ttu-id="138f2-p104">Уникальный идентификатор беседы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="138f2-p104">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="138f2-143">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="138f2-143">lastDeliveredDateTime</span></span>|<span data-ttu-id="138f2-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="138f2-144">DateTimeOffset</span></span>|<span data-ttu-id="138f2-p105">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="138f2-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="138f2-147">preview</span><span class="sxs-lookup"><span data-stu-id="138f2-147">preview</span></span>|<span data-ttu-id="138f2-148">String</span><span class="sxs-lookup"><span data-stu-id="138f2-148">String</span></span>|<span data-ttu-id="138f2-149">Краткая сводка из текста последней записи в этой беседе.</span><span class="sxs-lookup"><span data-stu-id="138f2-149">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="138f2-150">topic</span><span class="sxs-lookup"><span data-stu-id="138f2-150">topic</span></span>|<span data-ttu-id="138f2-151">String</span><span class="sxs-lookup"><span data-stu-id="138f2-151">String</span></span>|<span data-ttu-id="138f2-p106">Тема беседы. Это свойство можно задать при создании беседы, но его невозможно обновить.</span><span class="sxs-lookup"><span data-stu-id="138f2-p106">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="138f2-154">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="138f2-154">uniqueSenders</span></span>|<span data-ttu-id="138f2-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="138f2-155">String collection</span></span>|<span data-ttu-id="138f2-156">Все пользователи, которые отправили сообщение в эту беседу.</span><span class="sxs-lookup"><span data-stu-id="138f2-156">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="138f2-157">Отношения</span><span class="sxs-lookup"><span data-stu-id="138f2-157">Relationships</span></span>
| <span data-ttu-id="138f2-158">Связь</span><span class="sxs-lookup"><span data-stu-id="138f2-158">Relationship</span></span> | <span data-ttu-id="138f2-159">Тип</span><span class="sxs-lookup"><span data-stu-id="138f2-159">Type</span></span>   |<span data-ttu-id="138f2-160">Описание</span><span class="sxs-lookup"><span data-stu-id="138f2-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="138f2-161">threads</span><span class="sxs-lookup"><span data-stu-id="138f2-161">threads</span></span>|<span data-ttu-id="138f2-162">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="138f2-162">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="138f2-p107">Коллекция всех цепочек в беседе. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="138f2-p107">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="138f2-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="138f2-167">JSON representation</span></span>

<span data-ttu-id="138f2-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="138f2-168">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
