---
title: Тип ресурса Chat
description: Чат — это коллекция chatMessages между одним или несколькими участниками.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 88d08c8e6e0222c339c99db9cab9243f9c48c1f3
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597268"
---
# <a name="chat-resource-type"></a><span data-ttu-id="163ef-103">Тип ресурса Chat</span><span class="sxs-lookup"><span data-stu-id="163ef-103">chat resource type</span></span>

<span data-ttu-id="163ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="163ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="163ef-105">Чат — это коллекция [chatMessages](chatmessage.md) между одним или несколькими участниками.</span><span class="sxs-lookup"><span data-stu-id="163ef-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="163ef-106">Участники могут быть пользователями или приложениями.</span><span class="sxs-lookup"><span data-stu-id="163ef-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="163ef-107">Методы</span><span class="sxs-lookup"><span data-stu-id="163ef-107">Methods</span></span>

|  <span data-ttu-id="163ef-108">Метод</span><span class="sxs-lookup"><span data-stu-id="163ef-108">Method</span></span>       |  <span data-ttu-id="163ef-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="163ef-109">Return Type</span></span>  | <span data-ttu-id="163ef-110">Описание</span><span class="sxs-lookup"><span data-stu-id="163ef-110">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="163ef-111">Список чатов</span><span class="sxs-lookup"><span data-stu-id="163ef-111">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="163ef-112">Коллекция [чата](chat.md)</span><span class="sxs-lookup"><span data-stu-id="163ef-112">[chat](chat.md) collection</span></span> | <span data-ttu-id="163ef-113">Получение списка сеансов, в которые входит пользователь.</span><span class="sxs-lookup"><span data-stu-id="163ef-113">Get the list of chats a user is part of.</span></span>| 
|[<span data-ttu-id="163ef-114">Получение чата</span><span class="sxs-lookup"><span data-stu-id="163ef-114">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="163ef-115">chat</span><span class="sxs-lookup"><span data-stu-id="163ef-115">chat</span></span>](chat.md) | <span data-ttu-id="163ef-116">Чтение свойств и связей чата.</span><span class="sxs-lookup"><span data-stu-id="163ef-116">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="163ef-117">Список членов чата</span><span class="sxs-lookup"><span data-stu-id="163ef-117">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="163ef-118">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="163ef-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="163ef-119">Получение списка всех пользователей в чате.</span><span class="sxs-lookup"><span data-stu-id="163ef-119">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="163ef-120">Получение члена чата</span><span class="sxs-lookup"><span data-stu-id="163ef-120">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="163ef-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="163ef-121">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="163ef-122">Получение одного пользователя в чате.</span><span class="sxs-lookup"><span data-stu-id="163ef-122">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="163ef-123">Список сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="163ef-123">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="163ef-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="163ef-124">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="163ef-125">Получение сообщений в индивидуальном или групповом чате.</span><span class="sxs-lookup"><span data-stu-id="163ef-125">Get messages in a 1:1 or group chat.</span></span> | 
|[<span data-ttu-id="163ef-126">Получение сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="163ef-126">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="163ef-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="163ef-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="163ef-128">Получение одного сообщения в чате.</span><span class="sxs-lookup"><span data-stu-id="163ef-128">Get a single message in a chat.</span></span> | 
|[<span data-ttu-id="163ef-129">Получение разговора между пользователем и приложением</span><span class="sxs-lookup"><span data-stu-id="163ef-129">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="163ef-130">chat</span><span class="sxs-lookup"><span data-stu-id="163ef-130">chat</span></span>](chat.md)| <span data-ttu-id="163ef-131">Получение одного сеанса разговора между пользователем и приложением</span><span class="sxs-lookup"><span data-stu-id="163ef-131">Get one-on-one chat between user and the app</span></span> |
|[<span data-ttu-id="163ef-132">Получение всех сообщений чата</span><span class="sxs-lookup"><span data-stu-id="163ef-132">Get all chat messages</span></span>](../api/chats-getallmessages.md)| <span data-ttu-id="163ef-133">Коллекция [чата](chat.md)</span><span class="sxs-lookup"><span data-stu-id="163ef-133">[chat](chat.md) collection</span></span>| <span data-ttu-id="163ef-134">Получение сообщений от всех чатов, в которых пользователь является участником, в том числе беседы в одном месте, групповых чатов и сеансов собраний.</span><span class="sxs-lookup"><span data-stu-id="163ef-134">Get messages from all chats that a user is a participant in, including one-on-one chats, group chats, and meeting chats.</span></span> |

><span data-ttu-id="163ef-135">**Примечание:** При использовании разрешений приложений необходимо знать, как вы будете получать идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="163ef-135">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="163ef-136">Так как перечисление бесед с разрешениями приложений не поддерживается, не все сценарии возможны.</span><span class="sxs-lookup"><span data-stu-id="163ef-136">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="163ef-137">Можно получить идентификаторы чата с делегированными разрешениями и из [уведомлений об изменениях для/ЧАТС/жеталлмессажес](../api/subscription-post-subscriptions.md) с разрешениями приложений.</span><span class="sxs-lookup"><span data-stu-id="163ef-137">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="163ef-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="163ef-138">Properties</span></span>

| <span data-ttu-id="163ef-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="163ef-139">Property</span></span>   | <span data-ttu-id="163ef-140">Тип</span><span class="sxs-lookup"><span data-stu-id="163ef-140">Type</span></span> |<span data-ttu-id="163ef-141">Описание</span><span class="sxs-lookup"><span data-stu-id="163ef-141">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="163ef-142">id</span><span class="sxs-lookup"><span data-stu-id="163ef-142">id</span></span>| <span data-ttu-id="163ef-143">String</span><span class="sxs-lookup"><span data-stu-id="163ef-143">String</span></span>| <span data-ttu-id="163ef-144">Уникальный идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="163ef-144">The chat's unique identifier.</span></span> <span data-ttu-id="163ef-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="163ef-145">Read-only.</span></span>|
| <span data-ttu-id="163ef-146">topic</span><span class="sxs-lookup"><span data-stu-id="163ef-146">topic</span></span>| <span data-ttu-id="163ef-147">String</span><span class="sxs-lookup"><span data-stu-id="163ef-147">String</span></span>|  <span data-ttu-id="163ef-148">Необязательно Тема или тема чата.</span><span class="sxs-lookup"><span data-stu-id="163ef-148">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="163ef-149">Доступно только для чатов групп.</span><span class="sxs-lookup"><span data-stu-id="163ef-149">Only available for group chats.</span></span>|
| <span data-ttu-id="163ef-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="163ef-150">createdDateTime</span></span>| <span data-ttu-id="163ef-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="163ef-151">dateTimeOffset</span></span>|  <span data-ttu-id="163ef-152">Дата и время создания чата.</span><span class="sxs-lookup"><span data-stu-id="163ef-152">Date and time at which the chat was created.</span></span> <span data-ttu-id="163ef-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="163ef-153">Read-only.</span></span>|
| <span data-ttu-id="163ef-154">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="163ef-154">lastUpdatedDateTime</span></span>| <span data-ttu-id="163ef-155">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="163ef-155">dateTimeOffset</span></span>|  <span data-ttu-id="163ef-156">Дата и время переименования чата или изменения членства.</span><span class="sxs-lookup"><span data-stu-id="163ef-156">Date and time at which the chat was renamed or membership changed.</span></span> <span data-ttu-id="163ef-157">Ластупдатеддатетиме не обновляется при отправке сообщения в чат.</span><span class="sxs-lookup"><span data-stu-id="163ef-157">lastUpdatedDateTime is not updated when a message is sent to the chat.</span></span> <span data-ttu-id="163ef-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="163ef-158">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="163ef-159">Связи</span><span class="sxs-lookup"><span data-stu-id="163ef-159">Relationships</span></span>

| <span data-ttu-id="163ef-160">Связь</span><span class="sxs-lookup"><span data-stu-id="163ef-160">Relationship</span></span> | <span data-ttu-id="163ef-161">Тип</span><span class="sxs-lookup"><span data-stu-id="163ef-161">Type</span></span> |<span data-ttu-id="163ef-162">Описание</span><span class="sxs-lookup"><span data-stu-id="163ef-162">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="163ef-163">installedApps</span><span class="sxs-lookup"><span data-stu-id="163ef-163">installedApps</span></span> | <span data-ttu-id="163ef-164">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="163ef-164">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="163ef-165">Коллекция всех приложений в чате.</span><span class="sxs-lookup"><span data-stu-id="163ef-165">A collection of all the apps in the chat.</span></span> <span data-ttu-id="163ef-166">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="163ef-166">Nullable.</span></span> |
| <span data-ttu-id="163ef-167">members</span><span class="sxs-lookup"><span data-stu-id="163ef-167">members</span></span> | <span data-ttu-id="163ef-168">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="163ef-168">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="163ef-169">Коллекция всех людей в чате.</span><span class="sxs-lookup"><span data-stu-id="163ef-169">A collection of all people in the chat.</span></span> <span data-ttu-id="163ef-170">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="163ef-170">Nullable.</span></span> |
| <span data-ttu-id="163ef-171">messages</span><span class="sxs-lookup"><span data-stu-id="163ef-171">messages</span></span> | <span data-ttu-id="163ef-172">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="163ef-172">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="163ef-173">Коллекция всех сообщений в чате.</span><span class="sxs-lookup"><span data-stu-id="163ef-173">A collection of all the messages in the chat.</span></span> <span data-ttu-id="163ef-174">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="163ef-174">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="163ef-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="163ef-175">JSON representation</span></span>

<span data-ttu-id="163ef-176">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="163ef-176">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="163ef-177">См. также</span><span class="sxs-lookup"><span data-stu-id="163ef-177">See also</span></span>

- [<span data-ttu-id="163ef-178">channel</span><span class="sxs-lookup"><span data-stu-id="163ef-178">channel</span></span>](channel.md)
- [<span data-ttu-id="163ef-179">chatMessage</span><span class="sxs-lookup"><span data-stu-id="163ef-179">chatMessage</span></span>](chatmessage.md)

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


