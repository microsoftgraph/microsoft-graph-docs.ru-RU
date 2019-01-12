---
title: Тип ресурса канала
description: 'Канал представляет коллекцию сообщений в группе. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: f513a0c8de51cdfb8ca692098cab403dd74d747a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986350"
---
# <a name="channel-resource-type"></a><span data-ttu-id="1ada4-103">Тип ресурса канала</span><span class="sxs-lookup"><span data-stu-id="1ada4-103">channel resource type</span></span>



<span data-ttu-id="1ada4-104">Канал представляет коллекцию сообщений в пределах [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="1ada4-104">A channel is a collection of messages within a [team](../resources/team.md).</span></span> <span data-ttu-id="1ada4-105">Канал представляет раздел и логическая изоляции обсуждения в группе.</span><span class="sxs-lookup"><span data-stu-id="1ada4-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="1ada4-106">Примеры может быть канала «Пятница Lunch группы» и «Архитектура обсуждений» канала.</span><span class="sxs-lookup"><span data-stu-id="1ada4-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="1ada4-107">Методы</span><span class="sxs-lookup"><span data-stu-id="1ada4-107">Methods</span></span>

| <span data-ttu-id="1ada4-108">Метод</span><span class="sxs-lookup"><span data-stu-id="1ada4-108">Method</span></span>       | <span data-ttu-id="1ada4-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1ada4-109">Return Type</span></span>  |<span data-ttu-id="1ada4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1ada4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1ada4-111">Список каналов</span><span class="sxs-lookup"><span data-stu-id="1ada4-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="1ada4-112">Коллекция [канала](channel.md)</span><span class="sxs-lookup"><span data-stu-id="1ada4-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="1ada4-113">Получите список каналов в данной группы.</span><span class="sxs-lookup"><span data-stu-id="1ada4-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="1ada4-114">Создание канала</span><span class="sxs-lookup"><span data-stu-id="1ada4-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="1ada4-115">канал</span><span class="sxs-lookup"><span data-stu-id="1ada4-115">channel</span></span>](channel.md) | <span data-ttu-id="1ada4-116">Создайте новый канал, включая отображаемое имя и описание.</span><span class="sxs-lookup"><span data-stu-id="1ada4-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="1ada4-117">Получение канала</span><span class="sxs-lookup"><span data-stu-id="1ada4-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="1ada4-118">канал</span><span class="sxs-lookup"><span data-stu-id="1ada4-118">channel</span></span>](channel.md) | <span data-ttu-id="1ada4-119">Чтение свойства и связи канала.</span><span class="sxs-lookup"><span data-stu-id="1ada4-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="1ada4-120">Обновление канала</span><span class="sxs-lookup"><span data-stu-id="1ada4-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="1ada4-121">канал</span><span class="sxs-lookup"><span data-stu-id="1ada4-121">channel</span></span>](channel.md) | <span data-ttu-id="1ada4-122">Обновление свойств канала.</span><span class="sxs-lookup"><span data-stu-id="1ada4-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="1ada4-123">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="1ada4-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="1ada4-124">Нет</span><span class="sxs-lookup"><span data-stu-id="1ada4-124">None</span></span> | <span data-ttu-id="1ada4-125">Удаление канала.</span><span class="sxs-lookup"><span data-stu-id="1ada4-125">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="1ada4-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ada4-126">Properties</span></span>
| <span data-ttu-id="1ada4-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ada4-127">Property</span></span>     | <span data-ttu-id="1ada4-128">Тип</span><span class="sxs-lookup"><span data-stu-id="1ada4-128">Type</span></span>   |<span data-ttu-id="1ada4-129">Описание</span><span class="sxs-lookup"><span data-stu-id="1ada4-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ada4-130">описание</span><span class="sxs-lookup"><span data-stu-id="1ada4-130">description</span></span>|<span data-ttu-id="1ada4-131">Строка</span><span class="sxs-lookup"><span data-stu-id="1ada4-131">String</span></span>|<span data-ttu-id="1ada4-132">Необязательное текстовое описание для канала.</span><span class="sxs-lookup"><span data-stu-id="1ada4-132">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="1ada4-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1ada4-133">displayName</span></span>|<span data-ttu-id="1ada4-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1ada4-134">String</span></span>|<span data-ttu-id="1ada4-135">Имя канала, как оно будет отображаться для пользователей в группах Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1ada4-135">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="1ada4-136">id</span><span class="sxs-lookup"><span data-stu-id="1ada4-136">id</span></span>|<span data-ttu-id="1ada4-137">Строка</span><span class="sxs-lookup"><span data-stu-id="1ada4-137">String</span></span>|<span data-ttu-id="1ada4-138">Уникальный идентификатор, каналов.</span><span class="sxs-lookup"><span data-stu-id="1ada4-138">The channels's unique identifier.</span></span> <span data-ttu-id="1ada4-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1ada4-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ada4-140">Связи</span><span class="sxs-lookup"><span data-stu-id="1ada4-140">Relationships</span></span>
| <span data-ttu-id="1ada4-141">Связь</span><span class="sxs-lookup"><span data-stu-id="1ada4-141">Relationship</span></span> | <span data-ttu-id="1ada4-142">Тип</span><span class="sxs-lookup"><span data-stu-id="1ada4-142">Type</span></span>   |<span data-ttu-id="1ada4-143">Описание</span><span class="sxs-lookup"><span data-stu-id="1ada4-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ada4-144">вкладки</span><span class="sxs-lookup"><span data-stu-id="1ada4-144">tabs</span></span>|<span data-ttu-id="1ada4-145">[teamsTab](../resources/teamstab.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="1ada4-145">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="1ada4-146">Коллекция всех вкладок в канале.</span><span class="sxs-lookup"><span data-stu-id="1ada4-146">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="1ada4-147">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="1ada4-147">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1ada4-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ada4-148">JSON representation</span></span>

<span data-ttu-id="1ada4-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ada4-149">Here is a JSON representation of the resource</span></span>

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
