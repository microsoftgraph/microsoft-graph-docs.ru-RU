---
title: Тип ресурса channel
description: 'Канал — это коллекция объектов chatMessages в команде. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f78d6e8730e5f8168cbff94fa03dfbf5287dc5ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012991"
---
# <a name="channel-resource-type"></a><span data-ttu-id="4e63e-103">Тип ресурса channel</span><span class="sxs-lookup"><span data-stu-id="4e63e-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e63e-104">[Команды](../resources/team.md) состоят из каналов, являющихся беседами с сотрудниками.</span><span class="sxs-lookup"><span data-stu-id="4e63e-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="4e63e-105">Каждый канал предназначен для определенной темы, отдела или проекта.</span><span class="sxs-lookup"><span data-stu-id="4e63e-105">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="4e63e-106">Каналы — это место, где фактически выполняется работа. В них проходят командные обсуждения с помощью текста, аудио и видео, а также выполняется обмен файлами и добавление вкладок.</span><span class="sxs-lookup"><span data-stu-id="4e63e-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="4e63e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="4e63e-107">Methods</span></span>

| <span data-ttu-id="4e63e-108">Метод</span><span class="sxs-lookup"><span data-stu-id="4e63e-108">Method</span></span>       | <span data-ttu-id="4e63e-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4e63e-109">Return Type</span></span>  |<span data-ttu-id="4e63e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4e63e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4e63e-111">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="4e63e-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="4e63e-112">Коллекция [channel](channel.md)</span><span class="sxs-lookup"><span data-stu-id="4e63e-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="4e63e-113">Получение списка каналов в команде.</span><span class="sxs-lookup"><span data-stu-id="4e63e-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="4e63e-114">Создание канала</span><span class="sxs-lookup"><span data-stu-id="4e63e-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="4e63e-115">channel</span><span class="sxs-lookup"><span data-stu-id="4e63e-115">channel</span></span>](channel.md) | <span data-ttu-id="4e63e-116">Создание нового канала путем добавления отображаемого имени и описания.</span><span class="sxs-lookup"><span data-stu-id="4e63e-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="4e63e-117">Получение канала</span><span class="sxs-lookup"><span data-stu-id="4e63e-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="4e63e-118">channel</span><span class="sxs-lookup"><span data-stu-id="4e63e-118">channel</span></span>](channel.md) | <span data-ttu-id="4e63e-119">Чтение свойств и связей канала.</span><span class="sxs-lookup"><span data-stu-id="4e63e-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="4e63e-120">Обновление канала</span><span class="sxs-lookup"><span data-stu-id="4e63e-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="4e63e-121">channel</span><span class="sxs-lookup"><span data-stu-id="4e63e-121">channel</span></span>](channel.md) | <span data-ttu-id="4e63e-122">Обновление свойств канала.</span><span class="sxs-lookup"><span data-stu-id="4e63e-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="4e63e-123">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="4e63e-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="4e63e-124">Нет</span><span class="sxs-lookup"><span data-stu-id="4e63e-124">None</span></span> | <span data-ttu-id="4e63e-125">Удаление канала.</span><span class="sxs-lookup"><span data-stu-id="4e63e-125">Delete a channel.</span></span>|
|[<span data-ttu-id="4e63e-126">Перечисление сообщений в каналах</span><span class="sxs-lookup"><span data-stu-id="4e63e-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="4e63e-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="4e63e-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="4e63e-128">Получение сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="4e63e-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="4e63e-129">Создание объекта chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="4e63e-129">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="4e63e-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="4e63e-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="4e63e-131">Отправка сообщения в канал.</span><span class="sxs-lookup"><span data-stu-id="4e63e-131">Send a message to a channel</span></span> |
|[<span data-ttu-id="4e63e-132">Создание ответа на chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="4e63e-132">Create chatMessage reply in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="4e63e-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="4e63e-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="4e63e-134">Ответ на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="4e63e-134">Reply to a message in a channel</span></span>|
|[<span data-ttu-id="4e63e-135">Перечисление вкладок</span><span class="sxs-lookup"><span data-stu-id="4e63e-135">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="4e63e-136">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4e63e-136">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4e63e-137">Перечисление вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="4e63e-137">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="4e63e-138">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="4e63e-138">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="4e63e-139">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4e63e-139">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4e63e-140">Чтение вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="4e63e-140">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="4e63e-141">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="4e63e-141">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="4e63e-142">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4e63e-142">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4e63e-143">Добавление (закрепление) вкладки в канал.</span><span class="sxs-lookup"><span data-stu-id="4e63e-143">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="4e63e-144">Удаление вкладки</span><span class="sxs-lookup"><span data-stu-id="4e63e-144">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="4e63e-145">Нет</span><span class="sxs-lookup"><span data-stu-id="4e63e-145">None</span></span> | <span data-ttu-id="4e63e-146">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="4e63e-146">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="4e63e-147">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="4e63e-147">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="4e63e-148">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4e63e-148">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4e63e-149">Обновление свойств вкладки.</span><span class="sxs-lookup"><span data-stu-id="4e63e-149">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="4e63e-150">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e63e-150">Properties</span></span>
| <span data-ttu-id="4e63e-151">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e63e-151">Property</span></span>     | <span data-ttu-id="4e63e-152">Тип</span><span class="sxs-lookup"><span data-stu-id="4e63e-152">Type</span></span>   |<span data-ttu-id="4e63e-153">Описание</span><span class="sxs-lookup"><span data-stu-id="4e63e-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e63e-154">description</span><span class="sxs-lookup"><span data-stu-id="4e63e-154">description</span></span>|<span data-ttu-id="4e63e-155">String</span><span class="sxs-lookup"><span data-stu-id="4e63e-155">String</span></span>|<span data-ttu-id="4e63e-156">Необязательное текстовое описание канала.</span><span class="sxs-lookup"><span data-stu-id="4e63e-156">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="4e63e-157">displayName</span><span class="sxs-lookup"><span data-stu-id="4e63e-157">displayName</span></span>|<span data-ttu-id="4e63e-158">String</span><span class="sxs-lookup"><span data-stu-id="4e63e-158">String</span></span>|<span data-ttu-id="4e63e-159">Имя канала, отображаемое для пользователя в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4e63e-159">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="4e63e-160">id</span><span class="sxs-lookup"><span data-stu-id="4e63e-160">id</span></span>|<span data-ttu-id="4e63e-161">String</span><span class="sxs-lookup"><span data-stu-id="4e63e-161">String</span></span>|<span data-ttu-id="4e63e-162">Уникальный идентификатор канала.</span><span class="sxs-lookup"><span data-stu-id="4e63e-162">The channels's unique identifier.</span></span> <span data-ttu-id="4e63e-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e63e-163">Read-only.</span></span>|
|<span data-ttu-id="4e63e-164">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="4e63e-164">isFavoriteByDefault</span></span>|<span data-ttu-id="4e63e-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e63e-165">Boolean</span></span>|<span data-ttu-id="4e63e-166">Должен ли канал автоматически помечаться как "Избранное" для всех участников команды.</span><span class="sxs-lookup"><span data-stu-id="4e63e-166">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="4e63e-167">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="4e63e-167">Default: `false`.</span></span>|
|<span data-ttu-id="4e63e-168">email</span><span class="sxs-lookup"><span data-stu-id="4e63e-168">email</span></span>|<span data-ttu-id="4e63e-169">String</span><span class="sxs-lookup"><span data-stu-id="4e63e-169">String</span></span>| <span data-ttu-id="4e63e-170">Адрес электронной почты для отправки сообщений в канал.</span><span class="sxs-lookup"><span data-stu-id="4e63e-170">The email address for sending messages to the channel.</span></span> <span data-ttu-id="4e63e-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e63e-171">Read-only.</span></span>|
|<span data-ttu-id="4e63e-172">webUrl</span><span class="sxs-lookup"><span data-stu-id="4e63e-172">webUrl</span></span>|<span data-ttu-id="4e63e-173">String</span><span class="sxs-lookup"><span data-stu-id="4e63e-173">String</span></span>|<span data-ttu-id="4e63e-174">Гиперссылка, ведущая к каналу в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4e63e-174">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="4e63e-175">Это URL-адрес, получаемый при щелчке правой кнопкой мыши по каналу в Microsoft Teams и выборе пункта "Получить ссылку на канал".</span><span class="sxs-lookup"><span data-stu-id="4e63e-175">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="4e63e-176">Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться.</span><span class="sxs-lookup"><span data-stu-id="4e63e-176">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="4e63e-177">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e63e-177">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="4e63e-178">Отношения</span><span class="sxs-lookup"><span data-stu-id="4e63e-178">Relationships</span></span>
| <span data-ttu-id="4e63e-179">Отношение</span><span class="sxs-lookup"><span data-stu-id="4e63e-179">Relationship</span></span> | <span data-ttu-id="4e63e-180">Тип</span><span class="sxs-lookup"><span data-stu-id="4e63e-180">Type</span></span>   |<span data-ttu-id="4e63e-181">Описание</span><span class="sxs-lookup"><span data-stu-id="4e63e-181">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e63e-182">messages</span><span class="sxs-lookup"><span data-stu-id="4e63e-182">messages</span></span>|<span data-ttu-id="4e63e-183">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="4e63e-183">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="4e63e-184">Коллекция всех сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="4e63e-184">A collection of all the messages in the channel.</span></span> <span data-ttu-id="4e63e-185">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="4e63e-185">A navigation property.</span></span> <span data-ttu-id="4e63e-186">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4e63e-186">Nullable.</span></span> <span data-ttu-id="4e63e-187">В настоящее время этот API поддерживает чтение, но в конечном итоге будет также поддерживать написание сообщений.</span><span class="sxs-lookup"><span data-stu-id="4e63e-187">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="4e63e-188">tabs</span><span class="sxs-lookup"><span data-stu-id="4e63e-188">tabs</span></span>|<span data-ttu-id="4e63e-189">Коллекция [teamsTab](../resources/teamstab.md)</span><span class="sxs-lookup"><span data-stu-id="4e63e-189">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="4e63e-190">Коллекция всех вкладок в канале.</span><span class="sxs-lookup"><span data-stu-id="4e63e-190">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="4e63e-191">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="4e63e-191">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4e63e-192">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e63e-192">JSON representation</span></span>

<span data-ttu-id="4e63e-193">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e63e-193">Here is a JSON representation of the resource</span></span>

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
