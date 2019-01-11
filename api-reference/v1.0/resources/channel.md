---
title: Тип ресурса канала
description: 'Канал представляет коллекцию сообщений в группе. '
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 9a7b12646f36152bef17cec2d206e8e84abdcbbe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826567"
---
# <a name="channel-resource-type"></a><span data-ttu-id="0adf2-103">Тип ресурса канала</span><span class="sxs-lookup"><span data-stu-id="0adf2-103">channel resource type</span></span>



<span data-ttu-id="0adf2-104">Канал представляет коллекцию сообщений в пределах [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="0adf2-104">A channel is a collection of messages within a [team](../resources/team.md).</span></span> <span data-ttu-id="0adf2-105">Канал представляет раздел и логическая изоляции обсуждения в группе.</span><span class="sxs-lookup"><span data-stu-id="0adf2-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="0adf2-106">Примеры может быть канала «Пятница Lunch группы» и «Архитектура обсуждений» канала.</span><span class="sxs-lookup"><span data-stu-id="0adf2-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="0adf2-107">Методы</span><span class="sxs-lookup"><span data-stu-id="0adf2-107">Methods</span></span>

| <span data-ttu-id="0adf2-108">Метод</span><span class="sxs-lookup"><span data-stu-id="0adf2-108">Method</span></span>       | <span data-ttu-id="0adf2-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0adf2-109">Return Type</span></span>  |<span data-ttu-id="0adf2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0adf2-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0adf2-111">Список каналов</span><span class="sxs-lookup"><span data-stu-id="0adf2-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="0adf2-112">Коллекция [канала](channel.md)</span><span class="sxs-lookup"><span data-stu-id="0adf2-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="0adf2-113">Получите список каналов в данной группы.</span><span class="sxs-lookup"><span data-stu-id="0adf2-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="0adf2-114">Создание канала</span><span class="sxs-lookup"><span data-stu-id="0adf2-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="0adf2-115">канал</span><span class="sxs-lookup"><span data-stu-id="0adf2-115">channel</span></span>](channel.md) | <span data-ttu-id="0adf2-116">Создайте новый канал, включая отображаемое имя и описание.</span><span class="sxs-lookup"><span data-stu-id="0adf2-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="0adf2-117">Получение канала</span><span class="sxs-lookup"><span data-stu-id="0adf2-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="0adf2-118">канал</span><span class="sxs-lookup"><span data-stu-id="0adf2-118">channel</span></span>](channel.md) | <span data-ttu-id="0adf2-119">Чтение свойства и связи канала.</span><span class="sxs-lookup"><span data-stu-id="0adf2-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="0adf2-120">Обновление канала</span><span class="sxs-lookup"><span data-stu-id="0adf2-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="0adf2-121">канал</span><span class="sxs-lookup"><span data-stu-id="0adf2-121">channel</span></span>](channel.md) | <span data-ttu-id="0adf2-122">Обновление свойств канала.</span><span class="sxs-lookup"><span data-stu-id="0adf2-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="0adf2-123">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="0adf2-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="0adf2-124">Нет</span><span class="sxs-lookup"><span data-stu-id="0adf2-124">None</span></span> | <span data-ttu-id="0adf2-125">Удаление канала.</span><span class="sxs-lookup"><span data-stu-id="0adf2-125">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="0adf2-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="0adf2-126">Properties</span></span>
| <span data-ttu-id="0adf2-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="0adf2-127">Property</span></span>     | <span data-ttu-id="0adf2-128">Тип</span><span class="sxs-lookup"><span data-stu-id="0adf2-128">Type</span></span>   |<span data-ttu-id="0adf2-129">Описание</span><span class="sxs-lookup"><span data-stu-id="0adf2-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0adf2-130">описание</span><span class="sxs-lookup"><span data-stu-id="0adf2-130">description</span></span>|<span data-ttu-id="0adf2-131">Строка</span><span class="sxs-lookup"><span data-stu-id="0adf2-131">String</span></span>|<span data-ttu-id="0adf2-132">Необязательное текстовое описание для канала.</span><span class="sxs-lookup"><span data-stu-id="0adf2-132">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="0adf2-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0adf2-133">displayName</span></span>|<span data-ttu-id="0adf2-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0adf2-134">String</span></span>|<span data-ttu-id="0adf2-135">Имя канала, как оно будет отображаться для пользователей в группах Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="0adf2-135">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="0adf2-136">id</span><span class="sxs-lookup"><span data-stu-id="0adf2-136">id</span></span>|<span data-ttu-id="0adf2-137">Строка</span><span class="sxs-lookup"><span data-stu-id="0adf2-137">String</span></span>|<span data-ttu-id="0adf2-138">Уникальный идентификатор, каналов.</span><span class="sxs-lookup"><span data-stu-id="0adf2-138">The channels's unique identifier.</span></span> <span data-ttu-id="0adf2-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0adf2-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0adf2-140">Связи</span><span class="sxs-lookup"><span data-stu-id="0adf2-140">Relationships</span></span>
| <span data-ttu-id="0adf2-141">Связь</span><span class="sxs-lookup"><span data-stu-id="0adf2-141">Relationship</span></span> | <span data-ttu-id="0adf2-142">Тип</span><span class="sxs-lookup"><span data-stu-id="0adf2-142">Type</span></span>   |<span data-ttu-id="0adf2-143">Описание</span><span class="sxs-lookup"><span data-stu-id="0adf2-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0adf2-144">вкладки</span><span class="sxs-lookup"><span data-stu-id="0adf2-144">tabs</span></span>|<span data-ttu-id="0adf2-145">[teamsTab](../resources/teamstab.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0adf2-145">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="0adf2-146">Коллекция всех вкладок в канале.</span><span class="sxs-lookup"><span data-stu-id="0adf2-146">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="0adf2-147">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="0adf2-147">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0adf2-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0adf2-148">JSON representation</span></span>

<span data-ttu-id="0adf2-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0adf2-149">Here is a JSON representation of the resource</span></span>

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
