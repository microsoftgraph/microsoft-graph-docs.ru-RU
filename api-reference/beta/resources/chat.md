---
title: Тип ресурса Chat
description: Чат — это коллекция chatMessages между одним или несколькими участниками.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c536e94230866b209f6d0dffef31bbf23c49b71b
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872805"
---
# <a name="chat-resource-type"></a><span data-ttu-id="462c9-103">Тип ресурса Chat</span><span class="sxs-lookup"><span data-stu-id="462c9-103">chat resource type</span></span>

<span data-ttu-id="462c9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="462c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="462c9-105">Чат — это коллекция [chatMessages](chatmessage.md) между одним или несколькими участниками.</span><span class="sxs-lookup"><span data-stu-id="462c9-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="462c9-106">Участники могут быть пользователями или приложениями.</span><span class="sxs-lookup"><span data-stu-id="462c9-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="462c9-107">Методы</span><span class="sxs-lookup"><span data-stu-id="462c9-107">Methods</span></span>

|  <span data-ttu-id="462c9-108">Метод</span><span class="sxs-lookup"><span data-stu-id="462c9-108">Method</span></span>       |  <span data-ttu-id="462c9-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="462c9-109">Return Type</span></span>  | <span data-ttu-id="462c9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="462c9-110">Description</span></span>| <span data-ttu-id="462c9-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="462c9-111">Permissions</span></span> |
|:---------------|:--------|:----------|-----------|
|[<span data-ttu-id="462c9-112">Список чатов</span><span class="sxs-lookup"><span data-stu-id="462c9-112">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="462c9-113">Коллекция [чата](chat.md)</span><span class="sxs-lookup"><span data-stu-id="462c9-113">[chat](chat.md) collection</span></span> | <span data-ttu-id="462c9-114">Получение списка сеансов, в которые входит пользователь.</span><span class="sxs-lookup"><span data-stu-id="462c9-114">Get the list of chats a user is part of.</span></span>| <span data-ttu-id="462c9-115">**Только делегированные**</span><span class="sxs-lookup"><span data-stu-id="462c9-115">**Delegated only**</span></span> |
|[<span data-ttu-id="462c9-116">Получение чата</span><span class="sxs-lookup"><span data-stu-id="462c9-116">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="462c9-117">chat</span><span class="sxs-lookup"><span data-stu-id="462c9-117">chat</span></span>](chat.md) | <span data-ttu-id="462c9-118">Чтение свойств и связей чата.</span><span class="sxs-lookup"><span data-stu-id="462c9-118">Read properties and relationships of the chat.</span></span>| <span data-ttu-id="462c9-119">**Только делегированные**</span><span class="sxs-lookup"><span data-stu-id="462c9-119">**Delegated only**</span></span> |
|[<span data-ttu-id="462c9-120">Список членов чата</span><span class="sxs-lookup"><span data-stu-id="462c9-120">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="462c9-121">Коллекция [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="462c9-121">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="462c9-122">Получение списка всех пользователей в чате.</span><span class="sxs-lookup"><span data-stu-id="462c9-122">Get the list of all users in the chat.</span></span>| <span data-ttu-id="462c9-123">Делегирование и приложение \*</span><span class="sxs-lookup"><span data-stu-id="462c9-123">Delegated and application\*</span></span> |
|[<span data-ttu-id="462c9-124">Получение члена чата</span><span class="sxs-lookup"><span data-stu-id="462c9-124">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="462c9-125">conversationmember</span><span class="sxs-lookup"><span data-stu-id="462c9-125">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="462c9-126">Получение одного пользователя в чате.</span><span class="sxs-lookup"><span data-stu-id="462c9-126">Get a single user in the chat.</span></span>| <span data-ttu-id="462c9-127">Делегирование и приложение \*</span><span class="sxs-lookup"><span data-stu-id="462c9-127">Delegated and application\*</span></span> |
|[<span data-ttu-id="462c9-128">Список сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="462c9-128">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="462c9-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="462c9-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="462c9-130">Получение сообщений в индивидуальном или групповом чате.</span><span class="sxs-lookup"><span data-stu-id="462c9-130">Get messages in a 1:1 or group chat.</span></span> | <span data-ttu-id="462c9-131">Делегирование и приложение \*</span><span class="sxs-lookup"><span data-stu-id="462c9-131">Delegated and application\*</span></span> |
|[<span data-ttu-id="462c9-132">Получение сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="462c9-132">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="462c9-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="462c9-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="462c9-134">Получение одного сообщения в чате.</span><span class="sxs-lookup"><span data-stu-id="462c9-134">Get a single message in a chat.</span></span> | <span data-ttu-id="462c9-135">Делегирование и приложение \*</span><span class="sxs-lookup"><span data-stu-id="462c9-135">Delegated and application\*</span></span> |

<span data-ttu-id="462c9-136">\*> **Примечание:** При использовании разрешений приложений необходимо знать, как вы будете получать идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="462c9-136">\*> **Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="462c9-137">Так как перечисление бесед с разрешениями приложений не поддерживается, не все сценарии возможны.</span><span class="sxs-lookup"><span data-stu-id="462c9-137">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="462c9-138">Можно получить идентификаторы чата с делегированными разрешениями и из [уведомлений об изменениях для/ЧАТС/аллмессажес](../api/subscription-post-subscriptions.md) с разрешениями приложений.</span><span class="sxs-lookup"><span data-stu-id="462c9-138">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/allMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="462c9-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="462c9-139">Properties</span></span>

| <span data-ttu-id="462c9-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="462c9-140">Property</span></span>   | <span data-ttu-id="462c9-141">Тип</span><span class="sxs-lookup"><span data-stu-id="462c9-141">Type</span></span> |<span data-ttu-id="462c9-142">Описание</span><span class="sxs-lookup"><span data-stu-id="462c9-142">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="462c9-143">id</span><span class="sxs-lookup"><span data-stu-id="462c9-143">id</span></span>| <span data-ttu-id="462c9-144">Строка</span><span class="sxs-lookup"><span data-stu-id="462c9-144">String</span></span>| <span data-ttu-id="462c9-145">Уникальный идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="462c9-145">The chat's unique identifier.</span></span> <span data-ttu-id="462c9-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="462c9-146">Read-only.</span></span>|
| <span data-ttu-id="462c9-147">topic</span><span class="sxs-lookup"><span data-stu-id="462c9-147">topic</span></span>| <span data-ttu-id="462c9-148">String</span><span class="sxs-lookup"><span data-stu-id="462c9-148">String</span></span>|  <span data-ttu-id="462c9-149">Необязательно Тема или тема чата.</span><span class="sxs-lookup"><span data-stu-id="462c9-149">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="462c9-150">Доступно только для чатов групп.</span><span class="sxs-lookup"><span data-stu-id="462c9-150">Only available for group chats.</span></span>|
| <span data-ttu-id="462c9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="462c9-151">createdDateTime</span></span>| <span data-ttu-id="462c9-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="462c9-152">dateTimeOffset</span></span>|  <span data-ttu-id="462c9-153">Дата и время создания чата.</span><span class="sxs-lookup"><span data-stu-id="462c9-153">Date and time at which the chat was created.</span></span> <span data-ttu-id="462c9-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="462c9-154">Read-only.</span></span>|
| <span data-ttu-id="462c9-155">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="462c9-155">lastUpdatedDateTime</span></span>| <span data-ttu-id="462c9-156">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="462c9-156">dateTimeOffset</span></span>|  <span data-ttu-id="462c9-157">Дата и время переименования чата или изменения членства.</span><span class="sxs-lookup"><span data-stu-id="462c9-157">Date and time at which the chat was renamed or membership changed.</span></span> <span data-ttu-id="462c9-158">Ластупдатеддатетиме не обновляется при отправке сообщения в чат.</span><span class="sxs-lookup"><span data-stu-id="462c9-158">lastUpdatedDateTime is not updated when a message is sent to the chat.</span></span> <span data-ttu-id="462c9-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="462c9-159">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="462c9-160">Отношения</span><span class="sxs-lookup"><span data-stu-id="462c9-160">Relationships</span></span>

| <span data-ttu-id="462c9-161">Связь</span><span class="sxs-lookup"><span data-stu-id="462c9-161">Relationship</span></span> | <span data-ttu-id="462c9-162">Тип</span><span class="sxs-lookup"><span data-stu-id="462c9-162">Type</span></span> |<span data-ttu-id="462c9-163">Описание</span><span class="sxs-lookup"><span data-stu-id="462c9-163">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="462c9-164">installedApps</span><span class="sxs-lookup"><span data-stu-id="462c9-164">installedApps</span></span> | <span data-ttu-id="462c9-165">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="462c9-165">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="462c9-166">Коллекция всех приложений в чате.</span><span class="sxs-lookup"><span data-stu-id="462c9-166">A collection of all the apps in the chat.</span></span> <span data-ttu-id="462c9-167">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="462c9-167">Nullable.</span></span> |
| <span data-ttu-id="462c9-168">members</span><span class="sxs-lookup"><span data-stu-id="462c9-168">members</span></span> | <span data-ttu-id="462c9-169">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="462c9-169">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="462c9-170">Коллекция всех людей в чате.</span><span class="sxs-lookup"><span data-stu-id="462c9-170">A collection of all people in the chat.</span></span> <span data-ttu-id="462c9-171">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="462c9-171">Nullable.</span></span> |
| <span data-ttu-id="462c9-172">messages</span><span class="sxs-lookup"><span data-stu-id="462c9-172">messages</span></span> | <span data-ttu-id="462c9-173">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="462c9-173">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="462c9-174">Коллекция всех сообщений в чате.</span><span class="sxs-lookup"><span data-stu-id="462c9-174">A collection of all the messages in the chat.</span></span> <span data-ttu-id="462c9-175">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="462c9-175">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="462c9-176">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="462c9-176">JSON representation</span></span>

<span data-ttu-id="462c9-177">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="462c9-177">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="462c9-178">См. также</span><span class="sxs-lookup"><span data-stu-id="462c9-178">See also</span></span>

- [<span data-ttu-id="462c9-179">channel</span><span class="sxs-lookup"><span data-stu-id="462c9-179">channel</span></span>](channel.md)
- [<span data-ttu-id="462c9-180">chatMessage</span><span class="sxs-lookup"><span data-stu-id="462c9-180">chatMessage</span></span>](chatmessage.md)

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
