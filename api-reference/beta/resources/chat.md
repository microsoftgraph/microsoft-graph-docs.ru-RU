---
title: Тип ресурса Chat
description: Чат — это коллекция chatMessages между одним или несколькими участниками.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3fa6952640a1986d0139007ba863275aef2bc6aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507742"
---
# <a name="chat-resource-type"></a><span data-ttu-id="b25fc-103">Тип ресурса Chat</span><span class="sxs-lookup"><span data-stu-id="b25fc-103">chat resource type</span></span>

<span data-ttu-id="b25fc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b25fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b25fc-105">Чат — это коллекция [chatMessages](chatmessage.md) между одним или несколькими участниками.</span><span class="sxs-lookup"><span data-stu-id="b25fc-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="b25fc-106">Участники могут быть пользователями или приложениями.</span><span class="sxs-lookup"><span data-stu-id="b25fc-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="b25fc-107">Методы</span><span class="sxs-lookup"><span data-stu-id="b25fc-107">Methods</span></span>

|  <span data-ttu-id="b25fc-108">Метод</span><span class="sxs-lookup"><span data-stu-id="b25fc-108">Method</span></span>       |  <span data-ttu-id="b25fc-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b25fc-109">Return Type</span></span>  | <span data-ttu-id="b25fc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b25fc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b25fc-111">Список чатов</span><span class="sxs-lookup"><span data-stu-id="b25fc-111">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="b25fc-112">Коллекция [чата](channel.md)</span><span class="sxs-lookup"><span data-stu-id="b25fc-112">[chat](channel.md) collection</span></span> | <span data-ttu-id="b25fc-113">Получение списка сеансов, в которые входит пользователь.</span><span class="sxs-lookup"><span data-stu-id="b25fc-113">Get the list of chats a user is part of.</span></span>|
|[<span data-ttu-id="b25fc-114">Получение чата</span><span class="sxs-lookup"><span data-stu-id="b25fc-114">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="b25fc-115">отображаются</span><span class="sxs-lookup"><span data-stu-id="b25fc-115">chat</span></span>](channel.md) | <span data-ttu-id="b25fc-116">Чтение свойств и связей чата.</span><span class="sxs-lookup"><span data-stu-id="b25fc-116">Read properties and relationships of the chat.</span></span>|
|[<span data-ttu-id="b25fc-117">Список членов чата</span><span class="sxs-lookup"><span data-stu-id="b25fc-117">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="b25fc-118">Коллекция [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="b25fc-118">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="b25fc-119">Получение списка всех пользователей в чате.</span><span class="sxs-lookup"><span data-stu-id="b25fc-119">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="b25fc-120">Получение члена чата</span><span class="sxs-lookup"><span data-stu-id="b25fc-120">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="b25fc-121">conversationmember</span><span class="sxs-lookup"><span data-stu-id="b25fc-121">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="b25fc-122">Получение одного пользователя в чате.</span><span class="sxs-lookup"><span data-stu-id="b25fc-122">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="b25fc-123">Список сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="b25fc-123">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="b25fc-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b25fc-124">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="b25fc-125">Получение сообщений в индивидуальном или групповом чате.</span><span class="sxs-lookup"><span data-stu-id="b25fc-125">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="b25fc-126">Получение сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="b25fc-126">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="b25fc-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b25fc-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="b25fc-128">Получение одного сообщения в чате.</span><span class="sxs-lookup"><span data-stu-id="b25fc-128">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="b25fc-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="b25fc-129">Properties</span></span>

| <span data-ttu-id="b25fc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b25fc-130">Property</span></span>   | <span data-ttu-id="b25fc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b25fc-131">Type</span></span> |<span data-ttu-id="b25fc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b25fc-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b25fc-133">id</span><span class="sxs-lookup"><span data-stu-id="b25fc-133">id</span></span>| <span data-ttu-id="b25fc-134">String</span><span class="sxs-lookup"><span data-stu-id="b25fc-134">String</span></span>| <span data-ttu-id="b25fc-135">Уникальный идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="b25fc-135">The chat's unique identifier.</span></span> <span data-ttu-id="b25fc-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b25fc-136">Read-only.</span></span>|
| <span data-ttu-id="b25fc-137">topic</span><span class="sxs-lookup"><span data-stu-id="b25fc-137">topic</span></span>| <span data-ttu-id="b25fc-138">String</span><span class="sxs-lookup"><span data-stu-id="b25fc-138">String</span></span>|  <span data-ttu-id="b25fc-139">Необязательно Тема или тема чата.</span><span class="sxs-lookup"><span data-stu-id="b25fc-139">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="b25fc-140">Доступно только для чатов групп.</span><span class="sxs-lookup"><span data-stu-id="b25fc-140">Only available for group chats.</span></span>|
| <span data-ttu-id="b25fc-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b25fc-141">createdDateTime</span></span>| <span data-ttu-id="b25fc-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b25fc-142">dateTimeOffset</span></span>|  <span data-ttu-id="b25fc-143">Дата и время создания чата.</span><span class="sxs-lookup"><span data-stu-id="b25fc-143">Date and time at which the chat was created.</span></span> <span data-ttu-id="b25fc-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b25fc-144">Read-only.</span></span>|
| <span data-ttu-id="b25fc-145">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b25fc-145">lastUpdatedDateTime</span></span>| <span data-ttu-id="b25fc-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b25fc-146">dateTimeOffset</span></span>|  <span data-ttu-id="b25fc-147">Дата и время обновления чата.</span><span class="sxs-lookup"><span data-stu-id="b25fc-147">Date and time at which the chat was updated.</span></span> <span data-ttu-id="b25fc-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b25fc-148">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b25fc-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="b25fc-149">Relationships</span></span>

| <span data-ttu-id="b25fc-150">Связь</span><span class="sxs-lookup"><span data-stu-id="b25fc-150">Relationship</span></span> | <span data-ttu-id="b25fc-151">Тип</span><span class="sxs-lookup"><span data-stu-id="b25fc-151">Type</span></span> |<span data-ttu-id="b25fc-152">Описание</span><span class="sxs-lookup"><span data-stu-id="b25fc-152">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b25fc-153">installedApps</span><span class="sxs-lookup"><span data-stu-id="b25fc-153">installedApps</span></span> | <span data-ttu-id="b25fc-154">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="b25fc-154">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="b25fc-155">Коллекция всех приложений в чате.</span><span class="sxs-lookup"><span data-stu-id="b25fc-155">A collection of all the apps in the chat.</span></span> <span data-ttu-id="b25fc-156">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b25fc-156">Nullable.</span></span> |
| <span data-ttu-id="b25fc-157">members</span><span class="sxs-lookup"><span data-stu-id="b25fc-157">members</span></span> | <span data-ttu-id="b25fc-158">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="b25fc-158">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="b25fc-159">Коллекция всех людей в чате.</span><span class="sxs-lookup"><span data-stu-id="b25fc-159">A collection of all people in the chat.</span></span> <span data-ttu-id="b25fc-160">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b25fc-160">Nullable.</span></span> |
| <span data-ttu-id="b25fc-161">messages</span><span class="sxs-lookup"><span data-stu-id="b25fc-161">messages</span></span> | <span data-ttu-id="b25fc-162">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="b25fc-162">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="b25fc-163">Коллекция всех сообщений в чате.</span><span class="sxs-lookup"><span data-stu-id="b25fc-163">A collection of all the messages in the chat.</span></span> <span data-ttu-id="b25fc-164">Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="b25fc-164">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b25fc-165">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b25fc-165">JSON representation</span></span>

<span data-ttu-id="b25fc-166">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b25fc-166">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="b25fc-167">См. также</span><span class="sxs-lookup"><span data-stu-id="b25fc-167">See also</span></span>

- [<span data-ttu-id="b25fc-168">channel</span><span class="sxs-lookup"><span data-stu-id="b25fc-168">channel</span></span>](channel.md)
- [<span data-ttu-id="b25fc-169">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b25fc-169">chatMessage</span></span>](chatmessage.md)

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
