---
title: Тип ресурса Chat
description: Чат — это коллекция chatMessages между одним или несколькими участниками.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: da9dcf4a1777d23a3b5f4b73e505641057558605
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48222836"
---
# <a name="chat-resource-type"></a><span data-ttu-id="6d02f-103">Тип ресурса Chat</span><span class="sxs-lookup"><span data-stu-id="6d02f-103">chat resource type</span></span>

<span data-ttu-id="6d02f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d02f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d02f-105">Чат — это коллекция [chatMessages](chatmessage.md) между одним или несколькими участниками.</span><span class="sxs-lookup"><span data-stu-id="6d02f-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="6d02f-106">Участники могут быть пользователями или приложениями.</span><span class="sxs-lookup"><span data-stu-id="6d02f-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="6d02f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6d02f-107">Methods</span></span>

|  <span data-ttu-id="6d02f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="6d02f-108">Method</span></span>       |  <span data-ttu-id="6d02f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6d02f-109">Return Type</span></span>  | <span data-ttu-id="6d02f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6d02f-110">Description</span></span>| <span data-ttu-id="6d02f-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d02f-111">Permissions</span></span> |
|:---------------|:--------|:----------|-----------|
|[<span data-ttu-id="6d02f-112">Список чатов</span><span class="sxs-lookup"><span data-stu-id="6d02f-112">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="6d02f-113">Коллекция [чата](chat.md)</span><span class="sxs-lookup"><span data-stu-id="6d02f-113">[chat](chat.md) collection</span></span> | <span data-ttu-id="6d02f-114">Получение списка сеансов, в которые входит пользователь.</span><span class="sxs-lookup"><span data-stu-id="6d02f-114">Get the list of chats a user is part of.</span></span>| <span data-ttu-id="6d02f-115">**Только делегированные**</span><span class="sxs-lookup"><span data-stu-id="6d02f-115">**Delegated only**</span></span> |
|[<span data-ttu-id="6d02f-116">Получение чата</span><span class="sxs-lookup"><span data-stu-id="6d02f-116">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="6d02f-117">chat</span><span class="sxs-lookup"><span data-stu-id="6d02f-117">chat</span></span>](chat.md) | <span data-ttu-id="6d02f-118">Чтение свойств и связей чата.</span><span class="sxs-lookup"><span data-stu-id="6d02f-118">Read properties and relationships of the chat.</span></span>| <span data-ttu-id="6d02f-119">**Только делегированные**</span><span class="sxs-lookup"><span data-stu-id="6d02f-119">**Delegated only**</span></span> |
|[<span data-ttu-id="6d02f-120">Список членов чата</span><span class="sxs-lookup"><span data-stu-id="6d02f-120">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="6d02f-121">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="6d02f-121">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="6d02f-122">Получение списка всех пользователей в чате.</span><span class="sxs-lookup"><span data-stu-id="6d02f-122">Get the list of all users in the chat.</span></span>| <span data-ttu-id="6d02f-123">Делегирование и приложение \*</span><span class="sxs-lookup"><span data-stu-id="6d02f-123">Delegated and application\*</span></span> |
|[<span data-ttu-id="6d02f-124">Получение члена чата</span><span class="sxs-lookup"><span data-stu-id="6d02f-124">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="6d02f-125">conversationMember</span><span class="sxs-lookup"><span data-stu-id="6d02f-125">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="6d02f-126">Получение одного пользователя в чате.</span><span class="sxs-lookup"><span data-stu-id="6d02f-126">Get a single user in the chat.</span></span>| <span data-ttu-id="6d02f-127">Делегирование и приложение \*</span><span class="sxs-lookup"><span data-stu-id="6d02f-127">Delegated and application\*</span></span> |
|[<span data-ttu-id="6d02f-128">Список сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="6d02f-128">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="6d02f-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6d02f-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="6d02f-130">Получение сообщений в индивидуальном или групповом чате.</span><span class="sxs-lookup"><span data-stu-id="6d02f-130">Get messages in a 1:1 or group chat.</span></span> | <span data-ttu-id="6d02f-131">Делегирование и приложение \*</span><span class="sxs-lookup"><span data-stu-id="6d02f-131">Delegated and application\*</span></span> |
|[<span data-ttu-id="6d02f-132">Получение сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="6d02f-132">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="6d02f-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6d02f-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="6d02f-134">Получение одного сообщения в чате.</span><span class="sxs-lookup"><span data-stu-id="6d02f-134">Get a single message in a chat.</span></span> | <span data-ttu-id="6d02f-135">Делегирование и приложение \*</span><span class="sxs-lookup"><span data-stu-id="6d02f-135">Delegated and application\*</span></span> |

><span data-ttu-id="6d02f-136">**Примечание:** При использовании разрешений приложений необходимо знать, как вы будете получать идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="6d02f-136">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="6d02f-137">Так как перечисление бесед с разрешениями приложений не поддерживается, не все сценарии возможны.</span><span class="sxs-lookup"><span data-stu-id="6d02f-137">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="6d02f-138">Можно получить идентификаторы чата с делегированными разрешениями и из [уведомлений об изменениях для/ЧАТС/жеталлмессажес](../api/subscription-post-subscriptions.md) с разрешениями приложений.</span><span class="sxs-lookup"><span data-stu-id="6d02f-138">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="6d02f-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d02f-139">Properties</span></span>

| <span data-ttu-id="6d02f-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d02f-140">Property</span></span>   | <span data-ttu-id="6d02f-141">Тип</span><span class="sxs-lookup"><span data-stu-id="6d02f-141">Type</span></span> |<span data-ttu-id="6d02f-142">Описание</span><span class="sxs-lookup"><span data-stu-id="6d02f-142">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6d02f-143">id</span><span class="sxs-lookup"><span data-stu-id="6d02f-143">id</span></span>| <span data-ttu-id="6d02f-144">String</span><span class="sxs-lookup"><span data-stu-id="6d02f-144">String</span></span>| <span data-ttu-id="6d02f-145">Уникальный идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="6d02f-145">The chat's unique identifier.</span></span> <span data-ttu-id="6d02f-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6d02f-146">Read-only.</span></span>|
| <span data-ttu-id="6d02f-147">topic</span><span class="sxs-lookup"><span data-stu-id="6d02f-147">topic</span></span>| <span data-ttu-id="6d02f-148">String</span><span class="sxs-lookup"><span data-stu-id="6d02f-148">String</span></span>|  <span data-ttu-id="6d02f-149">Необязательно Тема или тема чата.</span><span class="sxs-lookup"><span data-stu-id="6d02f-149">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="6d02f-150">Доступно только для чатов групп.</span><span class="sxs-lookup"><span data-stu-id="6d02f-150">Only available for group chats.</span></span>|
| <span data-ttu-id="6d02f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d02f-151">createdDateTime</span></span>| <span data-ttu-id="6d02f-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d02f-152">dateTimeOffset</span></span>|  <span data-ttu-id="6d02f-153">Дата и время создания чата.</span><span class="sxs-lookup"><span data-stu-id="6d02f-153">Date and time at which the chat was created.</span></span> <span data-ttu-id="6d02f-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6d02f-154">Read-only.</span></span>|
| <span data-ttu-id="6d02f-155">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d02f-155">lastUpdatedDateTime</span></span>| <span data-ttu-id="6d02f-156">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d02f-156">dateTimeOffset</span></span>|  <span data-ttu-id="6d02f-157">Дата и время переименования чата или изменения членства.</span><span class="sxs-lookup"><span data-stu-id="6d02f-157">Date and time at which the chat was renamed or membership changed.</span></span> <span data-ttu-id="6d02f-158">Ластупдатеддатетиме не обновляется при отправке сообщения в чат.</span><span class="sxs-lookup"><span data-stu-id="6d02f-158">lastUpdatedDateTime is not updated when a message is sent to the chat.</span></span> <span data-ttu-id="6d02f-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6d02f-159">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d02f-160">Связи</span><span class="sxs-lookup"><span data-stu-id="6d02f-160">Relationships</span></span>

| <span data-ttu-id="6d02f-161">Связь</span><span class="sxs-lookup"><span data-stu-id="6d02f-161">Relationship</span></span> | <span data-ttu-id="6d02f-162">Тип</span><span class="sxs-lookup"><span data-stu-id="6d02f-162">Type</span></span> |<span data-ttu-id="6d02f-163">Описание</span><span class="sxs-lookup"><span data-stu-id="6d02f-163">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6d02f-164">installedApps</span><span class="sxs-lookup"><span data-stu-id="6d02f-164">installedApps</span></span> | <span data-ttu-id="6d02f-165">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="6d02f-165">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="6d02f-166">Коллекция всех приложений в чате.</span><span class="sxs-lookup"><span data-stu-id="6d02f-166">A collection of all the apps in the chat.</span></span> <span data-ttu-id="6d02f-167">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6d02f-167">Nullable.</span></span> |
| <span data-ttu-id="6d02f-168">members</span><span class="sxs-lookup"><span data-stu-id="6d02f-168">members</span></span> | <span data-ttu-id="6d02f-169">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="6d02f-169">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="6d02f-170">Коллекция всех людей в чате.</span><span class="sxs-lookup"><span data-stu-id="6d02f-170">A collection of all people in the chat.</span></span> <span data-ttu-id="6d02f-171">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6d02f-171">Nullable.</span></span> |
| <span data-ttu-id="6d02f-172">messages</span><span class="sxs-lookup"><span data-stu-id="6d02f-172">messages</span></span> | <span data-ttu-id="6d02f-173">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="6d02f-173">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="6d02f-174">Коллекция всех сообщений в чате.</span><span class="sxs-lookup"><span data-stu-id="6d02f-174">A collection of all the messages in the chat.</span></span> <span data-ttu-id="6d02f-175">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6d02f-175">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6d02f-176">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d02f-176">JSON representation</span></span>

<span data-ttu-id="6d02f-177">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d02f-177">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="6d02f-178">См. также</span><span class="sxs-lookup"><span data-stu-id="6d02f-178">See also</span></span>

- [<span data-ttu-id="6d02f-179">channel</span><span class="sxs-lookup"><span data-stu-id="6d02f-179">channel</span></span>](channel.md)
- [<span data-ttu-id="6d02f-180">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6d02f-180">chatMessage</span></span>](chatmessage.md)

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


