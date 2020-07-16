---
title: Тип ресурса Chat
description: Чат — это коллекция chatMessages между одним или несколькими участниками.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 43ed088889a4b81d59cb9e1361ed978c9cb61141
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864205"
---
# <a name="chat-resource-type"></a><span data-ttu-id="fb484-103">Тип ресурса Chat</span><span class="sxs-lookup"><span data-stu-id="fb484-103">chat resource type</span></span>

<span data-ttu-id="fb484-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb484-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb484-105">Чат — это коллекция [chatMessages](chatmessage.md) между одним или несколькими участниками.</span><span class="sxs-lookup"><span data-stu-id="fb484-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="fb484-106">Участники могут быть пользователями или приложениями.</span><span class="sxs-lookup"><span data-stu-id="fb484-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="fb484-107">Методы</span><span class="sxs-lookup"><span data-stu-id="fb484-107">Methods</span></span>

|  <span data-ttu-id="fb484-108">Метод</span><span class="sxs-lookup"><span data-stu-id="fb484-108">Method</span></span>       |  <span data-ttu-id="fb484-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fb484-109">Return Type</span></span>  | <span data-ttu-id="fb484-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fb484-110">Description</span></span>| <span data-ttu-id="fb484-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb484-111">Permissions</span></span> |
|:---------------|:--------|:----------|-----------|
|[<span data-ttu-id="fb484-112">Список чатов</span><span class="sxs-lookup"><span data-stu-id="fb484-112">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="fb484-113">Коллекция [чата](channel.md)</span><span class="sxs-lookup"><span data-stu-id="fb484-113">[chat](channel.md) collection</span></span> | <span data-ttu-id="fb484-114">Получение списка сеансов, в которые входит пользователь.</span><span class="sxs-lookup"><span data-stu-id="fb484-114">Get the list of chats a user is part of.</span></span>| <span data-ttu-id="fb484-115">**Только делегированные**</span><span class="sxs-lookup"><span data-stu-id="fb484-115">**Delegated only**</span></span> |
|[<span data-ttu-id="fb484-116">Получение чата</span><span class="sxs-lookup"><span data-stu-id="fb484-116">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="fb484-117">отображаются</span><span class="sxs-lookup"><span data-stu-id="fb484-117">chat</span></span>](channel.md) | <span data-ttu-id="fb484-118">Чтение свойств и связей чата.</span><span class="sxs-lookup"><span data-stu-id="fb484-118">Read properties and relationships of the chat.</span></span>| <span data-ttu-id="fb484-119">**Только делегированные**</span><span class="sxs-lookup"><span data-stu-id="fb484-119">**Delegated only**</span></span> |
|[<span data-ttu-id="fb484-120">Список членов чата</span><span class="sxs-lookup"><span data-stu-id="fb484-120">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="fb484-121">Коллекция [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="fb484-121">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="fb484-122">Получение списка всех пользователей в чате.</span><span class="sxs-lookup"><span data-stu-id="fb484-122">Get the list of all users in the chat.</span></span>| <span data-ttu-id="fb484-123">Делегирование и приложение \*</span><span class="sxs-lookup"><span data-stu-id="fb484-123">Delegated and application\*</span></span> |
|[<span data-ttu-id="fb484-124">Получение члена чата</span><span class="sxs-lookup"><span data-stu-id="fb484-124">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="fb484-125">conversationmember</span><span class="sxs-lookup"><span data-stu-id="fb484-125">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="fb484-126">Получение одного пользователя в чате.</span><span class="sxs-lookup"><span data-stu-id="fb484-126">Get a single user in the chat.</span></span>| <span data-ttu-id="fb484-127">Делегирование и приложение \*</span><span class="sxs-lookup"><span data-stu-id="fb484-127">Delegated and application\*</span></span> |
|[<span data-ttu-id="fb484-128">Список сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="fb484-128">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="fb484-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="fb484-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="fb484-130">Получение сообщений в индивидуальном или групповом чате.</span><span class="sxs-lookup"><span data-stu-id="fb484-130">Get messages in a 1:1 or group chat.</span></span> | <span data-ttu-id="fb484-131">Делегирование и приложение \*</span><span class="sxs-lookup"><span data-stu-id="fb484-131">Delegated and application\*</span></span> |
|[<span data-ttu-id="fb484-132">Получение сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="fb484-132">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="fb484-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="fb484-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="fb484-134">Получение одного сообщения в чате.</span><span class="sxs-lookup"><span data-stu-id="fb484-134">Get a single message in a chat.</span></span> | <span data-ttu-id="fb484-135">Делегирование и приложение \*</span><span class="sxs-lookup"><span data-stu-id="fb484-135">Delegated and application\*</span></span> |

<span data-ttu-id="fb484-136">\*> **Примечание:** При использовании разрешений приложений необходимо знать, как вы будете получать идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="fb484-136">\*> **Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="fb484-137">Так как перечисление бесед с разрешениями приложений не поддерживается, не все сценарии возможны.</span><span class="sxs-lookup"><span data-stu-id="fb484-137">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="fb484-138">Можно получить идентификаторы чата с делегированными разрешениями и из [уведомлений об изменениях для/ЧАТС/аллмессажес](../api/subscription-post-subscriptions.md) с разрешениями приложений.</span><span class="sxs-lookup"><span data-stu-id="fb484-138">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/allMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="fb484-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb484-139">Properties</span></span>

| <span data-ttu-id="fb484-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb484-140">Property</span></span>   | <span data-ttu-id="fb484-141">Тип</span><span class="sxs-lookup"><span data-stu-id="fb484-141">Type</span></span> |<span data-ttu-id="fb484-142">Описание</span><span class="sxs-lookup"><span data-stu-id="fb484-142">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fb484-143">id</span><span class="sxs-lookup"><span data-stu-id="fb484-143">id</span></span>| <span data-ttu-id="fb484-144">String</span><span class="sxs-lookup"><span data-stu-id="fb484-144">String</span></span>| <span data-ttu-id="fb484-145">Уникальный идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="fb484-145">The chat's unique identifier.</span></span> <span data-ttu-id="fb484-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb484-146">Read-only.</span></span>|
| <span data-ttu-id="fb484-147">topic</span><span class="sxs-lookup"><span data-stu-id="fb484-147">topic</span></span>| <span data-ttu-id="fb484-148">String</span><span class="sxs-lookup"><span data-stu-id="fb484-148">String</span></span>|  <span data-ttu-id="fb484-149">Необязательно Тема или тема чата.</span><span class="sxs-lookup"><span data-stu-id="fb484-149">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="fb484-150">Доступно только для чатов групп.</span><span class="sxs-lookup"><span data-stu-id="fb484-150">Only available for group chats.</span></span>|
| <span data-ttu-id="fb484-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb484-151">createdDateTime</span></span>| <span data-ttu-id="fb484-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb484-152">dateTimeOffset</span></span>|  <span data-ttu-id="fb484-153">Дата и время создания чата.</span><span class="sxs-lookup"><span data-stu-id="fb484-153">Date and time at which the chat was created.</span></span> <span data-ttu-id="fb484-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb484-154">Read-only.</span></span>|
| <span data-ttu-id="fb484-155">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb484-155">lastUpdatedDateTime</span></span>| <span data-ttu-id="fb484-156">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb484-156">dateTimeOffset</span></span>|  <span data-ttu-id="fb484-157">Дата и время обновления чата.</span><span class="sxs-lookup"><span data-stu-id="fb484-157">Date and time at which the chat was updated.</span></span> <span data-ttu-id="fb484-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb484-158">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb484-159">Отношения</span><span class="sxs-lookup"><span data-stu-id="fb484-159">Relationships</span></span>

| <span data-ttu-id="fb484-160">Связь</span><span class="sxs-lookup"><span data-stu-id="fb484-160">Relationship</span></span> | <span data-ttu-id="fb484-161">Тип</span><span class="sxs-lookup"><span data-stu-id="fb484-161">Type</span></span> |<span data-ttu-id="fb484-162">Описание</span><span class="sxs-lookup"><span data-stu-id="fb484-162">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fb484-163">installedApps</span><span class="sxs-lookup"><span data-stu-id="fb484-163">installedApps</span></span> | <span data-ttu-id="fb484-164">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="fb484-164">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="fb484-165">Коллекция всех приложений в чате.</span><span class="sxs-lookup"><span data-stu-id="fb484-165">A collection of all the apps in the chat.</span></span> <span data-ttu-id="fb484-166">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="fb484-166">Nullable.</span></span> |
| <span data-ttu-id="fb484-167">members</span><span class="sxs-lookup"><span data-stu-id="fb484-167">members</span></span> | <span data-ttu-id="fb484-168">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="fb484-168">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="fb484-169">Коллекция всех людей в чате.</span><span class="sxs-lookup"><span data-stu-id="fb484-169">A collection of all people in the chat.</span></span> <span data-ttu-id="fb484-170">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="fb484-170">Nullable.</span></span> |
| <span data-ttu-id="fb484-171">messages</span><span class="sxs-lookup"><span data-stu-id="fb484-171">messages</span></span> | <span data-ttu-id="fb484-172">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="fb484-172">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="fb484-173">Коллекция всех сообщений в чате.</span><span class="sxs-lookup"><span data-stu-id="fb484-173">A collection of all the messages in the chat.</span></span> <span data-ttu-id="fb484-174">Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="fb484-174">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fb484-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb484-175">JSON representation</span></span>

<span data-ttu-id="fb484-176">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb484-176">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="fb484-177">См. также</span><span class="sxs-lookup"><span data-stu-id="fb484-177">See also</span></span>

- [<span data-ttu-id="fb484-178">channel</span><span class="sxs-lookup"><span data-stu-id="fb484-178">channel</span></span>](channel.md)
- [<span data-ttu-id="fb484-179">chatMessage</span><span class="sxs-lookup"><span data-stu-id="fb484-179">chatMessage</span></span>](chatmessage.md)

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
