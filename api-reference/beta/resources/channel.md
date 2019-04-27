---
title: Тип ресурса channel
description: 'Канал — это коллекция объектов chatMessages в команде. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 1b77afb1560ed451683838a617123db013b71cd6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338763"
---
# <a name="channel-resource-type"></a><span data-ttu-id="5cbc0-103">Тип ресурса channel</span><span class="sxs-lookup"><span data-stu-id="5cbc0-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cbc0-104">[Команды](../resources/team.md) состоят из каналов, являющихся беседами с сотрудниками.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="5cbc0-105">Каждый канал предназначен для определенной темы, отдела или проекта.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-105">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="5cbc0-106">Каналы — это место, где фактически выполняется работа. В них проходят командные обсуждения с помощью текста, аудио и видео, а также выполняется обмен файлами и добавление вкладок.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="5cbc0-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5cbc0-107">Methods</span></span>

| <span data-ttu-id="5cbc0-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5cbc0-108">Method</span></span>       | <span data-ttu-id="5cbc0-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5cbc0-109">Return Type</span></span>  |<span data-ttu-id="5cbc0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5cbc0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5cbc0-111">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="5cbc0-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="5cbc0-112">Коллекция [channel](channel.md)</span><span class="sxs-lookup"><span data-stu-id="5cbc0-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="5cbc0-113">Получение списка каналов в команде.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="5cbc0-114">Создание канала</span><span class="sxs-lookup"><span data-stu-id="5cbc0-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="5cbc0-115">channel</span><span class="sxs-lookup"><span data-stu-id="5cbc0-115">channel</span></span>](channel.md) | <span data-ttu-id="5cbc0-116">Создание нового канала путем добавления отображаемого имени и описания.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="5cbc0-117">Получение канала</span><span class="sxs-lookup"><span data-stu-id="5cbc0-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="5cbc0-118">channel</span><span class="sxs-lookup"><span data-stu-id="5cbc0-118">channel</span></span>](channel.md) | <span data-ttu-id="5cbc0-119">Чтение свойств и связей канала.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="5cbc0-120">Обновление канала</span><span class="sxs-lookup"><span data-stu-id="5cbc0-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="5cbc0-121">channel</span><span class="sxs-lookup"><span data-stu-id="5cbc0-121">channel</span></span>](channel.md) | <span data-ttu-id="5cbc0-122">Обновление свойств канала.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="5cbc0-123">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="5cbc0-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="5cbc0-124">Нет</span><span class="sxs-lookup"><span data-stu-id="5cbc0-124">None</span></span> | <span data-ttu-id="5cbc0-125">Удаление канала.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-125">Delete a channel.</span></span>|
|[<span data-ttu-id="5cbc0-126">Перечисление сообщений в каналах</span><span class="sxs-lookup"><span data-stu-id="5cbc0-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="5cbc0-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="5cbc0-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="5cbc0-128">Получение сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="5cbc0-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="5cbc0-129">Отправка сообщения канала</span><span class="sxs-lookup"><span data-stu-id="5cbc0-129">Send channel message</span></span>](../api/channel-post-chatmessage.md)  | [<span data-ttu-id="5cbc0-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="5cbc0-130">chatMessage</span></span>](../resources/chatmessage.md) | [<span data-ttu-id="5cbc0-131">Отправка сообщения в канал</span><span class="sxs-lookup"><span data-stu-id="5cbc0-131">Send a message to a channel</span></span>](../api/channel-post-chatmessage.md) |
|[<span data-ttu-id="5cbc0-132">Перечисление вкладок</span><span class="sxs-lookup"><span data-stu-id="5cbc0-132">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="5cbc0-133">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5cbc0-133">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="5cbc0-134">Перечисление вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-134">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="5cbc0-135">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="5cbc0-135">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="5cbc0-136">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5cbc0-136">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="5cbc0-137">Чтение вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-137">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="5cbc0-138">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="5cbc0-138">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="5cbc0-139">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5cbc0-139">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="5cbc0-140">Добавление (закрепление) вкладки в канал.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-140">Adds (installs) a tab to a team's channel.</span></span>|
|[<span data-ttu-id="5cbc0-141">Удаление вкладки</span><span class="sxs-lookup"><span data-stu-id="5cbc0-141">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="5cbc0-142">Нет</span><span class="sxs-lookup"><span data-stu-id="5cbc0-142">None</span></span> | <span data-ttu-id="5cbc0-143">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-143">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="5cbc0-144">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="5cbc0-144">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="5cbc0-145">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5cbc0-145">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="5cbc0-146">Обновление свойств вкладки.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-146">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="5cbc0-147">Свойства</span><span class="sxs-lookup"><span data-stu-id="5cbc0-147">Properties</span></span>
| <span data-ttu-id="5cbc0-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cbc0-148">Property</span></span>     | <span data-ttu-id="5cbc0-149">Тип</span><span class="sxs-lookup"><span data-stu-id="5cbc0-149">Type</span></span>   |<span data-ttu-id="5cbc0-150">Описание</span><span class="sxs-lookup"><span data-stu-id="5cbc0-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cbc0-151">description</span><span class="sxs-lookup"><span data-stu-id="5cbc0-151">description</span></span>|<span data-ttu-id="5cbc0-152">String</span><span class="sxs-lookup"><span data-stu-id="5cbc0-152">String</span></span>|<span data-ttu-id="5cbc0-153">Необязательное текстовое описание канала.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-153">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="5cbc0-154">displayName</span><span class="sxs-lookup"><span data-stu-id="5cbc0-154">displayName</span></span>|<span data-ttu-id="5cbc0-155">String</span><span class="sxs-lookup"><span data-stu-id="5cbc0-155">String</span></span>|<span data-ttu-id="5cbc0-156">Имя канала, отображаемое для пользователя в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-156">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="5cbc0-157">id</span><span class="sxs-lookup"><span data-stu-id="5cbc0-157">id</span></span>|<span data-ttu-id="5cbc0-158">String</span><span class="sxs-lookup"><span data-stu-id="5cbc0-158">String</span></span>|<span data-ttu-id="5cbc0-159">Уникальный идентификатор канала.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-159">The channels's unique identifier.</span></span> <span data-ttu-id="5cbc0-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-160">Read-only.</span></span>|
|<span data-ttu-id="5cbc0-161">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="5cbc0-161">isFavoriteByDefault</span></span>|<span data-ttu-id="5cbc0-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="5cbc0-162">Boolean</span></span>|<span data-ttu-id="5cbc0-163">Должен ли канал автоматически помечаться как "Избранное" для всех участников команды.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-163">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="5cbc0-164">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-164">Default: `false`.</span></span>|
|<span data-ttu-id="5cbc0-165">email</span><span class="sxs-lookup"><span data-stu-id="5cbc0-165">email</span></span>|<span data-ttu-id="5cbc0-166">String</span><span class="sxs-lookup"><span data-stu-id="5cbc0-166">String</span></span>| <span data-ttu-id="5cbc0-167">Адрес электронной почты для отправки сообщений в канал.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-167">The email address for sending messages to the channel.</span></span> <span data-ttu-id="5cbc0-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-168">Read-only.</span></span>|
|<span data-ttu-id="5cbc0-169">webUrl</span><span class="sxs-lookup"><span data-stu-id="5cbc0-169">webUrl</span></span>|<span data-ttu-id="5cbc0-170">String</span><span class="sxs-lookup"><span data-stu-id="5cbc0-170">String</span></span>|<span data-ttu-id="5cbc0-171">Гиперссылка, ведущая к каналу в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-171">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="5cbc0-172">Это URL-адрес, получаемый при щелчке правой кнопкой мыши по каналу в Microsoft Teams и выборе пункта "Получить ссылку на канал".</span><span class="sxs-lookup"><span data-stu-id="5cbc0-172">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="5cbc0-173">Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-173">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="5cbc0-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-174">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="5cbc0-175">Отношения</span><span class="sxs-lookup"><span data-stu-id="5cbc0-175">Relationships</span></span>
| <span data-ttu-id="5cbc0-176">Отношение</span><span class="sxs-lookup"><span data-stu-id="5cbc0-176">Relationship</span></span> | <span data-ttu-id="5cbc0-177">Тип</span><span class="sxs-lookup"><span data-stu-id="5cbc0-177">Type</span></span>   |<span data-ttu-id="5cbc0-178">Описание</span><span class="sxs-lookup"><span data-stu-id="5cbc0-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cbc0-179">messages</span><span class="sxs-lookup"><span data-stu-id="5cbc0-179">messages</span></span>|<span data-ttu-id="5cbc0-180">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="5cbc0-180">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="5cbc0-181">Коллекция всех сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-181">A collection of all the messages in the channel.</span></span> <span data-ttu-id="5cbc0-182">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-182">A navigation property.</span></span> <span data-ttu-id="5cbc0-183">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-183">Nullable.</span></span> <span data-ttu-id="5cbc0-184">В настоящее время этот API поддерживает чтение, но в конечном итоге будет также поддерживать написание сообщений.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-184">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="5cbc0-185">tabs</span><span class="sxs-lookup"><span data-stu-id="5cbc0-185">tabs</span></span>|<span data-ttu-id="5cbc0-186">Коллекция [teamsTab](../resources/teamstab.md)</span><span class="sxs-lookup"><span data-stu-id="5cbc0-186">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="5cbc0-187">Коллекция всех вкладок в канале.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-187">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="5cbc0-188">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-188">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5cbc0-189">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5cbc0-189">JSON representation</span></span>

<span data-ttu-id="5cbc0-190">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5cbc0-190">Here is a JSON representation of the resource</span></span>

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
  "webUrl": "string"
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
