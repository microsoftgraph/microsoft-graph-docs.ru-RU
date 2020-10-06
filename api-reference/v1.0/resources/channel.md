---
title: Тип ресурса channel
description: 'Канал — это коллекция объектов chatMessages в команде. '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f9860f6d1385374258eeed11dd8db4db21ba895c
ms.sourcegitcommit: 39e48ed2d95b142ccf3f40ecc52441458f2745bf
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/06/2020
ms.locfileid: "48364405"
---
# <a name="channel-resource-type"></a><span data-ttu-id="69c77-103">Тип ресурса channel</span><span class="sxs-lookup"><span data-stu-id="69c77-103">channel resource type</span></span>

<span data-ttu-id="69c77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69c77-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69c77-105">[Команды](../resources/team.md) состоят из каналов, являющихся беседами с сотрудниками.</span><span class="sxs-lookup"><span data-stu-id="69c77-105">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="69c77-106">Каждый канал предназначен для определенной темы, отдела или проекта.</span><span class="sxs-lookup"><span data-stu-id="69c77-106">Each channel is dedicated to a specific topic, department, or project.</span></span> <span data-ttu-id="69c77-107">Каналы — это место, где фактически выполняется работа. В них проходят командные обсуждения с помощью текста, аудио и видео, а также выполняется обмен файлами и добавление вкладок.</span><span class="sxs-lookup"><span data-stu-id="69c77-107">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="69c77-108">Методы</span><span class="sxs-lookup"><span data-stu-id="69c77-108">Methods</span></span>

