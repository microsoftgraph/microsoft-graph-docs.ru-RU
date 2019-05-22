---
title: Тип ресурса Chat
description: Чат — это коллекция chatMessages между одним или несколькими участниками.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4d0f1009079c4994814385ae8758af6c211f17a2
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2019
ms.locfileid: "34344978"
---
# <a name="chat-resource-type"></a><span data-ttu-id="85c46-103">Тип ресурса Chat</span><span class="sxs-lookup"><span data-stu-id="85c46-103">chat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85c46-104">Чат — это коллекция [chatMessages](chatmessage.md) между одним или несколькими участниками.</span><span class="sxs-lookup"><span data-stu-id="85c46-104">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="85c46-105">Участники могут быть пользователями или приложениями.</span><span class="sxs-lookup"><span data-stu-id="85c46-105">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="85c46-106">Методы</span><span class="sxs-lookup"><span data-stu-id="85c46-106">Methods</span></span>

|  <span data-ttu-id="85c46-107">Метод</span><span class="sxs-lookup"><span data-stu-id="85c46-107">Method</span></span>       |  <span data-ttu-id="85c46-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="85c46-108">Return Type</span></span>  | <span data-ttu-id="85c46-109">Описание</span><span class="sxs-lookup"><span data-stu-id="85c46-109">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="85c46-110">Список чатов</span><span class="sxs-lookup"><span data-stu-id="85c46-110">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="85c46-111">Коллекция [чата](channel.md)</span><span class="sxs-lookup"><span data-stu-id="85c46-111">[chat](channel.md) collection</span></span> | <span data-ttu-id="85c46-112">Получение списка сеансов, в которые входит пользователь.</span><span class="sxs-lookup"><span data-stu-id="85c46-112">Get the list of chats a user is part of.</span></span>|
|[<span data-ttu-id="85c46-113">Получение чата</span><span class="sxs-lookup"><span data-stu-id="85c46-113">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="85c46-114">отображаются</span><span class="sxs-lookup"><span data-stu-id="85c46-114">chat</span></span>](channel.md) | <span data-ttu-id="85c46-115">Чтение свойств и связей чата.</span><span class="sxs-lookup"><span data-stu-id="85c46-115">Read properties and relationships of the chat.</span></span>|
|[<span data-ttu-id="85c46-116">Список членов чата</span><span class="sxs-lookup"><span data-stu-id="85c46-116">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="85c46-117">Коллекция [конверсатионмембер](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="85c46-117">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="85c46-118">Получение списка всех пользователей в чате.</span><span class="sxs-lookup"><span data-stu-id="85c46-118">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="85c46-119">Получение члена чата</span><span class="sxs-lookup"><span data-stu-id="85c46-119">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="85c46-120">конверсатионмембер</span><span class="sxs-lookup"><span data-stu-id="85c46-120">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="85c46-121">Получение одного пользователя в чате.</span><span class="sxs-lookup"><span data-stu-id="85c46-121">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="85c46-122">Список сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="85c46-122">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="85c46-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="85c46-123">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="85c46-124">Получение сообщений в индивидуальном или групповом чате.</span><span class="sxs-lookup"><span data-stu-id="85c46-124">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="85c46-125">Получение сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="85c46-125">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="85c46-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="85c46-126">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="85c46-127">Получение одного сообщения в чате.</span><span class="sxs-lookup"><span data-stu-id="85c46-127">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="85c46-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="85c46-128">Properties</span></span>

| <span data-ttu-id="85c46-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="85c46-129">Property</span></span>     | <span data-ttu-id="85c46-130">Тип</span><span class="sxs-lookup"><span data-stu-id="85c46-130">Type</span></span>   |<span data-ttu-id="85c46-131">Описание</span><span class="sxs-lookup"><span data-stu-id="85c46-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="85c46-132">id</span><span class="sxs-lookup"><span data-stu-id="85c46-132">id</span></span>| <span data-ttu-id="85c46-133">String</span><span class="sxs-lookup"><span data-stu-id="85c46-133">String</span></span>| <span data-ttu-id="85c46-134">Уникальный идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="85c46-134">The chat's unique identifier.</span></span> <span data-ttu-id="85c46-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85c46-135">Read-only.</span></span>|
| <span data-ttu-id="85c46-136">topic</span><span class="sxs-lookup"><span data-stu-id="85c46-136">topic</span></span>| <span data-ttu-id="85c46-137">String</span><span class="sxs-lookup"><span data-stu-id="85c46-137">String</span></span>|  <span data-ttu-id="85c46-138">Необязательно Тема или тема чата.</span><span class="sxs-lookup"><span data-stu-id="85c46-138">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="85c46-139">Доступно только для чатов групп.</span><span class="sxs-lookup"><span data-stu-id="85c46-139">Only available for group chats.</span></span>|
| <span data-ttu-id="85c46-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85c46-140">createdDateTime</span></span>| <span data-ttu-id="85c46-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85c46-141">dateTimeOffset</span></span>|  <span data-ttu-id="85c46-142">Дата и время создания чата.</span><span class="sxs-lookup"><span data-stu-id="85c46-142">Date and time at which the chat was created.</span></span> <span data-ttu-id="85c46-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85c46-143">Read-only.</span></span>|
| <span data-ttu-id="85c46-144">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="85c46-144">lastUpdatedDateTime</span></span>| <span data-ttu-id="85c46-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85c46-145">dateTimeOffset</span></span>|  <span data-ttu-id="85c46-146">Дата и время обновления чата.</span><span class="sxs-lookup"><span data-stu-id="85c46-146">Date and time at which the chat was updated.</span></span> <span data-ttu-id="85c46-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85c46-147">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85c46-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="85c46-148">Relationships</span></span>
| <span data-ttu-id="85c46-149">Отношение</span><span class="sxs-lookup"><span data-stu-id="85c46-149">Relationship</span></span> | <span data-ttu-id="85c46-150">Тип</span><span class="sxs-lookup"><span data-stu-id="85c46-150">Type</span></span>   |<span data-ttu-id="85c46-151">Описание</span><span class="sxs-lookup"><span data-stu-id="85c46-151">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="85c46-152">members</span><span class="sxs-lookup"><span data-stu-id="85c46-152">members</span></span> | <span data-ttu-id="85c46-153">Коллекция [конверсатионмембер](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="85c46-153">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="85c46-154">Коллекция всех людей в чате.</span><span class="sxs-lookup"><span data-stu-id="85c46-154">A collection of all people in the chat.</span></span> <span data-ttu-id="85c46-155">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="85c46-155">Nullable.</span></span> |
| <span data-ttu-id="85c46-156">messages</span><span class="sxs-lookup"><span data-stu-id="85c46-156">messages</span></span> | <span data-ttu-id="85c46-157">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="85c46-157">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="85c46-158">Коллекция всех сообщений в чате.</span><span class="sxs-lookup"><span data-stu-id="85c46-158">A collection of all the messages in the chat.</span></span> <span data-ttu-id="85c46-159">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="85c46-159">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="85c46-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85c46-160">JSON representation</span></span>

<span data-ttu-id="85c46-161">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85c46-161">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="85c46-162">См. также</span><span class="sxs-lookup"><span data-stu-id="85c46-162">See also</span></span>

- [<span data-ttu-id="85c46-163">channel</span><span class="sxs-lookup"><span data-stu-id="85c46-163">channel</span></span>](channel.md)
- [<span data-ttu-id="85c46-164">chatMessage</span><span class="sxs-lookup"><span data-stu-id="85c46-164">chatMessage</span></span>](chatmessage.md)

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
