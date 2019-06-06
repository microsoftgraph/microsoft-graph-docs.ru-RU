---
title: Тип ресурса channel
description: 'Канал — это коллекция объектов chatMessages в команде. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 8b284cdfef42e9eb3319fc51c17febcf02eba1a1
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2019
ms.locfileid: "34709434"
---
# <a name="channel-resource-type"></a><span data-ttu-id="55659-103">Тип ресурса channel</span><span class="sxs-lookup"><span data-stu-id="55659-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55659-104">[Команды](../resources/team.md) состоят из каналов, являющихся беседами с сотрудниками.</span><span class="sxs-lookup"><span data-stu-id="55659-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="55659-105">Каждый канал предназначен для определенной темы, отдела или проекта.</span><span class="sxs-lookup"><span data-stu-id="55659-105">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="55659-106">Каналы — это место, где фактически выполняется работа. В них проходят командные обсуждения с помощью текста, аудио и видео, а также выполняется обмен файлами и добавление вкладок.</span><span class="sxs-lookup"><span data-stu-id="55659-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="55659-107">Методы</span><span class="sxs-lookup"><span data-stu-id="55659-107">Methods</span></span>

| <span data-ttu-id="55659-108">Метод</span><span class="sxs-lookup"><span data-stu-id="55659-108">Method</span></span>       | <span data-ttu-id="55659-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="55659-109">Return Type</span></span>  |<span data-ttu-id="55659-110">Описание</span><span class="sxs-lookup"><span data-stu-id="55659-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55659-111">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="55659-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="55659-112">Коллекция [channel](channel.md)</span><span class="sxs-lookup"><span data-stu-id="55659-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="55659-113">Получение списка каналов в команде.</span><span class="sxs-lookup"><span data-stu-id="55659-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="55659-114">Создание канала</span><span class="sxs-lookup"><span data-stu-id="55659-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="55659-115">channel</span><span class="sxs-lookup"><span data-stu-id="55659-115">channel</span></span>](channel.md) | <span data-ttu-id="55659-116">Создание нового канала путем добавления отображаемого имени и описания.</span><span class="sxs-lookup"><span data-stu-id="55659-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="55659-117">Получение канала</span><span class="sxs-lookup"><span data-stu-id="55659-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="55659-118">channel</span><span class="sxs-lookup"><span data-stu-id="55659-118">channel</span></span>](channel.md) | <span data-ttu-id="55659-119">Чтение свойств и связей канала.</span><span class="sxs-lookup"><span data-stu-id="55659-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="55659-120">Обновление канала</span><span class="sxs-lookup"><span data-stu-id="55659-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="55659-121">channel</span><span class="sxs-lookup"><span data-stu-id="55659-121">channel</span></span>](channel.md) | <span data-ttu-id="55659-122">Обновление свойств канала.</span><span class="sxs-lookup"><span data-stu-id="55659-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="55659-123">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="55659-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="55659-124">Нет</span><span class="sxs-lookup"><span data-stu-id="55659-124">None</span></span> | <span data-ttu-id="55659-125">Удаление канала.</span><span class="sxs-lookup"><span data-stu-id="55659-125">Delete a channel.</span></span>|
|[<span data-ttu-id="55659-126">Перечисление сообщений в каналах</span><span class="sxs-lookup"><span data-stu-id="55659-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="55659-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="55659-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="55659-128">Получение сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="55659-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="55659-129">Создание объекта chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="55659-129">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="55659-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="55659-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="55659-131">Отправка сообщения в канал.</span><span class="sxs-lookup"><span data-stu-id="55659-131">Send a message to a channel</span></span> |
|[<span data-ttu-id="55659-132">Создание ответа на chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="55659-132">Create chatMessage reply in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="55659-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="55659-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="55659-134">Ответ на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="55659-134">Reply to a message in a channel</span></span>|
|[<span data-ttu-id="55659-135">Перечисление вкладок</span><span class="sxs-lookup"><span data-stu-id="55659-135">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="55659-136">teamsTab</span><span class="sxs-lookup"><span data-stu-id="55659-136">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="55659-137">Перечисление вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="55659-137">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="55659-138">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="55659-138">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="55659-139">teamsTab</span><span class="sxs-lookup"><span data-stu-id="55659-139">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="55659-140">Чтение вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="55659-140">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="55659-141">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="55659-141">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="55659-142">teamsTab</span><span class="sxs-lookup"><span data-stu-id="55659-142">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="55659-143">Добавление (закрепление) вкладки в канал.</span><span class="sxs-lookup"><span data-stu-id="55659-143">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="55659-144">Удаление вкладки</span><span class="sxs-lookup"><span data-stu-id="55659-144">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="55659-145">Нет</span><span class="sxs-lookup"><span data-stu-id="55659-145">None</span></span> | <span data-ttu-id="55659-146">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="55659-146">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="55659-147">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="55659-147">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="55659-148">teamsTab</span><span class="sxs-lookup"><span data-stu-id="55659-148">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="55659-149">Обновление свойств вкладки.</span><span class="sxs-lookup"><span data-stu-id="55659-149">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="55659-150">Свойства</span><span class="sxs-lookup"><span data-stu-id="55659-150">Properties</span></span>
| <span data-ttu-id="55659-151">Свойство</span><span class="sxs-lookup"><span data-stu-id="55659-151">Property</span></span>     | <span data-ttu-id="55659-152">Тип</span><span class="sxs-lookup"><span data-stu-id="55659-152">Type</span></span>   |<span data-ttu-id="55659-153">Описание</span><span class="sxs-lookup"><span data-stu-id="55659-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55659-154">description</span><span class="sxs-lookup"><span data-stu-id="55659-154">description</span></span>|<span data-ttu-id="55659-155">String</span><span class="sxs-lookup"><span data-stu-id="55659-155">String</span></span>|<span data-ttu-id="55659-156">Необязательное текстовое описание канала.</span><span class="sxs-lookup"><span data-stu-id="55659-156">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="55659-157">displayName</span><span class="sxs-lookup"><span data-stu-id="55659-157">displayName</span></span>|<span data-ttu-id="55659-158">String</span><span class="sxs-lookup"><span data-stu-id="55659-158">String</span></span>|<span data-ttu-id="55659-159">Имя канала, отображаемое для пользователя в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="55659-159">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="55659-160">id</span><span class="sxs-lookup"><span data-stu-id="55659-160">id</span></span>|<span data-ttu-id="55659-161">String</span><span class="sxs-lookup"><span data-stu-id="55659-161">String</span></span>|<span data-ttu-id="55659-162">Уникальный идентификатор канала.</span><span class="sxs-lookup"><span data-stu-id="55659-162">The channels's unique identifier.</span></span> <span data-ttu-id="55659-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55659-163">Read-only.</span></span>|
|<span data-ttu-id="55659-164">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="55659-164">isFavoriteByDefault</span></span>|<span data-ttu-id="55659-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="55659-165">Boolean</span></span>|<span data-ttu-id="55659-166">Должен ли канал автоматически помечаться как "Избранное" для всех участников команды.</span><span class="sxs-lookup"><span data-stu-id="55659-166">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="55659-167">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="55659-167">Default: `false`.</span></span>|
|<span data-ttu-id="55659-168">email</span><span class="sxs-lookup"><span data-stu-id="55659-168">email</span></span>|<span data-ttu-id="55659-169">String</span><span class="sxs-lookup"><span data-stu-id="55659-169">String</span></span>| <span data-ttu-id="55659-170">Адрес электронной почты для отправки сообщений в канал.</span><span class="sxs-lookup"><span data-stu-id="55659-170">The email address for sending messages to the channel.</span></span> <span data-ttu-id="55659-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55659-171">Read-only.</span></span>|
|<span data-ttu-id="55659-172">webUrl</span><span class="sxs-lookup"><span data-stu-id="55659-172">webUrl</span></span>|<span data-ttu-id="55659-173">String</span><span class="sxs-lookup"><span data-stu-id="55659-173">String</span></span>|<span data-ttu-id="55659-174">Гиперссылка, ведущая к каналу в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="55659-174">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="55659-175">Это URL-адрес, получаемый при щелчке правой кнопкой мыши по каналу в Microsoft Teams и выборе пункта "Получить ссылку на канал".</span><span class="sxs-lookup"><span data-stu-id="55659-175">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="55659-176">Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться.</span><span class="sxs-lookup"><span data-stu-id="55659-176">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="55659-177">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55659-177">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="55659-178">Отношения</span><span class="sxs-lookup"><span data-stu-id="55659-178">Relationships</span></span>
| <span data-ttu-id="55659-179">Отношение</span><span class="sxs-lookup"><span data-stu-id="55659-179">Relationship</span></span> | <span data-ttu-id="55659-180">Тип</span><span class="sxs-lookup"><span data-stu-id="55659-180">Type</span></span>   |<span data-ttu-id="55659-181">Описание</span><span class="sxs-lookup"><span data-stu-id="55659-181">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55659-182">messages</span><span class="sxs-lookup"><span data-stu-id="55659-182">messages</span></span>|<span data-ttu-id="55659-183">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="55659-183">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="55659-184">Коллекция всех сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="55659-184">A collection of all the messages in the channel.</span></span> <span data-ttu-id="55659-185">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="55659-185">A navigation property.</span></span> <span data-ttu-id="55659-186">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="55659-186">Nullable.</span></span> <span data-ttu-id="55659-187">В настоящее время этот API поддерживает чтение, но в конечном итоге будет также поддерживать написание сообщений.</span><span class="sxs-lookup"><span data-stu-id="55659-187">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="55659-188">tabs</span><span class="sxs-lookup"><span data-stu-id="55659-188">tabs</span></span>|<span data-ttu-id="55659-189">Коллекция [teamsTab](../resources/teamstab.md)</span><span class="sxs-lookup"><span data-stu-id="55659-189">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="55659-190">Коллекция всех вкладок в канале.</span><span class="sxs-lookup"><span data-stu-id="55659-190">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="55659-191">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="55659-191">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="55659-192">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55659-192">JSON representation</span></span>

<span data-ttu-id="55659-193">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55659-193">Here is a JSON representation of the resource</span></span>

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