| <span data-ttu-id="69c77-109">Метод</span><span class="sxs-lookup"><span data-stu-id="69c77-109">Method</span></span>       | <span data-ttu-id="69c77-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="69c77-110">Return Type</span></span>  |<span data-ttu-id="69c77-111">Описание</span><span class="sxs-lookup"><span data-stu-id="69c77-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="69c77-112">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="69c77-112">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="69c77-113">Коллекция [channel](channel.md)</span><span class="sxs-lookup"><span data-stu-id="69c77-113">[channel](channel.md) collection</span></span> | <span data-ttu-id="69c77-114">Получение списка каналов в команде.</span><span class="sxs-lookup"><span data-stu-id="69c77-114">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="69c77-115">Создание канала</span><span class="sxs-lookup"><span data-stu-id="69c77-115">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="69c77-116">channel</span><span class="sxs-lookup"><span data-stu-id="69c77-116">channel</span></span>](channel.md) | <span data-ttu-id="69c77-117">Создание нового канала путем добавления отображаемого имени и описания.</span><span class="sxs-lookup"><span data-stu-id="69c77-117">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="69c77-118">Получение канала</span><span class="sxs-lookup"><span data-stu-id="69c77-118">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="69c77-119">channel</span><span class="sxs-lookup"><span data-stu-id="69c77-119">channel</span></span>](channel.md) | <span data-ttu-id="69c77-120">Чтение свойств и связей канала.</span><span class="sxs-lookup"><span data-stu-id="69c77-120">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="69c77-121">Обновление канала</span><span class="sxs-lookup"><span data-stu-id="69c77-121">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="69c77-122">channel</span><span class="sxs-lookup"><span data-stu-id="69c77-122">channel</span></span>](channel.md) | <span data-ttu-id="69c77-123">Обновление свойств канала.</span><span class="sxs-lookup"><span data-stu-id="69c77-123">Update properties of the channel.</span></span>|
|[<span data-ttu-id="69c77-124">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="69c77-124">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="69c77-125">Нет</span><span class="sxs-lookup"><span data-stu-id="69c77-125">None</span></span> | <span data-ttu-id="69c77-126">Удаление канала.</span><span class="sxs-lookup"><span data-stu-id="69c77-126">Delete a channel.</span></span>|
|[<span data-ttu-id="69c77-127">Перечисление вкладок</span><span class="sxs-lookup"><span data-stu-id="69c77-127">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="69c77-128">teamsTab</span><span class="sxs-lookup"><span data-stu-id="69c77-128">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="69c77-129">Перечисление вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="69c77-129">Lists tabs pinned to a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="69c77-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="69c77-130">Properties</span></span>

| <span data-ttu-id="69c77-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="69c77-131">Property</span></span>   | <span data-ttu-id="69c77-132">Тип</span><span class="sxs-lookup"><span data-stu-id="69c77-132">Type</span></span> |<span data-ttu-id="69c77-133">Описание</span><span class="sxs-lookup"><span data-stu-id="69c77-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69c77-134">description</span><span class="sxs-lookup"><span data-stu-id="69c77-134">description</span></span>|<span data-ttu-id="69c77-135">String</span><span class="sxs-lookup"><span data-stu-id="69c77-135">String</span></span>|<span data-ttu-id="69c77-136">Необязательное текстовое описание канала.</span><span class="sxs-lookup"><span data-stu-id="69c77-136">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="69c77-137">displayName</span><span class="sxs-lookup"><span data-stu-id="69c77-137">displayName</span></span>|<span data-ttu-id="69c77-138">String</span><span class="sxs-lookup"><span data-stu-id="69c77-138">String</span></span>|<span data-ttu-id="69c77-139">Имя канала, отображаемое для пользователя в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="69c77-139">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="69c77-140">id</span><span class="sxs-lookup"><span data-stu-id="69c77-140">id</span></span>|<span data-ttu-id="69c77-141">String</span><span class="sxs-lookup"><span data-stu-id="69c77-141">String</span></span>|<span data-ttu-id="69c77-142">Уникальный идентификатор канала.</span><span class="sxs-lookup"><span data-stu-id="69c77-142">The channel's unique identifier.</span></span> <span data-ttu-id="69c77-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69c77-143">Read-only.</span></span>|
|<span data-ttu-id="69c77-144">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="69c77-144">isFavoriteByDefault</span></span>|<span data-ttu-id="69c77-145">Логический</span><span class="sxs-lookup"><span data-stu-id="69c77-145">Boolean</span></span>|<span data-ttu-id="69c77-146">Указывает, должен ли канал автоматически помечаться как "Избранное" для всех участников команды.</span><span class="sxs-lookup"><span data-stu-id="69c77-146">Indicates whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="69c77-147">Задается только программными средствами с помощью [Создания группы](../api/team-post.md).</span><span class="sxs-lookup"><span data-stu-id="69c77-147">Can only be set programmatically with [Create team](../api/team-post.md).</span></span> <span data-ttu-id="69c77-148">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="69c77-148">Default: `false`.</span></span>|
|<span data-ttu-id="69c77-149">email</span><span class="sxs-lookup"><span data-stu-id="69c77-149">email</span></span>|<span data-ttu-id="69c77-150">String</span><span class="sxs-lookup"><span data-stu-id="69c77-150">String</span></span>| <span data-ttu-id="69c77-151">Адрес электронной почты для отправки сообщений в канал.</span><span class="sxs-lookup"><span data-stu-id="69c77-151">The email address for sending messages to the channel.</span></span> <span data-ttu-id="69c77-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69c77-152">Read-only.</span></span>|
|<span data-ttu-id="69c77-153">webUrl</span><span class="sxs-lookup"><span data-stu-id="69c77-153">webUrl</span></span>|<span data-ttu-id="69c77-154">String</span><span class="sxs-lookup"><span data-stu-id="69c77-154">String</span></span>|<span data-ttu-id="69c77-155">Гиперссылка, ведущая к каналу в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="69c77-155">A hyperlink that will go to the channel in Microsoft Teams.</span></span> <span data-ttu-id="69c77-156">Это URL-адрес, получаемый при щелчке правой кнопкой мыши по каналу в Microsoft Teams и выборе пункта "Получить ссылку на канал".</span><span class="sxs-lookup"><span data-stu-id="69c77-156">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="69c77-157">Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться.</span><span class="sxs-lookup"><span data-stu-id="69c77-157">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="69c77-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69c77-158">Read-only.</span></span>|
|<span data-ttu-id="69c77-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69c77-159">createdDateTime</span></span>|<span data-ttu-id="69c77-160">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69c77-160">dateTimeOffset</span></span>|<span data-ttu-id="69c77-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69c77-161">Read only.</span></span> <span data-ttu-id="69c77-162">Метка времени создания канала.</span><span class="sxs-lookup"><span data-stu-id="69c77-162">Timestamp at which the channel was created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69c77-163">Связи</span><span class="sxs-lookup"><span data-stu-id="69c77-163">Relationships</span></span>

| <span data-ttu-id="69c77-164">Связь</span><span class="sxs-lookup"><span data-stu-id="69c77-164">Relationship</span></span> | <span data-ttu-id="69c77-165">Тип</span><span class="sxs-lookup"><span data-stu-id="69c77-165">Type</span></span> |<span data-ttu-id="69c77-166">Описание</span><span class="sxs-lookup"><span data-stu-id="69c77-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69c77-167">messages</span><span class="sxs-lookup"><span data-stu-id="69c77-167">messages</span></span>|<span data-ttu-id="69c77-168">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="69c77-168">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="69c77-169">Коллекция всех сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="69c77-169">A collection of all the messages in the channel.</span></span> <span data-ttu-id="69c77-170">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="69c77-170">A navigation property.</span></span> <span data-ttu-id="69c77-171">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="69c77-171">Nullable.</span></span>|
|<span data-ttu-id="69c77-172">tabs</span><span class="sxs-lookup"><span data-stu-id="69c77-172">tabs</span></span>|<span data-ttu-id="69c77-173">Коллекция [teamsTab](../resources/teamstab.md)</span><span class="sxs-lookup"><span data-stu-id="69c77-173">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="69c77-174">Коллекция всех вкладок в канале.</span><span class="sxs-lookup"><span data-stu-id="69c77-174">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="69c77-175">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="69c77-175">A navigation property.</span></span>|
|[<span data-ttu-id="69c77-176">filesFolder</span><span class="sxs-lookup"><span data-stu-id="69c77-176">filesFolder</span></span>](../api/channel-get-filesfolder.md)|[<span data-ttu-id="69c77-177">driveItem</span><span class="sxs-lookup"><span data-stu-id="69c77-177">driveItem</span></span>](driveitem.md)|<span data-ttu-id="69c77-178">Метаданные для расположения, в котором хранятся файлы канала.</span><span class="sxs-lookup"><span data-stu-id="69c77-178">Metadata for the location where the channel's files are stored.</span></span>|
|<span data-ttu-id="69c77-179">operations</span><span class="sxs-lookup"><span data-stu-id="69c77-179">operations</span></span>|<span data-ttu-id="69c77-180">Коллекция [teamsAsyncOperation](teamsasyncoperation.md)</span><span class="sxs-lookup"><span data-stu-id="69c77-180">[teamsAsyncOperation](teamsasyncoperation.md) collection</span></span>| <span data-ttu-id="69c77-181">Асинхронные операции, которые выполнялись или выполняются для этой команды.</span><span class="sxs-lookup"><span data-stu-id="69c77-181">The async operations that ran or are running on this team.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="69c77-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69c77-182">JSON representation</span></span>

<span data-ttu-id="69c77-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69c77-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messages"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "isFavoriteByDefault": true,
  "email": "string",
  "webUrl": "string",
  "createdDateTime": "string (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
