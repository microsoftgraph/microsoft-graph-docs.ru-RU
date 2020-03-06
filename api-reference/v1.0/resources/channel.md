---
title: Тип ресурса channel
description: 'Канал — это коллекция сообщений в команде. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4117190df40eb3bcf5a837fdad298cefe5121793
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531932"
---
# <a name="channel-resource-type"></a><span data-ttu-id="e4cc8-103">Тип ресурса channel</span><span class="sxs-lookup"><span data-stu-id="e4cc8-103">channel resource type</span></span>

<span data-ttu-id="e4cc8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4cc8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4cc8-105">[Команды](../resources/team.md) состоят из каналов, являющихся беседами с сотрудниками.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-105">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="e4cc8-106">Каждый канал предназначен для определенной темы, отдела или проекта.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-106">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="e4cc8-107">Каналы — это место, где фактически выполняется работа. В них проходят командные обсуждения с помощью текста, аудио и видео, а также выполняется обмен файлами и добавление вкладок.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-107">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="e4cc8-108">Методы</span><span class="sxs-lookup"><span data-stu-id="e4cc8-108">Methods</span></span>

| <span data-ttu-id="e4cc8-109">Метод</span><span class="sxs-lookup"><span data-stu-id="e4cc8-109">Method</span></span>       | <span data-ttu-id="e4cc8-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e4cc8-110">Return Type</span></span>  |<span data-ttu-id="e4cc8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e4cc8-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e4cc8-112">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="e4cc8-112">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="e4cc8-113">Коллекция [channel](channel.md)</span><span class="sxs-lookup"><span data-stu-id="e4cc8-113">[channel](channel.md) collection</span></span> | <span data-ttu-id="e4cc8-114">Получение списка каналов в команде.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-114">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="e4cc8-115">Создание канала</span><span class="sxs-lookup"><span data-stu-id="e4cc8-115">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="e4cc8-116">channel</span><span class="sxs-lookup"><span data-stu-id="e4cc8-116">channel</span></span>](channel.md) | <span data-ttu-id="e4cc8-117">Создание нового канала путем добавления отображаемого имени и описания.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-117">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="e4cc8-118">Получение канала</span><span class="sxs-lookup"><span data-stu-id="e4cc8-118">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="e4cc8-119">channel</span><span class="sxs-lookup"><span data-stu-id="e4cc8-119">channel</span></span>](channel.md) | <span data-ttu-id="e4cc8-120">Чтение свойств и связей канала.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-120">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="e4cc8-121">Обновление канала</span><span class="sxs-lookup"><span data-stu-id="e4cc8-121">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="e4cc8-122">channel</span><span class="sxs-lookup"><span data-stu-id="e4cc8-122">channel</span></span>](channel.md) | <span data-ttu-id="e4cc8-123">Обновление свойств канала.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-123">Update properties of the channel.</span></span>|
|[<span data-ttu-id="e4cc8-124">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="e4cc8-124">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="e4cc8-125">Нет</span><span class="sxs-lookup"><span data-stu-id="e4cc8-125">None</span></span> | <span data-ttu-id="e4cc8-126">Удаление канала.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-126">Delete a channel.</span></span>|
|[<span data-ttu-id="e4cc8-127">Перечисление вкладок</span><span class="sxs-lookup"><span data-stu-id="e4cc8-127">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="e4cc8-128">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e4cc8-128">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e4cc8-129">Перечисление вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-129">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="e4cc8-130">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="e4cc8-130">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="e4cc8-131">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e4cc8-131">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e4cc8-132">Чтение вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-132">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="e4cc8-133">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="e4cc8-133">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="e4cc8-134">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e4cc8-134">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e4cc8-135">Добавление (закрепление) вкладки в канал.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-135">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="e4cc8-136">Удаление вкладки</span><span class="sxs-lookup"><span data-stu-id="e4cc8-136">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="e4cc8-137">Нет</span><span class="sxs-lookup"><span data-stu-id="e4cc8-137">None</span></span> | <span data-ttu-id="e4cc8-138">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-138">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="e4cc8-139">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="e4cc8-139">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="e4cc8-140">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e4cc8-140">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e4cc8-141">Обновление свойств вкладки.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-141">Updates the tab properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="e4cc8-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4cc8-142">Properties</span></span>
| <span data-ttu-id="e4cc8-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4cc8-143">Property</span></span>     | <span data-ttu-id="e4cc8-144">Тип</span><span class="sxs-lookup"><span data-stu-id="e4cc8-144">Type</span></span>   |<span data-ttu-id="e4cc8-145">Описание</span><span class="sxs-lookup"><span data-stu-id="e4cc8-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4cc8-146">description</span><span class="sxs-lookup"><span data-stu-id="e4cc8-146">description</span></span>|<span data-ttu-id="e4cc8-147">String</span><span class="sxs-lookup"><span data-stu-id="e4cc8-147">String</span></span>|<span data-ttu-id="e4cc8-148">Необязательное текстовое описание канала.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-148">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="e4cc8-149">displayName</span><span class="sxs-lookup"><span data-stu-id="e4cc8-149">displayName</span></span>|<span data-ttu-id="e4cc8-150">String</span><span class="sxs-lookup"><span data-stu-id="e4cc8-150">String</span></span>|<span data-ttu-id="e4cc8-151">Имя канала, отображаемое для пользователя в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-151">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="e4cc8-152">email</span><span class="sxs-lookup"><span data-stu-id="e4cc8-152">email</span></span>|<span data-ttu-id="e4cc8-153">String</span><span class="sxs-lookup"><span data-stu-id="e4cc8-153">String</span></span>| <span data-ttu-id="e4cc8-154">Адрес электронной почты для отправки сообщений в канал.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-154">The email address for sending messages to the channel.</span></span> <span data-ttu-id="e4cc8-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-155">Read-only.</span></span>|
|<span data-ttu-id="e4cc8-156">id</span><span class="sxs-lookup"><span data-stu-id="e4cc8-156">id</span></span>|<span data-ttu-id="e4cc8-157">String</span><span class="sxs-lookup"><span data-stu-id="e4cc8-157">String</span></span>|<span data-ttu-id="e4cc8-158">Уникальный идентификатор канала.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-158">The channels's unique identifier.</span></span> <span data-ttu-id="e4cc8-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-159">Read-only.</span></span>|
|<span data-ttu-id="e4cc8-160">webUrl</span><span class="sxs-lookup"><span data-stu-id="e4cc8-160">webUrl</span></span>|<span data-ttu-id="e4cc8-161">String</span><span class="sxs-lookup"><span data-stu-id="e4cc8-161">String</span></span>|<span data-ttu-id="e4cc8-162">Гиперссылка, ведущая к каналу в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-162">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="e4cc8-163">Это URL-адрес, получаемый при щелчке правой кнопкой мыши по каналу в Microsoft Teams и выборе пункта "Получить ссылку на канал".</span><span class="sxs-lookup"><span data-stu-id="e4cc8-163">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="e4cc8-164">Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-164">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="e4cc8-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-165">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4cc8-166">Отношения</span><span class="sxs-lookup"><span data-stu-id="e4cc8-166">Relationships</span></span>
| <span data-ttu-id="e4cc8-167">Связь</span><span class="sxs-lookup"><span data-stu-id="e4cc8-167">Relationship</span></span> | <span data-ttu-id="e4cc8-168">Тип</span><span class="sxs-lookup"><span data-stu-id="e4cc8-168">Type</span></span>   |<span data-ttu-id="e4cc8-169">Описание</span><span class="sxs-lookup"><span data-stu-id="e4cc8-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4cc8-170">tabs</span><span class="sxs-lookup"><span data-stu-id="e4cc8-170">tabs</span></span>|<span data-ttu-id="e4cc8-171">Коллекция [teamsTab](../resources/teamstab.md)</span><span class="sxs-lookup"><span data-stu-id="e4cc8-171">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="e4cc8-172">Коллекция всех вкладок в канале.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-172">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="e4cc8-173">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-173">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e4cc8-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4cc8-174">JSON representation</span></span>

<span data-ttu-id="e4cc8-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4cc8-175">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "email": "string (identifier)",
  "id": "string",
  "webUrl": "string"
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
