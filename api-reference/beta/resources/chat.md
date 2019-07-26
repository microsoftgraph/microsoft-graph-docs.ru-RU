---
title: Тип ресурса Chat
description: Чат — это коллекция chatMessages между одним или несколькими участниками.
author: clearab
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 83ab8428fb09a7a2dc0546dcebdf2f409d90d25a
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908497"
---
# <a name="chat-resource-type"></a><span data-ttu-id="8a9a2-103">Тип ресурса Chat</span><span class="sxs-lookup"><span data-stu-id="8a9a2-103">chat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a9a2-104">Чат — это коллекция [chatMessages](chatmessage.md) между одним или несколькими участниками.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-104">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="8a9a2-105">Участники могут быть пользователями или приложениями.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-105">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="8a9a2-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8a9a2-106">Methods</span></span>

|  <span data-ttu-id="8a9a2-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8a9a2-107">Method</span></span>       |  <span data-ttu-id="8a9a2-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8a9a2-108">Return Type</span></span>  | <span data-ttu-id="8a9a2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8a9a2-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8a9a2-110">Список чатов</span><span class="sxs-lookup"><span data-stu-id="8a9a2-110">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="8a9a2-111">Коллекция [чата](channel.md)</span><span class="sxs-lookup"><span data-stu-id="8a9a2-111">[chat](channel.md) collection</span></span> | <span data-ttu-id="8a9a2-112">Получение списка сеансов, в которые входит пользователь.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-112">Get the list of chats a user is part of.</span></span>|
|[<span data-ttu-id="8a9a2-113">Получение чата</span><span class="sxs-lookup"><span data-stu-id="8a9a2-113">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="8a9a2-114">отображаются</span><span class="sxs-lookup"><span data-stu-id="8a9a2-114">chat</span></span>](channel.md) | <span data-ttu-id="8a9a2-115">Чтение свойств и связей чата.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-115">Read properties and relationships of the chat.</span></span>|
|[<span data-ttu-id="8a9a2-116">Список членов чата</span><span class="sxs-lookup"><span data-stu-id="8a9a2-116">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="8a9a2-117">Коллекция [конверсатионмембер](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="8a9a2-117">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="8a9a2-118">Получение списка всех пользователей в чате.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-118">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="8a9a2-119">Получение члена чата</span><span class="sxs-lookup"><span data-stu-id="8a9a2-119">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="8a9a2-120">конверсатионмембер</span><span class="sxs-lookup"><span data-stu-id="8a9a2-120">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="8a9a2-121">Получение одного пользователя в чате.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-121">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="8a9a2-122">Список сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="8a9a2-122">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="8a9a2-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8a9a2-123">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="8a9a2-124">Получение сообщений в индивидуальном или групповом чате.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-124">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="8a9a2-125">Получение сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="8a9a2-125">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="8a9a2-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8a9a2-126">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="8a9a2-127">Получение одного сообщения в чате.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-127">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="8a9a2-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a9a2-128">Properties</span></span>

| <span data-ttu-id="8a9a2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a9a2-129">Property</span></span>   | <span data-ttu-id="8a9a2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8a9a2-130">Type</span></span> |<span data-ttu-id="8a9a2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8a9a2-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8a9a2-132">id</span><span class="sxs-lookup"><span data-stu-id="8a9a2-132">id</span></span>| <span data-ttu-id="8a9a2-133">String</span><span class="sxs-lookup"><span data-stu-id="8a9a2-133">String</span></span>| <span data-ttu-id="8a9a2-134">Уникальный идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-134">The chat's unique identifier.</span></span> <span data-ttu-id="8a9a2-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-135">Read-only.</span></span>|
| <span data-ttu-id="8a9a2-136">topic</span><span class="sxs-lookup"><span data-stu-id="8a9a2-136">topic</span></span>| <span data-ttu-id="8a9a2-137">String</span><span class="sxs-lookup"><span data-stu-id="8a9a2-137">String</span></span>|  <span data-ttu-id="8a9a2-138">Необязательно Тема или тема чата.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-138">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="8a9a2-139">Доступно только для чатов групп.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-139">Only available for group chats.</span></span>|
| <span data-ttu-id="8a9a2-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a9a2-140">createdDateTime</span></span>| <span data-ttu-id="8a9a2-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a9a2-141">dateTimeOffset</span></span>|  <span data-ttu-id="8a9a2-142">Дата и время создания чата.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-142">Date and time at which the chat was created.</span></span> <span data-ttu-id="8a9a2-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-143">Read-only.</span></span>|
| <span data-ttu-id="8a9a2-144">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a9a2-144">lastUpdatedDateTime</span></span>| <span data-ttu-id="8a9a2-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a9a2-145">dateTimeOffset</span></span>|  <span data-ttu-id="8a9a2-146">Дата и время обновления чата.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-146">Date and time at which the chat was updated.</span></span> <span data-ttu-id="8a9a2-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-147">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a9a2-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="8a9a2-148">Relationships</span></span>

| <span data-ttu-id="8a9a2-149">Отношение</span><span class="sxs-lookup"><span data-stu-id="8a9a2-149">Relationship</span></span> | <span data-ttu-id="8a9a2-150">Тип</span><span class="sxs-lookup"><span data-stu-id="8a9a2-150">Type</span></span> |<span data-ttu-id="8a9a2-151">Описание</span><span class="sxs-lookup"><span data-stu-id="8a9a2-151">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8a9a2-152">installedApps</span><span class="sxs-lookup"><span data-stu-id="8a9a2-152">installedApps</span></span> | <span data-ttu-id="8a9a2-153">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="8a9a2-153">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="8a9a2-154">Коллекция всех приложений в чате.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-154">A collection of all the apps in the chat.</span></span> <span data-ttu-id="8a9a2-155">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-155">Nullable.</span></span> |
| <span data-ttu-id="8a9a2-156">members</span><span class="sxs-lookup"><span data-stu-id="8a9a2-156">members</span></span> | <span data-ttu-id="8a9a2-157">Коллекция [конверсатионмембер](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="8a9a2-157">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="8a9a2-158">Коллекция всех людей в чате.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-158">A collection of all people in the chat.</span></span> <span data-ttu-id="8a9a2-159">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-159">Nullable.</span></span> |
| <span data-ttu-id="8a9a2-160">messages</span><span class="sxs-lookup"><span data-stu-id="8a9a2-160">messages</span></span> | <span data-ttu-id="8a9a2-161">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="8a9a2-161">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="8a9a2-162">Коллекция всех сообщений в чате.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-162">A collection of all the messages in the chat.</span></span> <span data-ttu-id="8a9a2-163">Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-163">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8a9a2-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a9a2-164">JSON representation</span></span>

<span data-ttu-id="8a9a2-165">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a9a2-165">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="8a9a2-166">См. также</span><span class="sxs-lookup"><span data-stu-id="8a9a2-166">See also</span></span>

- [<span data-ttu-id="8a9a2-167">channel</span><span class="sxs-lookup"><span data-stu-id="8a9a2-167">channel</span></span>](channel.md)
- [<span data-ttu-id="8a9a2-168">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8a9a2-168">chatMessage</span></span>](chatmessage.md)

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
