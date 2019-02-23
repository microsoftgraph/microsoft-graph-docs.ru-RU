---
title: Тип ресурса channel
description: 'Канал — это коллекция сообщений в команде. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 2bebf78e4ad31047289bff77e681c34d92a94abf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163716"
---
# <a name="channel-resource-type"></a><span data-ttu-id="c43a4-103">Тип ресурса channel</span><span class="sxs-lookup"><span data-stu-id="c43a4-103">channel resource type</span></span>



<span data-ttu-id="c43a4-104">Канал — это коллекция сообщений в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="c43a4-104">A channel is a collection of chatMessages within a team.</span></span> <span data-ttu-id="c43a4-105">Канал представляет тему и логически обособляет обсуждение в команде.</span><span class="sxs-lookup"><span data-stu-id="c43a4-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="c43a4-106">Примеры: канал "Пятничный обед команды" и канал "Обсуждение архитектуры".</span><span class="sxs-lookup"><span data-stu-id="c43a4-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="c43a4-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c43a4-107">Methods</span></span>

| <span data-ttu-id="c43a4-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c43a4-108">Method</span></span>       | <span data-ttu-id="c43a4-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c43a4-109">Return Type</span></span>  |<span data-ttu-id="c43a4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c43a4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c43a4-111">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="c43a4-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="c43a4-112">Коллекция [channel](channel.md)</span><span class="sxs-lookup"><span data-stu-id="c43a4-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="c43a4-113">Получение списка каналов в команде.</span><span class="sxs-lookup"><span data-stu-id="c43a4-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="c43a4-114">Создание канала</span><span class="sxs-lookup"><span data-stu-id="c43a4-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="c43a4-115">channel</span><span class="sxs-lookup"><span data-stu-id="c43a4-115">channel</span></span>](channel.md) | <span data-ttu-id="c43a4-116">Создание нового канала путем добавления отображаемого имени и описания.</span><span class="sxs-lookup"><span data-stu-id="c43a4-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="c43a4-117">Получение канала</span><span class="sxs-lookup"><span data-stu-id="c43a4-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="c43a4-118">channel</span><span class="sxs-lookup"><span data-stu-id="c43a4-118">channel</span></span>](channel.md) | <span data-ttu-id="c43a4-119">Чтение свойств и связей канала.</span><span class="sxs-lookup"><span data-stu-id="c43a4-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="c43a4-120">Обновление канала</span><span class="sxs-lookup"><span data-stu-id="c43a4-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="c43a4-121">channel</span><span class="sxs-lookup"><span data-stu-id="c43a4-121">channel</span></span>](channel.md) | <span data-ttu-id="c43a4-122">Обновление свойств канала.</span><span class="sxs-lookup"><span data-stu-id="c43a4-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="c43a4-123">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="c43a4-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="c43a4-124">Нет</span><span class="sxs-lookup"><span data-stu-id="c43a4-124">None</span></span> | <span data-ttu-id="c43a4-125">Удаление канала.</span><span class="sxs-lookup"><span data-stu-id="c43a4-125">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="c43a4-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="c43a4-126">Properties</span></span>
| <span data-ttu-id="c43a4-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="c43a4-127">Property</span></span>     | <span data-ttu-id="c43a4-128">Тип</span><span class="sxs-lookup"><span data-stu-id="c43a4-128">Type</span></span>   |<span data-ttu-id="c43a4-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c43a4-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c43a4-130">description</span><span class="sxs-lookup"><span data-stu-id="c43a4-130">description</span></span>|<span data-ttu-id="c43a4-131">String</span><span class="sxs-lookup"><span data-stu-id="c43a4-131">String</span></span>|<span data-ttu-id="c43a4-132">Необязательное текстовое описание канала.</span><span class="sxs-lookup"><span data-stu-id="c43a4-132">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="c43a4-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c43a4-133">displayName</span></span>|<span data-ttu-id="c43a4-134">String</span><span class="sxs-lookup"><span data-stu-id="c43a4-134">String</span></span>|<span data-ttu-id="c43a4-135">Имя канала, отображаемое для пользователя в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c43a4-135">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="c43a4-136">id</span><span class="sxs-lookup"><span data-stu-id="c43a4-136">id</span></span>|<span data-ttu-id="c43a4-137">String</span><span class="sxs-lookup"><span data-stu-id="c43a4-137">String</span></span>|<span data-ttu-id="c43a4-138">Уникальный идентификатор канала.</span><span class="sxs-lookup"><span data-stu-id="c43a4-138">The channels's unique identifier.</span></span> <span data-ttu-id="c43a4-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c43a4-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c43a4-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="c43a4-140">Relationships</span></span>
| <span data-ttu-id="c43a4-141">Отношение</span><span class="sxs-lookup"><span data-stu-id="c43a4-141">Relationship</span></span> | <span data-ttu-id="c43a4-142">Тип</span><span class="sxs-lookup"><span data-stu-id="c43a4-142">Type</span></span>   |<span data-ttu-id="c43a4-143">Описание</span><span class="sxs-lookup"><span data-stu-id="c43a4-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c43a4-144">tabs</span><span class="sxs-lookup"><span data-stu-id="c43a4-144">tabs</span></span>|<span data-ttu-id="c43a4-145">Коллекция [teamsTab](../resources/teamstab.md)</span><span class="sxs-lookup"><span data-stu-id="c43a4-145">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="c43a4-146">Коллекция всех вкладок в канале.</span><span class="sxs-lookup"><span data-stu-id="c43a4-146">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="c43a4-147">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="c43a4-147">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c43a4-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c43a4-148">JSON representation</span></span>

<span data-ttu-id="c43a4-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c43a4-149">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)"
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
