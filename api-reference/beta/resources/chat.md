---
title: Тип ресурса Chat
description: Чат — это коллекция chatMessages между одним или несколькими участниками.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e6316f7c3aad0fc90e258d145b57942395265ce7
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563452"
---
# <a name="chat-resource-type"></a><span data-ttu-id="b6d30-103">Тип ресурса Chat</span><span class="sxs-lookup"><span data-stu-id="b6d30-103">chat resource type</span></span>

<span data-ttu-id="b6d30-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6d30-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6d30-105">Чат — это коллекция [chatMessages](chatmessage.md) между одним или несколькими участниками.</span><span class="sxs-lookup"><span data-stu-id="b6d30-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="b6d30-106">Участники могут быть пользователями или приложениями.</span><span class="sxs-lookup"><span data-stu-id="b6d30-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="b6d30-107">Методы</span><span class="sxs-lookup"><span data-stu-id="b6d30-107">Methods</span></span>

|  <span data-ttu-id="b6d30-108">Метод</span><span class="sxs-lookup"><span data-stu-id="b6d30-108">Method</span></span>       |  <span data-ttu-id="b6d30-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b6d30-109">Return Type</span></span>  | <span data-ttu-id="b6d30-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b6d30-110">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="b6d30-111">Список чатов</span><span class="sxs-lookup"><span data-stu-id="b6d30-111">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="b6d30-112">Коллекция [чата](chat.md)</span><span class="sxs-lookup"><span data-stu-id="b6d30-112">[chat](chat.md) collection</span></span> | <span data-ttu-id="b6d30-113">Получение списка сеансов, в которые входит пользователь.</span><span class="sxs-lookup"><span data-stu-id="b6d30-113">Get the list of chats a user is part of.</span></span>| 
|[<span data-ttu-id="b6d30-114">Получение чата</span><span class="sxs-lookup"><span data-stu-id="b6d30-114">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="b6d30-115">chat</span><span class="sxs-lookup"><span data-stu-id="b6d30-115">chat</span></span>](chat.md) | <span data-ttu-id="b6d30-116">Чтение свойств и связей чата.</span><span class="sxs-lookup"><span data-stu-id="b6d30-116">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="b6d30-117">Список членов чата</span><span class="sxs-lookup"><span data-stu-id="b6d30-117">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="b6d30-118">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="b6d30-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="b6d30-119">Получение списка всех пользователей в чате.</span><span class="sxs-lookup"><span data-stu-id="b6d30-119">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="b6d30-120">Получение члена чата</span><span class="sxs-lookup"><span data-stu-id="b6d30-120">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="b6d30-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="b6d30-121">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="b6d30-122">Получение одного пользователя в чате.</span><span class="sxs-lookup"><span data-stu-id="b6d30-122">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="b6d30-123">Список сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="b6d30-123">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="b6d30-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b6d30-124">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="b6d30-125">Получение сообщений в индивидуальном или групповом чате.</span><span class="sxs-lookup"><span data-stu-id="b6d30-125">Get messages in a 1:1 or group chat.</span></span> | 
|[<span data-ttu-id="b6d30-126">Получение сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="b6d30-126">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="b6d30-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b6d30-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="b6d30-128">Получение одного сообщения в чате.</span><span class="sxs-lookup"><span data-stu-id="b6d30-128">Get a single message in a chat.</span></span> | 
|[<span data-ttu-id="b6d30-129">Получение разговора между пользователем и приложением</span><span class="sxs-lookup"><span data-stu-id="b6d30-129">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="b6d30-130">chat</span><span class="sxs-lookup"><span data-stu-id="b6d30-130">chat</span></span>](chat.md)| <span data-ttu-id="b6d30-131">Получение одного сеанса разговора между пользователем и приложением</span><span class="sxs-lookup"><span data-stu-id="b6d30-131">Get one-on-one chat between user and the app</span></span> |

><span data-ttu-id="b6d30-132">**Примечание:** При использовании разрешений приложений необходимо знать, как вы будете получать идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="b6d30-132">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="b6d30-133">Так как перечисление бесед с разрешениями приложений не поддерживается, не все сценарии возможны.</span><span class="sxs-lookup"><span data-stu-id="b6d30-133">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="b6d30-134">Можно получить идентификаторы чата с делегированными разрешениями и из [уведомлений об изменениях для/ЧАТС/жеталлмессажес](../api/subscription-post-subscriptions.md) с разрешениями приложений.</span><span class="sxs-lookup"><span data-stu-id="b6d30-134">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="b6d30-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6d30-135">Properties</span></span>

| <span data-ttu-id="b6d30-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6d30-136">Property</span></span>   | <span data-ttu-id="b6d30-137">Тип</span><span class="sxs-lookup"><span data-stu-id="b6d30-137">Type</span></span> |<span data-ttu-id="b6d30-138">Описание</span><span class="sxs-lookup"><span data-stu-id="b6d30-138">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b6d30-139">id</span><span class="sxs-lookup"><span data-stu-id="b6d30-139">id</span></span>| <span data-ttu-id="b6d30-140">String</span><span class="sxs-lookup"><span data-stu-id="b6d30-140">String</span></span>| <span data-ttu-id="b6d30-141">Уникальный идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="b6d30-141">The chat's unique identifier.</span></span> <span data-ttu-id="b6d30-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6d30-142">Read-only.</span></span>|
| <span data-ttu-id="b6d30-143">topic</span><span class="sxs-lookup"><span data-stu-id="b6d30-143">topic</span></span>| <span data-ttu-id="b6d30-144">String</span><span class="sxs-lookup"><span data-stu-id="b6d30-144">String</span></span>|  <span data-ttu-id="b6d30-145">Необязательно Тема или тема чата.</span><span class="sxs-lookup"><span data-stu-id="b6d30-145">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="b6d30-146">Доступно только для чатов групп.</span><span class="sxs-lookup"><span data-stu-id="b6d30-146">Only available for group chats.</span></span>|
| <span data-ttu-id="b6d30-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6d30-147">createdDateTime</span></span>| <span data-ttu-id="b6d30-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6d30-148">dateTimeOffset</span></span>|  <span data-ttu-id="b6d30-149">Дата и время создания чата.</span><span class="sxs-lookup"><span data-stu-id="b6d30-149">Date and time at which the chat was created.</span></span> <span data-ttu-id="b6d30-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6d30-150">Read-only.</span></span>|
| <span data-ttu-id="b6d30-151">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6d30-151">lastUpdatedDateTime</span></span>| <span data-ttu-id="b6d30-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6d30-152">dateTimeOffset</span></span>|  <span data-ttu-id="b6d30-153">Дата и время переименования чата или изменения членства.</span><span class="sxs-lookup"><span data-stu-id="b6d30-153">Date and time at which the chat was renamed or membership changed.</span></span> <span data-ttu-id="b6d30-154">Ластупдатеддатетиме не обновляется при отправке сообщения в чат.</span><span class="sxs-lookup"><span data-stu-id="b6d30-154">lastUpdatedDateTime is not updated when a message is sent to the chat.</span></span> <span data-ttu-id="b6d30-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6d30-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6d30-156">Связи</span><span class="sxs-lookup"><span data-stu-id="b6d30-156">Relationships</span></span>

| <span data-ttu-id="b6d30-157">Связь</span><span class="sxs-lookup"><span data-stu-id="b6d30-157">Relationship</span></span> | <span data-ttu-id="b6d30-158">Тип</span><span class="sxs-lookup"><span data-stu-id="b6d30-158">Type</span></span> |<span data-ttu-id="b6d30-159">Описание</span><span class="sxs-lookup"><span data-stu-id="b6d30-159">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b6d30-160">installedApps</span><span class="sxs-lookup"><span data-stu-id="b6d30-160">installedApps</span></span> | <span data-ttu-id="b6d30-161">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="b6d30-161">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="b6d30-162">Коллекция всех приложений в чате.</span><span class="sxs-lookup"><span data-stu-id="b6d30-162">A collection of all the apps in the chat.</span></span> <span data-ttu-id="b6d30-163">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b6d30-163">Nullable.</span></span> |
| <span data-ttu-id="b6d30-164">members</span><span class="sxs-lookup"><span data-stu-id="b6d30-164">members</span></span> | <span data-ttu-id="b6d30-165">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="b6d30-165">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="b6d30-166">Коллекция всех людей в чате.</span><span class="sxs-lookup"><span data-stu-id="b6d30-166">A collection of all people in the chat.</span></span> <span data-ttu-id="b6d30-167">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b6d30-167">Nullable.</span></span> |
| <span data-ttu-id="b6d30-168">messages</span><span class="sxs-lookup"><span data-stu-id="b6d30-168">messages</span></span> | <span data-ttu-id="b6d30-169">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="b6d30-169">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="b6d30-170">Коллекция всех сообщений в чате.</span><span class="sxs-lookup"><span data-stu-id="b6d30-170">A collection of all the messages in the chat.</span></span> <span data-ttu-id="b6d30-171">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b6d30-171">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b6d30-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6d30-172">JSON representation</span></span>

<span data-ttu-id="b6d30-173">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6d30-173">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="b6d30-174">См. также</span><span class="sxs-lookup"><span data-stu-id="b6d30-174">See also</span></span>

- [<span data-ttu-id="b6d30-175">channel</span><span class="sxs-lookup"><span data-stu-id="b6d30-175">channel</span></span>](channel.md)
- [<span data-ttu-id="b6d30-176">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b6d30-176">chatMessage</span></span>](chatmessage.md)

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


