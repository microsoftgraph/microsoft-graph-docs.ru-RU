---
title: Тип ресурса Chat
description: Чат — это коллекция chatMessages между одним или несколькими участниками.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7f9cc43442e077dfe245fa8422b954859bf1c569
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564128"
---
# <a name="chat-resource-type"></a><span data-ttu-id="f681c-103">Тип ресурса Chat</span><span class="sxs-lookup"><span data-stu-id="f681c-103">chat resource type</span></span>

<span data-ttu-id="f681c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f681c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f681c-105">Чат — это коллекция [chatMessages](chatmessage.md) между одним или несколькими участниками.</span><span class="sxs-lookup"><span data-stu-id="f681c-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="f681c-106">Участники могут быть пользователями или приложениями.</span><span class="sxs-lookup"><span data-stu-id="f681c-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="f681c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="f681c-107">Methods</span></span>

|  <span data-ttu-id="f681c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="f681c-108">Method</span></span>       |  <span data-ttu-id="f681c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f681c-109">Return Type</span></span>  | <span data-ttu-id="f681c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f681c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f681c-111">Получение разговора между пользователем и приложением</span><span class="sxs-lookup"><span data-stu-id="f681c-111">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="f681c-112">chat</span><span class="sxs-lookup"><span data-stu-id="f681c-112">chat</span></span>](chat.md)| <span data-ttu-id="f681c-113">Получение одного сеанса разговора между пользователем и приложением</span><span class="sxs-lookup"><span data-stu-id="f681c-113">Get one-on-one chat between user and the app</span></span> | 

><span data-ttu-id="f681c-114">**Примечание:** При использовании разрешений приложений необходимо знать, как вы будете получать идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="f681c-114">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="f681c-115">Так как перечисление бесед с разрешениями приложений не поддерживается, не все сценарии возможны.</span><span class="sxs-lookup"><span data-stu-id="f681c-115">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="f681c-116">Можно получить идентификаторы чата с делегированными разрешениями и из [уведомлений об изменениях для/ЧАТС/жеталлмессажес](../api/subscription-post-subscriptions.md) с разрешениями приложений.</span><span class="sxs-lookup"><span data-stu-id="f681c-116">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="f681c-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="f681c-117">Properties</span></span>

| <span data-ttu-id="f681c-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="f681c-118">Property</span></span>   | <span data-ttu-id="f681c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f681c-119">Type</span></span> |<span data-ttu-id="f681c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f681c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f681c-121">id</span><span class="sxs-lookup"><span data-stu-id="f681c-121">id</span></span>| <span data-ttu-id="f681c-122">String</span><span class="sxs-lookup"><span data-stu-id="f681c-122">String</span></span>| <span data-ttu-id="f681c-123">Уникальный идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="f681c-123">The chat's unique identifier.</span></span> <span data-ttu-id="f681c-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f681c-124">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="f681c-125">Связи</span><span class="sxs-lookup"><span data-stu-id="f681c-125">Relationships</span></span>

| <span data-ttu-id="f681c-126">Связь</span><span class="sxs-lookup"><span data-stu-id="f681c-126">Relationship</span></span> | <span data-ttu-id="f681c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f681c-127">Type</span></span> |<span data-ttu-id="f681c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f681c-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f681c-129">messages</span><span class="sxs-lookup"><span data-stu-id="f681c-129">messages</span></span> | <span data-ttu-id="f681c-130">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="f681c-130">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="f681c-131">Коллекция всех сообщений в чате.</span><span class="sxs-lookup"><span data-stu-id="f681c-131">A collection of all the messages in the chat.</span></span> <span data-ttu-id="f681c-132">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f681c-132">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f681c-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f681c-133">JSON representation</span></span>

<span data-ttu-id="f681c-134">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f681c-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chat"
}-->

```json
{
  "id": "string (identifier)",
}
```

## <a name="see-also"></a><span data-ttu-id="f681c-135">См. также</span><span class="sxs-lookup"><span data-stu-id="f681c-135">See also</span></span>

- [<span data-ttu-id="f681c-136">channel</span><span class="sxs-lookup"><span data-stu-id="f681c-136">channel</span></span>](channel.md)
- [<span data-ttu-id="f681c-137">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f681c-137">chatMessage</span></span>](chatmessage.md)

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


