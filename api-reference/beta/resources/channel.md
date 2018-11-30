---
title: Тип ресурса канала
description: 'Канал представляет коллекцию chatMessages в группе. '
ms.openlocfilehash: 90a2c6641a79829e340f2487d7f0381998d2a205
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081958"
---
# <a name="channel-resource-type"></a><span data-ttu-id="26666-103">Тип ресурса канала</span><span class="sxs-lookup"><span data-stu-id="26666-103">channel resource type</span></span>

> <span data-ttu-id="26666-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="26666-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26666-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26666-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="26666-106">Канал представляет коллекцию [chatMessages](chatmessage.md) внутри [групп](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="26666-106">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="26666-107">Канал представляет раздел и логическая изоляции обсуждения в группе.</span><span class="sxs-lookup"><span data-stu-id="26666-107">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="26666-108">Примеры может быть канала «Пятница Lunch группы» и «Архитектура обсуждений» канала.</span><span class="sxs-lookup"><span data-stu-id="26666-108">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="26666-109">Методы</span><span class="sxs-lookup"><span data-stu-id="26666-109">Methods</span></span>

| <span data-ttu-id="26666-110">Метод</span><span class="sxs-lookup"><span data-stu-id="26666-110">Method</span></span>       | <span data-ttu-id="26666-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="26666-111">Return Type</span></span>  |<span data-ttu-id="26666-112">Описание</span><span class="sxs-lookup"><span data-stu-id="26666-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="26666-113">Список каналов</span><span class="sxs-lookup"><span data-stu-id="26666-113">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="26666-114">Коллекция [канала](channel.md)</span><span class="sxs-lookup"><span data-stu-id="26666-114">[channel](channel.md) collection</span></span> | <span data-ttu-id="26666-115">Получите список каналов в данной группы.</span><span class="sxs-lookup"><span data-stu-id="26666-115">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="26666-116">Создание канала</span><span class="sxs-lookup"><span data-stu-id="26666-116">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="26666-117">канал</span><span class="sxs-lookup"><span data-stu-id="26666-117">channel</span></span>](channel.md) | <span data-ttu-id="26666-118">Создайте новый канал, включая отображаемое имя и описание.</span><span class="sxs-lookup"><span data-stu-id="26666-118">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="26666-119">Получение канала</span><span class="sxs-lookup"><span data-stu-id="26666-119">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="26666-120">канал</span><span class="sxs-lookup"><span data-stu-id="26666-120">channel</span></span>](channel.md) | <span data-ttu-id="26666-121">Чтение свойства и связи канала.</span><span class="sxs-lookup"><span data-stu-id="26666-121">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="26666-122">Обновление канала</span><span class="sxs-lookup"><span data-stu-id="26666-122">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="26666-123">канал</span><span class="sxs-lookup"><span data-stu-id="26666-123">channel</span></span>](channel.md) | <span data-ttu-id="26666-124">Обновление свойств канала.</span><span class="sxs-lookup"><span data-stu-id="26666-124">Update properties of the channel.</span></span>|
|[<span data-ttu-id="26666-125">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="26666-125">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="26666-126">Нет</span><span class="sxs-lookup"><span data-stu-id="26666-126">None</span></span> | <span data-ttu-id="26666-127">Удаление канала.</span><span class="sxs-lookup"><span data-stu-id="26666-127">Delete a channel.</span></span>|
|[<span data-ttu-id="26666-128">Список сообщения</span><span class="sxs-lookup"><span data-stu-id="26666-128">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="26666-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="26666-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="26666-130">Получение сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="26666-130">Get messages in a channel</span></span> |
|[<span data-ttu-id="26666-131">Создать поток разговора</span><span class="sxs-lookup"><span data-stu-id="26666-131">Create chat thread</span></span>](../api/channel-post-chatthreads.md) | <span data-ttu-id="26666-132">[chatThread](chatthread.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="26666-132">[chatThread](chatthread.md) collection</span></span>| <span data-ttu-id="26666-133">Создайте поток разговора в указанном канала.</span><span class="sxs-lookup"><span data-stu-id="26666-133">Create a chat thread in the specified channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="26666-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="26666-134">Properties</span></span>
| <span data-ttu-id="26666-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="26666-135">Property</span></span>     | <span data-ttu-id="26666-136">Тип</span><span class="sxs-lookup"><span data-stu-id="26666-136">Type</span></span>   |<span data-ttu-id="26666-137">Описание</span><span class="sxs-lookup"><span data-stu-id="26666-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26666-138">описание</span><span class="sxs-lookup"><span data-stu-id="26666-138">description</span></span>|<span data-ttu-id="26666-139">String</span><span class="sxs-lookup"><span data-stu-id="26666-139">String</span></span>|<span data-ttu-id="26666-140">Необязательное текстовое описание для канала.</span><span class="sxs-lookup"><span data-stu-id="26666-140">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="26666-141">displayName</span><span class="sxs-lookup"><span data-stu-id="26666-141">displayName</span></span>|<span data-ttu-id="26666-142">String</span><span class="sxs-lookup"><span data-stu-id="26666-142">String</span></span>|<span data-ttu-id="26666-143">Имя канала, как оно будет отображаться для пользователей в группах Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="26666-143">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="26666-144">id</span><span class="sxs-lookup"><span data-stu-id="26666-144">id</span></span>|<span data-ttu-id="26666-145">String</span><span class="sxs-lookup"><span data-stu-id="26666-145">String</span></span>|<span data-ttu-id="26666-146">Уникальный идентификатор, каналов.</span><span class="sxs-lookup"><span data-stu-id="26666-146">The channels's unique identifier.</span></span> <span data-ttu-id="26666-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26666-147">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26666-148">Связи</span><span class="sxs-lookup"><span data-stu-id="26666-148">Relationships</span></span>
| <span data-ttu-id="26666-149">Связь</span><span class="sxs-lookup"><span data-stu-id="26666-149">Relationship</span></span> | <span data-ttu-id="26666-150">Тип</span><span class="sxs-lookup"><span data-stu-id="26666-150">Type</span></span>   |<span data-ttu-id="26666-151">Description</span><span class="sxs-lookup"><span data-stu-id="26666-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26666-152">messages</span><span class="sxs-lookup"><span data-stu-id="26666-152">messages</span></span>|<span data-ttu-id="26666-153">[chatMessage](chatmessage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="26666-153">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="26666-154">Коллекция всех сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="26666-154">A collection of all the messages in the channel.</span></span> <span data-ttu-id="26666-155">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="26666-155">A navigation property.</span></span> <span data-ttu-id="26666-156">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="26666-156">Nullable.</span></span> <span data-ttu-id="26666-157">В настоящее время этот интерфейс API только поддерживает чтение, но со временем будут поддерживать сообщения о записи слишком.</span><span class="sxs-lookup"><span data-stu-id="26666-157">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="26666-158">chatThreads</span><span class="sxs-lookup"><span data-stu-id="26666-158">chatThreads</span></span>|<span data-ttu-id="26666-159">[chatThread](chatthread.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="26666-159">[chatThread](chatthread.md) collection</span></span>|<span data-ttu-id="26666-160">(Это постепенно пользу свойства сообщения) chatThreads поддерживает создание новых сообщений, но не чтение сообщений.</span><span class="sxs-lookup"><span data-stu-id="26666-160">(This is being phased out in favor of the messages property) chatThreads supports creating new messages but not reading messages.</span></span> <span data-ttu-id="26666-161">ChatThreads — это свойство навигации, а значение NULL.</span><span class="sxs-lookup"><span data-stu-id="26666-161">ChatThreads is a navigation property, and is Nullable.</span></span>|
|<span data-ttu-id="26666-162">вкладки</span><span class="sxs-lookup"><span data-stu-id="26666-162">tabs</span></span>|<span data-ttu-id="26666-163">[teamsTab](../resources/teamstab.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="26666-163">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="26666-164">Коллекция всех вкладок в канале.</span><span class="sxs-lookup"><span data-stu-id="26666-164">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="26666-165">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="26666-165">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="26666-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26666-166">JSON representation</span></span>

<span data-ttu-id="26666-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26666-167">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
