---
title: Тип ресурса channel
description: 'Канал — это коллекция сообщений в команде. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f995fa1cb725ae5c0764f349180e7f757a9f423e
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272656"
---
# <a name="channel-resource-type"></a><span data-ttu-id="f3737-103">Тип ресурса channel</span><span class="sxs-lookup"><span data-stu-id="f3737-103">channel resource type</span></span>

<span data-ttu-id="f3737-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3737-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f3737-105">[Команды](../resources/team.md) состоят из каналов, являющихся беседами с сотрудниками.</span><span class="sxs-lookup"><span data-stu-id="f3737-105">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="f3737-106">Каждый канал предназначен для определенной темы, отдела или проекта.</span><span class="sxs-lookup"><span data-stu-id="f3737-106">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="f3737-107">Каналы — это место, где фактически выполняется работа. В них проходят командные обсуждения с помощью текста, аудио и видео, а также выполняется обмен файлами и добавление вкладок.</span><span class="sxs-lookup"><span data-stu-id="f3737-107">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="f3737-108">Методы</span><span class="sxs-lookup"><span data-stu-id="f3737-108">Methods</span></span>

| <span data-ttu-id="f3737-109">Метод</span><span class="sxs-lookup"><span data-stu-id="f3737-109">Method</span></span>       | <span data-ttu-id="f3737-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f3737-110">Return Type</span></span>  |<span data-ttu-id="f3737-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f3737-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f3737-112">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="f3737-112">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="f3737-113">Коллекция [channel](channel.md)</span><span class="sxs-lookup"><span data-stu-id="f3737-113">[channel](channel.md) collection</span></span> | <span data-ttu-id="f3737-114">Получение списка каналов в команде.</span><span class="sxs-lookup"><span data-stu-id="f3737-114">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="f3737-115">Создание канала</span><span class="sxs-lookup"><span data-stu-id="f3737-115">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="f3737-116">channel</span><span class="sxs-lookup"><span data-stu-id="f3737-116">channel</span></span>](channel.md) | <span data-ttu-id="f3737-117">Создание нового канала путем добавления отображаемого имени и описания.</span><span class="sxs-lookup"><span data-stu-id="f3737-117">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="f3737-118">Получение канала</span><span class="sxs-lookup"><span data-stu-id="f3737-118">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="f3737-119">channel</span><span class="sxs-lookup"><span data-stu-id="f3737-119">channel</span></span>](channel.md) | <span data-ttu-id="f3737-120">Чтение свойств и связей канала.</span><span class="sxs-lookup"><span data-stu-id="f3737-120">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="f3737-121">Обновление канала</span><span class="sxs-lookup"><span data-stu-id="f3737-121">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="f3737-122">channel</span><span class="sxs-lookup"><span data-stu-id="f3737-122">channel</span></span>](channel.md) | <span data-ttu-id="f3737-123">Обновление свойств канала.</span><span class="sxs-lookup"><span data-stu-id="f3737-123">Update properties of the channel.</span></span>|
|[<span data-ttu-id="f3737-124">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="f3737-124">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="f3737-125">Нет</span><span class="sxs-lookup"><span data-stu-id="f3737-125">None</span></span> | <span data-ttu-id="f3737-126">Удаление канала.</span><span class="sxs-lookup"><span data-stu-id="f3737-126">Delete a channel.</span></span>|
|[<span data-ttu-id="f3737-127">Перечисление вкладок</span><span class="sxs-lookup"><span data-stu-id="f3737-127">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="f3737-128">teamsTab</span><span class="sxs-lookup"><span data-stu-id="f3737-128">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="f3737-129">Перечисление вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="f3737-129">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="f3737-130">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="f3737-130">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="f3737-131">teamsTab</span><span class="sxs-lookup"><span data-stu-id="f3737-131">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="f3737-132">Чтение вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="f3737-132">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="f3737-133">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="f3737-133">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="f3737-134">teamsTab</span><span class="sxs-lookup"><span data-stu-id="f3737-134">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="f3737-135">Добавление (закрепление) вкладки в канал.</span><span class="sxs-lookup"><span data-stu-id="f3737-135">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="f3737-136">Удаление вкладки</span><span class="sxs-lookup"><span data-stu-id="f3737-136">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="f3737-137">Нет</span><span class="sxs-lookup"><span data-stu-id="f3737-137">None</span></span> | <span data-ttu-id="f3737-138">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="f3737-138">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="f3737-139">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="f3737-139">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="f3737-140">teamsTab</span><span class="sxs-lookup"><span data-stu-id="f3737-140">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="f3737-141">Обновление свойств вкладки.</span><span class="sxs-lookup"><span data-stu-id="f3737-141">Updates the tab properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="f3737-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3737-142">Properties</span></span>

| <span data-ttu-id="f3737-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3737-143">Property</span></span>   | <span data-ttu-id="f3737-144">Тип</span><span class="sxs-lookup"><span data-stu-id="f3737-144">Type</span></span> | <span data-ttu-id="f3737-145">Описание</span><span class="sxs-lookup"><span data-stu-id="f3737-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3737-146">description</span><span class="sxs-lookup"><span data-stu-id="f3737-146">description</span></span>|<span data-ttu-id="f3737-147">String</span><span class="sxs-lookup"><span data-stu-id="f3737-147">String</span></span>|<span data-ttu-id="f3737-148">Необязательное текстовое описание канала.</span><span class="sxs-lookup"><span data-stu-id="f3737-148">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="f3737-149">displayName</span><span class="sxs-lookup"><span data-stu-id="f3737-149">displayName</span></span>|<span data-ttu-id="f3737-150">String</span><span class="sxs-lookup"><span data-stu-id="f3737-150">String</span></span>|<span data-ttu-id="f3737-151">Имя канала, отображаемое для пользователя в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f3737-151">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="f3737-152">email</span><span class="sxs-lookup"><span data-stu-id="f3737-152">email</span></span>|<span data-ttu-id="f3737-153">String</span><span class="sxs-lookup"><span data-stu-id="f3737-153">String</span></span>| <span data-ttu-id="f3737-154">Адрес электронной почты для отправки сообщений в канал.</span><span class="sxs-lookup"><span data-stu-id="f3737-154">The email address for sending messages to the channel.</span></span> <span data-ttu-id="f3737-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3737-155">Read-only.</span></span>|
|<span data-ttu-id="f3737-156">id</span><span class="sxs-lookup"><span data-stu-id="f3737-156">id</span></span>|<span data-ttu-id="f3737-157">String</span><span class="sxs-lookup"><span data-stu-id="f3737-157">String</span></span>|<span data-ttu-id="f3737-158">Уникальный идентификатор канала.</span><span class="sxs-lookup"><span data-stu-id="f3737-158">The channels's unique identifier.</span></span> <span data-ttu-id="f3737-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3737-159">Read-only.</span></span>|
|<span data-ttu-id="f3737-160">webUrl</span><span class="sxs-lookup"><span data-stu-id="f3737-160">webUrl</span></span>|<span data-ttu-id="f3737-161">String</span><span class="sxs-lookup"><span data-stu-id="f3737-161">String</span></span>|<span data-ttu-id="f3737-162">Гиперссылка, ведущая к каналу в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f3737-162">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="f3737-163">Это URL-адрес, получаемый при щелчке правой кнопкой мыши по каналу в Microsoft Teams и выборе пункта "Получить ссылку на канал".</span><span class="sxs-lookup"><span data-stu-id="f3737-163">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="f3737-164">Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться.</span><span class="sxs-lookup"><span data-stu-id="f3737-164">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="f3737-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3737-165">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3737-166">Отношения</span><span class="sxs-lookup"><span data-stu-id="f3737-166">Relationships</span></span>

| <span data-ttu-id="f3737-167">Связь</span><span class="sxs-lookup"><span data-stu-id="f3737-167">Relationship</span></span> | <span data-ttu-id="f3737-168">Тип</span><span class="sxs-lookup"><span data-stu-id="f3737-168">Type</span></span> | <span data-ttu-id="f3737-169">Описание</span><span class="sxs-lookup"><span data-stu-id="f3737-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3737-170">messages</span><span class="sxs-lookup"><span data-stu-id="f3737-170">messages</span></span>|<span data-ttu-id="f3737-171">Коллекция [chatMessage](./chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="f3737-171">[chatMessage](./chatmessage.md) collection</span></span>|<span data-ttu-id="f3737-172">Коллекция всех сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="f3737-172">A collection of all the messages in the channel.</span></span> <span data-ttu-id="f3737-173">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="f3737-173">A navigation property.</span></span> <span data-ttu-id="f3737-174">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f3737-174">Nullable.</span></span>|
|<span data-ttu-id="f3737-175">tabs</span><span class="sxs-lookup"><span data-stu-id="f3737-175">tabs</span></span>|<span data-ttu-id="f3737-176">Коллекция [teamsTab](../resources/teamstab.md)</span><span class="sxs-lookup"><span data-stu-id="f3737-176">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="f3737-177">Коллекция всех вкладок в канале.</span><span class="sxs-lookup"><span data-stu-id="f3737-177">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="f3737-178">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="f3737-178">A navigation property.</span></span>|
|<span data-ttu-id="f3737-179">filesFolder</span><span class="sxs-lookup"><span data-stu-id="f3737-179">filesFolder</span></span>|[<span data-ttu-id="f3737-180">driveItem</span><span class="sxs-lookup"><span data-stu-id="f3737-180">driveItem</span></span>](driveitem.md)|<span data-ttu-id="f3737-181">Метаданные для расположения, в котором хранятся файлы канала.</span><span class="sxs-lookup"><span data-stu-id="f3737-181">Metadata for the location where the channel's files are stored.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f3737-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3737-182">JSON representation</span></span>

<span data-ttu-id="f3737-183">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3737-183">Here is a JSON representation of the resource</span></span>

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
