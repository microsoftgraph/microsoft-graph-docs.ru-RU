---
title: Тип ресурса chat
description: Чат — это коллекция chatMessages между одним или более участниками.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dcfa853f8ba246443f0f5073a4a62fd84f92adc6
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659410"
---
# <a name="chat-resource-type"></a><span data-ttu-id="b845d-103">Тип ресурса chat</span><span class="sxs-lookup"><span data-stu-id="b845d-103">chat resource type</span></span>

<span data-ttu-id="b845d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b845d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b845d-105">Чат — это коллекция [chatMessages](chatmessage.md) между одним или более участниками.</span><span class="sxs-lookup"><span data-stu-id="b845d-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="b845d-106">Участниками могут быть пользователи или приложения.</span><span class="sxs-lookup"><span data-stu-id="b845d-106">Participants can be users or apps.</span></span>

> <span data-ttu-id="b845d-107">**Примечание.** Если чат связан с экземпляром [onlineMeeting,](../resources/onlinemeeting.md) некоторые из перечисленных методов транзитивно влияют на собрание.</span><span class="sxs-lookup"><span data-stu-id="b845d-107">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then some of the listed methods will transitively impact the meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="b845d-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b845d-108">Methods</span></span>

|  <span data-ttu-id="b845d-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b845d-109">Method</span></span>       |  <span data-ttu-id="b845d-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b845d-110">Return Type</span></span>  | <span data-ttu-id="b845d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b845d-111">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="b845d-112">Список чатов</span><span class="sxs-lookup"><span data-stu-id="b845d-112">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="b845d-113">[коллекция chat](chat.md)</span><span class="sxs-lookup"><span data-stu-id="b845d-113">[chat](chat.md) collection</span></span> | <span data-ttu-id="b845d-114">Получите список чатов, в которые входит пользователь.</span><span class="sxs-lookup"><span data-stu-id="b845d-114">Get the list of chats a user is part of.</span></span>| 
|[<span data-ttu-id="b845d-115">Получение чата</span><span class="sxs-lookup"><span data-stu-id="b845d-115">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="b845d-116">chat</span><span class="sxs-lookup"><span data-stu-id="b845d-116">chat</span></span>](chat.md) | <span data-ttu-id="b845d-117">Чтение свойств и связей чата.</span><span class="sxs-lookup"><span data-stu-id="b845d-117">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="b845d-118">Список участников чата</span><span class="sxs-lookup"><span data-stu-id="b845d-118">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="b845d-119">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="b845d-119">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="b845d-120">Получение списка всех пользователей в чате.</span><span class="sxs-lookup"><span data-stu-id="b845d-120">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="b845d-121">Получить участника чата</span><span class="sxs-lookup"><span data-stu-id="b845d-121">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="b845d-122">conversationMember</span><span class="sxs-lookup"><span data-stu-id="b845d-122">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="b845d-123">Получение одного пользователя в чате.</span><span class="sxs-lookup"><span data-stu-id="b845d-123">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="b845d-124">Список сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="b845d-124">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="b845d-125">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b845d-125">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="b845d-126">Получение сообщений в индивидуальном или групповом чате.</span><span class="sxs-lookup"><span data-stu-id="b845d-126">Get messages in a 1:1 or group chat.</span></span> | 
|[<span data-ttu-id="b845d-127">Получение сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="b845d-127">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="b845d-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b845d-128">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="b845d-129">Получение одного сообщения в чате.</span><span class="sxs-lookup"><span data-stu-id="b845d-129">Get a single message in a chat.</span></span> | 
|[<span data-ttu-id="b845d-130">Общение в чате между пользователем и приложением</span><span class="sxs-lookup"><span data-stu-id="b845d-130">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="b845d-131">chat</span><span class="sxs-lookup"><span data-stu-id="b845d-131">chat</span></span>](chat.md)| <span data-ttu-id="b845d-132">Как получить один-на-один чат между пользователем и приложением</span><span class="sxs-lookup"><span data-stu-id="b845d-132">Get one-on-one chat between user and the app</span></span> |
|[<span data-ttu-id="b845d-133">Получить все сообщения чата</span><span class="sxs-lookup"><span data-stu-id="b845d-133">Get all chat messages</span></span>](../api/chats-getallmessages.md)| <span data-ttu-id="b845d-134">[коллекция chat](chat.md)</span><span class="sxs-lookup"><span data-stu-id="b845d-134">[chat](chat.md) collection</span></span>| <span data-ttu-id="b845d-135">Получать сообщения из всех чатов, в которых состоит пользователь, включая чаты с одним пользователем, групповые чаты и чаты собраний.</span><span class="sxs-lookup"><span data-stu-id="b845d-135">Get messages from all chats that a user is a participant in, including one-on-one chats, group chats, and meeting chats.</span></span> |
|[<span data-ttu-id="b845d-136">Список приложений в каталоге</span><span class="sxs-lookup"><span data-stu-id="b845d-136">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="b845d-137">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="b845d-137">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="b845d-138">Список приложений, установленных в чате (и связанном собрании).</span><span class="sxs-lookup"><span data-stu-id="b845d-138">List apps installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="b845d-139">Получить приложение в чате</span><span class="sxs-lookup"><span data-stu-id="b845d-139">Get app in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="b845d-140">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b845d-140">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="b845d-141">Получите определенное приложение, установленное в чате (и связанном собрании).</span><span class="sxs-lookup"><span data-stu-id="b845d-141">Get a specific app installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="b845d-142">Добавление приложения в чате</span><span class="sxs-lookup"><span data-stu-id="b845d-142">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="b845d-143">Добавление (установка) приложения в чате (и связанном собрании).</span><span class="sxs-lookup"><span data-stu-id="b845d-143">Add (install) an app in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="b845d-144">Обновление приложения в чате</span><span class="sxs-lookup"><span data-stu-id="b845d-144">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="b845d-145">Нет</span><span class="sxs-lookup"><span data-stu-id="b845d-145">None</span></span> | <span data-ttu-id="b845d-146">Обновление до последней версии приложения, установленного в чате (и связанном собрании).</span><span class="sxs-lookup"><span data-stu-id="b845d-146">Update to the latest version of the app installed in chat (and associated meeting).</span></span>|
|[<span data-ttu-id="b845d-147">Удалить приложение из чата</span><span class="sxs-lookup"><span data-stu-id="b845d-147">Uninstall app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="b845d-148">Нет</span><span class="sxs-lookup"><span data-stu-id="b845d-148">None</span></span> | <span data-ttu-id="b845d-149">Удаление приложения из чата (и связанного собрания).</span><span class="sxs-lookup"><span data-stu-id="b845d-149">Remove (uninstall) app from a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="b845d-150">Список вкладок в чате</span><span class="sxs-lookup"><span data-stu-id="b845d-150">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="b845d-151">teamsTab</span><span class="sxs-lookup"><span data-stu-id="b845d-151">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="b845d-152">Список вкладок, закрепленных в чате (и связанном собрании).</span><span class="sxs-lookup"><span data-stu-id="b845d-152">List tabs pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="b845d-153">Получить вкладку в чате</span><span class="sxs-lookup"><span data-stu-id="b845d-153">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="b845d-154">teamsTab</span><span class="sxs-lookup"><span data-stu-id="b845d-154">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="b845d-155">Получить определенную вкладку, закрепленную в чате (и связанном собрании).</span><span class="sxs-lookup"><span data-stu-id="b845d-155">Get a specific tab pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="b845d-156">Добавление вкладки в чат</span><span class="sxs-lookup"><span data-stu-id="b845d-156">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="b845d-157">teamsTab</span><span class="sxs-lookup"><span data-stu-id="b845d-157">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="b845d-158">Добавление (закрепление) вкладки в чат (и связанное собрание).</span><span class="sxs-lookup"><span data-stu-id="b845d-158">Add (pin) a tab to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="b845d-159">Вкладка "Обновление" в чате</span><span class="sxs-lookup"><span data-stu-id="b845d-159">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="b845d-160">teamsTab</span><span class="sxs-lookup"><span data-stu-id="b845d-160">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="b845d-161">Обновление свойств вкладки в чате (и связанном собрании).</span><span class="sxs-lookup"><span data-stu-id="b845d-161">Update the properties of a tab in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="b845d-162">Удаление вкладки из чата</span><span class="sxs-lookup"><span data-stu-id="b845d-162">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="b845d-163">Нет</span><span class="sxs-lookup"><span data-stu-id="b845d-163">None</span></span> | <span data-ttu-id="b845d-164">Удалите (открепите) вкладку из чата (и связанного собрания).</span><span class="sxs-lookup"><span data-stu-id="b845d-164">Remove (unpin) a tab from a chat (and associated meeting).</span></span>|

><span data-ttu-id="b845d-165">**Примечание.** При использовании разрешений приложения убедитесь, что вы знаете, как получить ИД чата.</span><span class="sxs-lookup"><span data-stu-id="b845d-165">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="b845d-166">Так как перечисление чатов с разрешениями приложения не поддерживается, не все сценарии возможны.</span><span class="sxs-lookup"><span data-stu-id="b845d-166">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="b845d-167">Можно получить ИД чата с делегными разрешениями и из уведомлений об изменениях [для /chats/getAllMessages с](../api/subscription-post-subscriptions.md) разрешениями приложения.</span><span class="sxs-lookup"><span data-stu-id="b845d-167">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="b845d-168">Свойства</span><span class="sxs-lookup"><span data-stu-id="b845d-168">Properties</span></span>

| <span data-ttu-id="b845d-169">Свойство</span><span class="sxs-lookup"><span data-stu-id="b845d-169">Property</span></span>   | <span data-ttu-id="b845d-170">Тип</span><span class="sxs-lookup"><span data-stu-id="b845d-170">Type</span></span> |<span data-ttu-id="b845d-171">Описание</span><span class="sxs-lookup"><span data-stu-id="b845d-171">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b845d-172">id</span><span class="sxs-lookup"><span data-stu-id="b845d-172">id</span></span>| <span data-ttu-id="b845d-173">String</span><span class="sxs-lookup"><span data-stu-id="b845d-173">String</span></span>| <span data-ttu-id="b845d-174">Уникальный идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="b845d-174">The chat's unique identifier.</span></span> <span data-ttu-id="b845d-175">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b845d-175">Read-only.</span></span>|
| <span data-ttu-id="b845d-176">topic</span><span class="sxs-lookup"><span data-stu-id="b845d-176">topic</span></span>| <span data-ttu-id="b845d-177">String</span><span class="sxs-lookup"><span data-stu-id="b845d-177">String</span></span>|  <span data-ttu-id="b845d-178">(Необязательно) Тема или тема чата.</span><span class="sxs-lookup"><span data-stu-id="b845d-178">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="b845d-179">Доступно только для групповых чатов.</span><span class="sxs-lookup"><span data-stu-id="b845d-179">Only available for group chats.</span></span>|
| <span data-ttu-id="b845d-180">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b845d-180">createdDateTime</span></span>| <span data-ttu-id="b845d-181">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b845d-181">dateTimeOffset</span></span>|  <span data-ttu-id="b845d-182">Дата и время создания чата.</span><span class="sxs-lookup"><span data-stu-id="b845d-182">Date and time at which the chat was created.</span></span> <span data-ttu-id="b845d-183">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b845d-183">Read-only.</span></span>|
| <span data-ttu-id="b845d-184">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b845d-184">lastUpdatedDateTime</span></span>| <span data-ttu-id="b845d-185">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b845d-185">dateTimeOffset</span></span>|  <span data-ttu-id="b845d-186">Дата и время переименования чата или изменения членства.</span><span class="sxs-lookup"><span data-stu-id="b845d-186">Date and time at which the chat was renamed or membership changed.</span></span> <span data-ttu-id="b845d-187">lastUpdatedDateTime не обновляется при отправлении сообщения в чат.</span><span class="sxs-lookup"><span data-stu-id="b845d-187">lastUpdatedDateTime is not updated when a message is sent to the chat.</span></span> <span data-ttu-id="b845d-188">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b845d-188">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b845d-189">Связи</span><span class="sxs-lookup"><span data-stu-id="b845d-189">Relationships</span></span>

| <span data-ttu-id="b845d-190">Связь</span><span class="sxs-lookup"><span data-stu-id="b845d-190">Relationship</span></span> | <span data-ttu-id="b845d-191">Тип</span><span class="sxs-lookup"><span data-stu-id="b845d-191">Type</span></span> |<span data-ttu-id="b845d-192">Описание</span><span class="sxs-lookup"><span data-stu-id="b845d-192">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b845d-193">installedApps</span><span class="sxs-lookup"><span data-stu-id="b845d-193">installedApps</span></span> | <span data-ttu-id="b845d-194">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="b845d-194">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="b845d-195">Коллекция всех приложений в чате.</span><span class="sxs-lookup"><span data-stu-id="b845d-195">A collection of all the apps in the chat.</span></span> <span data-ttu-id="b845d-196">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b845d-196">Nullable.</span></span> |
| <span data-ttu-id="b845d-197">members</span><span class="sxs-lookup"><span data-stu-id="b845d-197">members</span></span> | <span data-ttu-id="b845d-198">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="b845d-198">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="b845d-199">Коллекция всех людей в чате.</span><span class="sxs-lookup"><span data-stu-id="b845d-199">A collection of all people in the chat.</span></span> <span data-ttu-id="b845d-200">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b845d-200">Nullable.</span></span> |
| <span data-ttu-id="b845d-201">messages</span><span class="sxs-lookup"><span data-stu-id="b845d-201">messages</span></span> | <span data-ttu-id="b845d-202">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="b845d-202">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="b845d-203">Коллекция всех сообщений в чате.</span><span class="sxs-lookup"><span data-stu-id="b845d-203">A collection of all the messages in the chat.</span></span> <span data-ttu-id="b845d-204">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b845d-204">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b845d-205">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b845d-205">JSON representation</span></span>

<span data-ttu-id="b845d-206">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b845d-206">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="b845d-207">См. также</span><span class="sxs-lookup"><span data-stu-id="b845d-207">See also</span></span>

- [<span data-ttu-id="b845d-208">channel</span><span class="sxs-lookup"><span data-stu-id="b845d-208">channel</span></span>](channel.md)
- [<span data-ttu-id="b845d-209">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b845d-209">chatMessage</span></span>](chatmessage.md)

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


