---
title: Тип ресурса Chat
description: Чат — это коллекция chatMessages между одним или несколькими участниками.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f1745f987577d94f14f81d79a9f8afb89c1ab793
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606939"
---
# <a name="chat-resource-type"></a><span data-ttu-id="94bf2-103">Тип ресурса Chat</span><span class="sxs-lookup"><span data-stu-id="94bf2-103">chat resource type</span></span>

<span data-ttu-id="94bf2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94bf2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94bf2-105">Чат — это коллекция [chatMessages](chatmessage.md) между одним или несколькими участниками.</span><span class="sxs-lookup"><span data-stu-id="94bf2-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="94bf2-106">Участники могут быть пользователями или приложениями.</span><span class="sxs-lookup"><span data-stu-id="94bf2-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="94bf2-107">Методы</span><span class="sxs-lookup"><span data-stu-id="94bf2-107">Methods</span></span>

|  <span data-ttu-id="94bf2-108">Метод</span><span class="sxs-lookup"><span data-stu-id="94bf2-108">Method</span></span>       |  <span data-ttu-id="94bf2-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="94bf2-109">Return Type</span></span>  | <span data-ttu-id="94bf2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="94bf2-110">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="94bf2-111">Список чатов</span><span class="sxs-lookup"><span data-stu-id="94bf2-111">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="94bf2-112">Коллекция [чата](chat.md)</span><span class="sxs-lookup"><span data-stu-id="94bf2-112">[chat](chat.md) collection</span></span> | <span data-ttu-id="94bf2-113">Получение списка сеансов, в которые входит пользователь.</span><span class="sxs-lookup"><span data-stu-id="94bf2-113">Get the list of chats a user is part of.</span></span>| 
|[<span data-ttu-id="94bf2-114">Получение чата</span><span class="sxs-lookup"><span data-stu-id="94bf2-114">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="94bf2-115">chat</span><span class="sxs-lookup"><span data-stu-id="94bf2-115">chat</span></span>](chat.md) | <span data-ttu-id="94bf2-116">Чтение свойств и связей чата.</span><span class="sxs-lookup"><span data-stu-id="94bf2-116">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="94bf2-117">Список членов чата</span><span class="sxs-lookup"><span data-stu-id="94bf2-117">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="94bf2-118">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="94bf2-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="94bf2-119">Получение списка всех пользователей в чате.</span><span class="sxs-lookup"><span data-stu-id="94bf2-119">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="94bf2-120">Получение члена чата</span><span class="sxs-lookup"><span data-stu-id="94bf2-120">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="94bf2-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="94bf2-121">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="94bf2-122">Получение одного пользователя в чате.</span><span class="sxs-lookup"><span data-stu-id="94bf2-122">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="94bf2-123">Список сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="94bf2-123">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="94bf2-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="94bf2-124">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="94bf2-125">Получение сообщений в индивидуальном или групповом чате.</span><span class="sxs-lookup"><span data-stu-id="94bf2-125">Get messages in a 1:1 or group chat.</span></span> | 
|[<span data-ttu-id="94bf2-126">Получение сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="94bf2-126">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="94bf2-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="94bf2-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="94bf2-128">Получение одного сообщения в чате.</span><span class="sxs-lookup"><span data-stu-id="94bf2-128">Get a single message in a chat.</span></span> | 
|[<span data-ttu-id="94bf2-129">Получение разговора между пользователем и приложением</span><span class="sxs-lookup"><span data-stu-id="94bf2-129">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="94bf2-130">chat</span><span class="sxs-lookup"><span data-stu-id="94bf2-130">chat</span></span>](chat.md)| <span data-ttu-id="94bf2-131">Получение одного сеанса разговора между пользователем и приложением</span><span class="sxs-lookup"><span data-stu-id="94bf2-131">Get one-on-one chat between user and the app</span></span> |
|[<span data-ttu-id="94bf2-132">Получение всех сообщений чата</span><span class="sxs-lookup"><span data-stu-id="94bf2-132">Get all chat messages</span></span>](../api/chats-getallmessages.md)| <span data-ttu-id="94bf2-133">Коллекция [чата](chat.md)</span><span class="sxs-lookup"><span data-stu-id="94bf2-133">[chat](chat.md) collection</span></span>| <span data-ttu-id="94bf2-134">Получение сообщений от всех чатов, в которых пользователь является участником, в том числе беседы в одном месте, групповых чатов и сеансов собраний.</span><span class="sxs-lookup"><span data-stu-id="94bf2-134">Get messages from all chats that a user is a participant in, including one-on-one chats, group chats, and meeting chats.</span></span> |
|[<span data-ttu-id="94bf2-135">Перечисление приложений в чате</span><span class="sxs-lookup"><span data-stu-id="94bf2-135">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="94bf2-136">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="94bf2-136">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="94bf2-137">Список приложений, установленных в чате.</span><span class="sxs-lookup"><span data-stu-id="94bf2-137">List apps installed in a chat.</span></span>|
|[<span data-ttu-id="94bf2-138">Получение приложения в чате</span><span class="sxs-lookup"><span data-stu-id="94bf2-138">Get app in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="94bf2-139">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="94bf2-139">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="94bf2-140">Получение определенного приложения, установленного в чате.</span><span class="sxs-lookup"><span data-stu-id="94bf2-140">Get a specific app installed in a chat.</span></span>|
|[<span data-ttu-id="94bf2-141">Добавление приложения в чат</span><span class="sxs-lookup"><span data-stu-id="94bf2-141">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="94bf2-142">Добавляет (устанавливает) приложение в чат.</span><span class="sxs-lookup"><span data-stu-id="94bf2-142">Adds (installs) an app in a chat.</span></span>|
|[<span data-ttu-id="94bf2-143">Обновление приложения в чате</span><span class="sxs-lookup"><span data-stu-id="94bf2-143">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="94bf2-144">Нет</span><span class="sxs-lookup"><span data-stu-id="94bf2-144">None</span></span> | <span data-ttu-id="94bf2-145">Обновление до последней версии приложения, установленного в чате.</span><span class="sxs-lookup"><span data-stu-id="94bf2-145">Update to the latest version of the app installed in chat.</span></span>|
|[<span data-ttu-id="94bf2-146">Удаление приложения из чата</span><span class="sxs-lookup"><span data-stu-id="94bf2-146">Uninstall app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="94bf2-147">Нет</span><span class="sxs-lookup"><span data-stu-id="94bf2-147">None</span></span> | <span data-ttu-id="94bf2-148">Удаление (удаление) приложения из чата.</span><span class="sxs-lookup"><span data-stu-id="94bf2-148">Remove (uninstall) app from a chat.</span></span>|
|[<span data-ttu-id="94bf2-149">Список вкладок в чате</span><span class="sxs-lookup"><span data-stu-id="94bf2-149">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="94bf2-150">teamsTab</span><span class="sxs-lookup"><span data-stu-id="94bf2-150">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="94bf2-151">Список вкладок, закрепленных в чате.</span><span class="sxs-lookup"><span data-stu-id="94bf2-151">List tabs pinned to a chat.</span></span>|
|[<span data-ttu-id="94bf2-152">Получение вкладки в чате</span><span class="sxs-lookup"><span data-stu-id="94bf2-152">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="94bf2-153">teamsTab</span><span class="sxs-lookup"><span data-stu-id="94bf2-153">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="94bf2-154">Получение определенной вкладки, закрепленной в чате.</span><span class="sxs-lookup"><span data-stu-id="94bf2-154">Get a specific tab pinned to a chat.</span></span>|
|[<span data-ttu-id="94bf2-155">Добавление вкладки в чат</span><span class="sxs-lookup"><span data-stu-id="94bf2-155">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="94bf2-156">teamsTab</span><span class="sxs-lookup"><span data-stu-id="94bf2-156">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="94bf2-157">Добавление вкладки в чат (ПИН-код).</span><span class="sxs-lookup"><span data-stu-id="94bf2-157">Add (pin) a tab to a chat.</span></span>|
|[<span data-ttu-id="94bf2-158">Вкладка "обновление" в чате</span><span class="sxs-lookup"><span data-stu-id="94bf2-158">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="94bf2-159">teamsTab</span><span class="sxs-lookup"><span data-stu-id="94bf2-159">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="94bf2-160">Обновляет свойства вкладки в чате.</span><span class="sxs-lookup"><span data-stu-id="94bf2-160">Updates the properties of a tab in a chat.</span></span>|
|[<span data-ttu-id="94bf2-161">Удаление вкладки из чата</span><span class="sxs-lookup"><span data-stu-id="94bf2-161">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="94bf2-162">Нет</span><span class="sxs-lookup"><span data-stu-id="94bf2-162">None</span></span> | <span data-ttu-id="94bf2-163">Удаление (открепление) вкладки из чата.</span><span class="sxs-lookup"><span data-stu-id="94bf2-163">Remove (unpin) a tab from a chat.</span></span>|

><span data-ttu-id="94bf2-164">**Примечание:** При использовании разрешений приложений необходимо знать, как вы будете получать идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="94bf2-164">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="94bf2-165">Так как перечисление бесед с разрешениями приложений не поддерживается, не все сценарии возможны.</span><span class="sxs-lookup"><span data-stu-id="94bf2-165">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="94bf2-166">Можно получить идентификаторы чата с делегированными разрешениями и из [уведомлений об изменениях для/ЧАТС/жеталлмессажес](../api/subscription-post-subscriptions.md) с разрешениями приложений.</span><span class="sxs-lookup"><span data-stu-id="94bf2-166">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="94bf2-167">Свойства</span><span class="sxs-lookup"><span data-stu-id="94bf2-167">Properties</span></span>

| <span data-ttu-id="94bf2-168">Свойство</span><span class="sxs-lookup"><span data-stu-id="94bf2-168">Property</span></span>   | <span data-ttu-id="94bf2-169">Тип</span><span class="sxs-lookup"><span data-stu-id="94bf2-169">Type</span></span> |<span data-ttu-id="94bf2-170">Описание</span><span class="sxs-lookup"><span data-stu-id="94bf2-170">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="94bf2-171">id</span><span class="sxs-lookup"><span data-stu-id="94bf2-171">id</span></span>| <span data-ttu-id="94bf2-172">String</span><span class="sxs-lookup"><span data-stu-id="94bf2-172">String</span></span>| <span data-ttu-id="94bf2-173">Уникальный идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="94bf2-173">The chat's unique identifier.</span></span> <span data-ttu-id="94bf2-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94bf2-174">Read-only.</span></span>|
| <span data-ttu-id="94bf2-175">topic</span><span class="sxs-lookup"><span data-stu-id="94bf2-175">topic</span></span>| <span data-ttu-id="94bf2-176">String</span><span class="sxs-lookup"><span data-stu-id="94bf2-176">String</span></span>|  <span data-ttu-id="94bf2-177">Необязательно Тема или тема чата.</span><span class="sxs-lookup"><span data-stu-id="94bf2-177">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="94bf2-178">Доступно только для чатов групп.</span><span class="sxs-lookup"><span data-stu-id="94bf2-178">Only available for group chats.</span></span>|
| <span data-ttu-id="94bf2-179">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94bf2-179">createdDateTime</span></span>| <span data-ttu-id="94bf2-180">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94bf2-180">dateTimeOffset</span></span>|  <span data-ttu-id="94bf2-181">Дата и время создания чата.</span><span class="sxs-lookup"><span data-stu-id="94bf2-181">Date and time at which the chat was created.</span></span> <span data-ttu-id="94bf2-182">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94bf2-182">Read-only.</span></span>|
| <span data-ttu-id="94bf2-183">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="94bf2-183">lastUpdatedDateTime</span></span>| <span data-ttu-id="94bf2-184">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94bf2-184">dateTimeOffset</span></span>|  <span data-ttu-id="94bf2-185">Дата и время переименования чата или изменения членства.</span><span class="sxs-lookup"><span data-stu-id="94bf2-185">Date and time at which the chat was renamed or membership changed.</span></span> <span data-ttu-id="94bf2-186">Ластупдатеддатетиме не обновляется при отправке сообщения в чат.</span><span class="sxs-lookup"><span data-stu-id="94bf2-186">lastUpdatedDateTime is not updated when a message is sent to the chat.</span></span> <span data-ttu-id="94bf2-187">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94bf2-187">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94bf2-188">Связи</span><span class="sxs-lookup"><span data-stu-id="94bf2-188">Relationships</span></span>

| <span data-ttu-id="94bf2-189">Связь</span><span class="sxs-lookup"><span data-stu-id="94bf2-189">Relationship</span></span> | <span data-ttu-id="94bf2-190">Тип</span><span class="sxs-lookup"><span data-stu-id="94bf2-190">Type</span></span> |<span data-ttu-id="94bf2-191">Описание</span><span class="sxs-lookup"><span data-stu-id="94bf2-191">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="94bf2-192">installedApps</span><span class="sxs-lookup"><span data-stu-id="94bf2-192">installedApps</span></span> | <span data-ttu-id="94bf2-193">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="94bf2-193">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="94bf2-194">Коллекция всех приложений в чате.</span><span class="sxs-lookup"><span data-stu-id="94bf2-194">A collection of all the apps in the chat.</span></span> <span data-ttu-id="94bf2-195">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="94bf2-195">Nullable.</span></span> |
| <span data-ttu-id="94bf2-196">members</span><span class="sxs-lookup"><span data-stu-id="94bf2-196">members</span></span> | <span data-ttu-id="94bf2-197">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="94bf2-197">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="94bf2-198">Коллекция всех людей в чате.</span><span class="sxs-lookup"><span data-stu-id="94bf2-198">A collection of all people in the chat.</span></span> <span data-ttu-id="94bf2-199">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="94bf2-199">Nullable.</span></span> |
| <span data-ttu-id="94bf2-200">messages</span><span class="sxs-lookup"><span data-stu-id="94bf2-200">messages</span></span> | <span data-ttu-id="94bf2-201">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="94bf2-201">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="94bf2-202">Коллекция всех сообщений в чате.</span><span class="sxs-lookup"><span data-stu-id="94bf2-202">A collection of all the messages in the chat.</span></span> <span data-ttu-id="94bf2-203">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="94bf2-203">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="94bf2-204">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="94bf2-204">JSON representation</span></span>

<span data-ttu-id="94bf2-205">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94bf2-205">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="94bf2-206">См. также</span><span class="sxs-lookup"><span data-stu-id="94bf2-206">See also</span></span>

- [<span data-ttu-id="94bf2-207">channel</span><span class="sxs-lookup"><span data-stu-id="94bf2-207">channel</span></span>](channel.md)
- [<span data-ttu-id="94bf2-208">chatMessage</span><span class="sxs-lookup"><span data-stu-id="94bf2-208">chatMessage</span></span>](chatmessage.md)

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


