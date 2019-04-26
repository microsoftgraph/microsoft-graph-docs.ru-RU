---
title: Тип ресурса Chat
description: Чат — это коллекция chatMessages между одним или несколькими участниками.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1091021235a50d3dfa237467e319da9b131b7a72
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339719"
---
# <a name="chat-resource-type"></a><span data-ttu-id="1519b-103">Тип ресурса Chat</span><span class="sxs-lookup"><span data-stu-id="1519b-103">chat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1519b-104">Чат — это коллекция [chatMessages](chatmessage.md) между одним или несколькими участниками.</span><span class="sxs-lookup"><span data-stu-id="1519b-104">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="1519b-105">Участники могут быть пользователями или приложениями.</span><span class="sxs-lookup"><span data-stu-id="1519b-105">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="1519b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1519b-106">Methods</span></span>

|  <span data-ttu-id="1519b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1519b-107">Method</span></span>       |  <span data-ttu-id="1519b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1519b-108">Return Type</span></span>  | <span data-ttu-id="1519b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1519b-109">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="1519b-110">Список чатов</span><span class="sxs-lookup"><span data-stu-id="1519b-110">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="1519b-111">Коллекция [чата](channel.md)</span><span class="sxs-lookup"><span data-stu-id="1519b-111">[chat](channel.md) collection</span></span> | <span data-ttu-id="1519b-112">Получение списка сеансов, в которые входит пользователь.</span><span class="sxs-lookup"><span data-stu-id="1519b-112">Get the list of chats a user is part of.</span></span>|
|[<span data-ttu-id="1519b-113">Получение чата</span><span class="sxs-lookup"><span data-stu-id="1519b-113">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="1519b-114">отображаются</span><span class="sxs-lookup"><span data-stu-id="1519b-114">chat</span></span>](channel.md) | <span data-ttu-id="1519b-115">Чтение свойств и связей чата.</span><span class="sxs-lookup"><span data-stu-id="1519b-115">Read properties and relationships of the chat.</span></span>|
|[<span data-ttu-id="1519b-116">ПереЧисление сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="1519b-116">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="1519b-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="1519b-117">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="1519b-118">Получение сообщений в 1:1 или группе чата.</span><span class="sxs-lookup"><span data-stu-id="1519b-118">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="1519b-119">Получение сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="1519b-119">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="1519b-120">chatMessage</span><span class="sxs-lookup"><span data-stu-id="1519b-120">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="1519b-121">Получение одного сообщения в чате.</span><span class="sxs-lookup"><span data-stu-id="1519b-121">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="1519b-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="1519b-122">Properties</span></span>

| <span data-ttu-id="1519b-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="1519b-123">Property</span></span>     | <span data-ttu-id="1519b-124">Тип</span><span class="sxs-lookup"><span data-stu-id="1519b-124">Type</span></span>   |<span data-ttu-id="1519b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1519b-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1519b-126">id</span><span class="sxs-lookup"><span data-stu-id="1519b-126">id</span></span>| <span data-ttu-id="1519b-127">String</span><span class="sxs-lookup"><span data-stu-id="1519b-127">String</span></span>| <span data-ttu-id="1519b-128">Уникальный идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="1519b-128">The chat's unique identifier.</span></span> <span data-ttu-id="1519b-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1519b-129">Read-only.</span></span>|
| <span data-ttu-id="1519b-130">topic</span><span class="sxs-lookup"><span data-stu-id="1519b-130">topic</span></span>| <span data-ttu-id="1519b-131">String</span><span class="sxs-lookup"><span data-stu-id="1519b-131">String</span></span>|  <span data-ttu-id="1519b-132">Необязательно Тема или тема чата.</span><span class="sxs-lookup"><span data-stu-id="1519b-132">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="1519b-133">Доступно только для чатов групп.</span><span class="sxs-lookup"><span data-stu-id="1519b-133">Only available for group chats.</span></span>|
| <span data-ttu-id="1519b-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1519b-134">createdDateTime</span></span>| <span data-ttu-id="1519b-135">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1519b-135">dateTimeOffset</span></span>|  <span data-ttu-id="1519b-136">Дата и время создания чата.</span><span class="sxs-lookup"><span data-stu-id="1519b-136">Date and time at which the chat was created.</span></span> <span data-ttu-id="1519b-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1519b-137">Read-only.</span></span>|
| <span data-ttu-id="1519b-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1519b-138">lastUpdatedDateTime</span></span>| <span data-ttu-id="1519b-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1519b-139">dateTimeOffset</span></span>|  <span data-ttu-id="1519b-140">Дата и время обновления чата.</span><span class="sxs-lookup"><span data-stu-id="1519b-140">Date and time at which the chat was updated.</span></span> <span data-ttu-id="1519b-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1519b-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1519b-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="1519b-142">Relationships</span></span>
| <span data-ttu-id="1519b-143">Отношение</span><span class="sxs-lookup"><span data-stu-id="1519b-143">Relationship</span></span> | <span data-ttu-id="1519b-144">Тип</span><span class="sxs-lookup"><span data-stu-id="1519b-144">Type</span></span>   |<span data-ttu-id="1519b-145">Описание</span><span class="sxs-lookup"><span data-stu-id="1519b-145">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1519b-146">messages</span><span class="sxs-lookup"><span data-stu-id="1519b-146">messages</span></span> | <span data-ttu-id="1519b-147">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="1519b-147">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="1519b-148">Коллекция всех сообщений в чате.</span><span class="sxs-lookup"><span data-stu-id="1519b-148">A collection of all the messages in the chat.</span></span> <span data-ttu-id="1519b-149">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1519b-149">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1519b-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1519b-150">JSON representation</span></span>

<span data-ttu-id="1519b-151">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1519b-151">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chat"
}-->

```json
{
  "id": "string (identifier)",
  "topic": "string",
  "createdDateTime": "dateTimeOffset",
  "lastUpdatedDateTime": "dateTimeOffset"
}

```

## <a name="see-also"></a><span data-ttu-id="1519b-152">См. также</span><span class="sxs-lookup"><span data-stu-id="1519b-152">See also</span></span>

- [<span data-ttu-id="1519b-153">channel</span><span class="sxs-lookup"><span data-stu-id="1519b-153">channel</span></span>](channel.md)
- [<span data-ttu-id="1519b-154">chatMessage</span><span class="sxs-lookup"><span data-stu-id="1519b-154">chatMessage</span></span>](chatmessage.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
