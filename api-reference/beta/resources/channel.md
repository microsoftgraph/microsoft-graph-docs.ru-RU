---
title: Тип ресурса channel
description: 'Канал — это коллекция объектов chatMessages в команде. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ae93d6f81d1be9b1af767129d75ceab75d23cec4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543715"
---
# <a name="channel-resource-type"></a><span data-ttu-id="1ce88-103">Тип ресурса channel</span><span class="sxs-lookup"><span data-stu-id="1ce88-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ce88-104">[Команды](../resources/team.md) состоят из каналов, являющихся беседами с сотрудниками.</span><span class="sxs-lookup"><span data-stu-id="1ce88-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="1ce88-105">Каждый канал предназначен для определенной темы, отдела или проекта.</span><span class="sxs-lookup"><span data-stu-id="1ce88-105">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="1ce88-106">Каналы — это место, где фактически выполняется работа. В них проходят командные обсуждения с помощью текста, аудио и видео, а также выполняется обмен файлами и добавление вкладок.</span><span class="sxs-lookup"><span data-stu-id="1ce88-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="1ce88-107">Методы</span><span class="sxs-lookup"><span data-stu-id="1ce88-107">Methods</span></span>

| <span data-ttu-id="1ce88-108">Метод</span><span class="sxs-lookup"><span data-stu-id="1ce88-108">Method</span></span>       | <span data-ttu-id="1ce88-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1ce88-109">Return Type</span></span>  |<span data-ttu-id="1ce88-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1ce88-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1ce88-111">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="1ce88-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="1ce88-112">Коллекция [channel](channel.md)</span><span class="sxs-lookup"><span data-stu-id="1ce88-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="1ce88-113">Получение списка каналов в команде.</span><span class="sxs-lookup"><span data-stu-id="1ce88-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="1ce88-114">Создание канала</span><span class="sxs-lookup"><span data-stu-id="1ce88-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="1ce88-115">channel</span><span class="sxs-lookup"><span data-stu-id="1ce88-115">channel</span></span>](channel.md) | <span data-ttu-id="1ce88-116">Создание нового канала путем добавления отображаемого имени и описания.</span><span class="sxs-lookup"><span data-stu-id="1ce88-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="1ce88-117">Получение канала</span><span class="sxs-lookup"><span data-stu-id="1ce88-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="1ce88-118">channel</span><span class="sxs-lookup"><span data-stu-id="1ce88-118">channel</span></span>](channel.md) | <span data-ttu-id="1ce88-119">Чтение свойств и связей канала.</span><span class="sxs-lookup"><span data-stu-id="1ce88-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="1ce88-120">Обновление канала</span><span class="sxs-lookup"><span data-stu-id="1ce88-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="1ce88-121">channel</span><span class="sxs-lookup"><span data-stu-id="1ce88-121">channel</span></span>](channel.md) | <span data-ttu-id="1ce88-122">Обновление свойств канала.</span><span class="sxs-lookup"><span data-stu-id="1ce88-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="1ce88-123">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="1ce88-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="1ce88-124">Нет</span><span class="sxs-lookup"><span data-stu-id="1ce88-124">None</span></span> | <span data-ttu-id="1ce88-125">Удаление канала.</span><span class="sxs-lookup"><span data-stu-id="1ce88-125">Delete a channel.</span></span>|
|[<span data-ttu-id="1ce88-126">Перечисление сообщений в каналах</span><span class="sxs-lookup"><span data-stu-id="1ce88-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="1ce88-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="1ce88-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="1ce88-128">Получение сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="1ce88-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="1ce88-129">Отправка сообщения канала</span><span class="sxs-lookup"><span data-stu-id="1ce88-129">Send channel message</span></span>](../api/channel-post-chatmessage.md)  | [<span data-ttu-id="1ce88-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="1ce88-130">chatMessage</span></span>](../resources/chatmessage.md) | [<span data-ttu-id="1ce88-131">Отправка сообщения в канал</span><span class="sxs-lookup"><span data-stu-id="1ce88-131">Send a message to a channel</span></span>](../api/channel-post-chatmessage.md) |
|[<span data-ttu-id="1ce88-132">Перечисление вкладок</span><span class="sxs-lookup"><span data-stu-id="1ce88-132">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="1ce88-133">teamsTab</span><span class="sxs-lookup"><span data-stu-id="1ce88-133">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="1ce88-134">Перечисление вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="1ce88-134">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="1ce88-135">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="1ce88-135">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="1ce88-136">teamsTab</span><span class="sxs-lookup"><span data-stu-id="1ce88-136">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="1ce88-137">Чтение вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="1ce88-137">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="1ce88-138">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="1ce88-138">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="1ce88-139">teamsTab</span><span class="sxs-lookup"><span data-stu-id="1ce88-139">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="1ce88-140">Добавление (закрепление) вкладки в канал.</span><span class="sxs-lookup"><span data-stu-id="1ce88-140">Adds (installs) a tab to a team's channel.</span></span>|
|[<span data-ttu-id="1ce88-141">Удаление вкладки</span><span class="sxs-lookup"><span data-stu-id="1ce88-141">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="1ce88-142">Нет</span><span class="sxs-lookup"><span data-stu-id="1ce88-142">None</span></span> | <span data-ttu-id="1ce88-143">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="1ce88-143">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="1ce88-144">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="1ce88-144">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="1ce88-145">teamsTab</span><span class="sxs-lookup"><span data-stu-id="1ce88-145">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="1ce88-146">Обновление свойств вкладки.</span><span class="sxs-lookup"><span data-stu-id="1ce88-146">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="1ce88-147">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ce88-147">Properties</span></span>
| <span data-ttu-id="1ce88-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ce88-148">Property</span></span>     | <span data-ttu-id="1ce88-149">Тип</span><span class="sxs-lookup"><span data-stu-id="1ce88-149">Type</span></span>   |<span data-ttu-id="1ce88-150">Описание</span><span class="sxs-lookup"><span data-stu-id="1ce88-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ce88-151">description</span><span class="sxs-lookup"><span data-stu-id="1ce88-151">description</span></span>|<span data-ttu-id="1ce88-152">String</span><span class="sxs-lookup"><span data-stu-id="1ce88-152">String</span></span>|<span data-ttu-id="1ce88-153">Необязательное текстовое описание канала.</span><span class="sxs-lookup"><span data-stu-id="1ce88-153">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="1ce88-154">displayName</span><span class="sxs-lookup"><span data-stu-id="1ce88-154">displayName</span></span>|<span data-ttu-id="1ce88-155">String</span><span class="sxs-lookup"><span data-stu-id="1ce88-155">String</span></span>|<span data-ttu-id="1ce88-156">Имя канала, отображаемое для пользователя в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1ce88-156">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="1ce88-157">id</span><span class="sxs-lookup"><span data-stu-id="1ce88-157">id</span></span>|<span data-ttu-id="1ce88-158">String</span><span class="sxs-lookup"><span data-stu-id="1ce88-158">String</span></span>|<span data-ttu-id="1ce88-159">Уникальный идентификатор канала.</span><span class="sxs-lookup"><span data-stu-id="1ce88-159">The channels's unique identifier.</span></span> <span data-ttu-id="1ce88-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1ce88-160">Read-only.</span></span>|
|<span data-ttu-id="1ce88-161">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="1ce88-161">isFavoriteByDefault</span></span>|<span data-ttu-id="1ce88-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ce88-162">Boolean</span></span>|<span data-ttu-id="1ce88-163">Должен ли канал автоматически помечаться как "Избранное" для всех участников команды.</span><span class="sxs-lookup"><span data-stu-id="1ce88-163">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="1ce88-164">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="1ce88-164">Default: `false`.</span></span>|
|<span data-ttu-id="1ce88-165">email</span><span class="sxs-lookup"><span data-stu-id="1ce88-165">email</span></span>|<span data-ttu-id="1ce88-166">String</span><span class="sxs-lookup"><span data-stu-id="1ce88-166">String</span></span>| <span data-ttu-id="1ce88-167">Адрес электронной почты для отправки сообщений в канал.</span><span class="sxs-lookup"><span data-stu-id="1ce88-167">The email address for sending messages to the channel.</span></span> <span data-ttu-id="1ce88-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1ce88-168">Read-only.</span></span>|
|<span data-ttu-id="1ce88-169">webUrl</span><span class="sxs-lookup"><span data-stu-id="1ce88-169">webUrl</span></span>|<span data-ttu-id="1ce88-170">String</span><span class="sxs-lookup"><span data-stu-id="1ce88-170">String</span></span>|<span data-ttu-id="1ce88-171">Гиперссылка, ведущая к каналу в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1ce88-171">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="1ce88-172">Это URL-адрес, получаемый при щелчке правой кнопкой мыши по каналу в Microsoft Teams и выборе пункта "Получить ссылку на канал".</span><span class="sxs-lookup"><span data-stu-id="1ce88-172">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="1ce88-173">Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться.</span><span class="sxs-lookup"><span data-stu-id="1ce88-173">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="1ce88-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1ce88-174">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="1ce88-175">Отношения</span><span class="sxs-lookup"><span data-stu-id="1ce88-175">Relationships</span></span>
| <span data-ttu-id="1ce88-176">Отношение</span><span class="sxs-lookup"><span data-stu-id="1ce88-176">Relationship</span></span> | <span data-ttu-id="1ce88-177">Тип</span><span class="sxs-lookup"><span data-stu-id="1ce88-177">Type</span></span>   |<span data-ttu-id="1ce88-178">Описание</span><span class="sxs-lookup"><span data-stu-id="1ce88-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ce88-179">messages</span><span class="sxs-lookup"><span data-stu-id="1ce88-179">messages</span></span>|<span data-ttu-id="1ce88-180">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="1ce88-180">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="1ce88-181">Коллекция всех сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="1ce88-181">A collection of all the messages in the channel.</span></span> <span data-ttu-id="1ce88-182">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="1ce88-182">A navigation property.</span></span> <span data-ttu-id="1ce88-183">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1ce88-183">Nullable.</span></span> <span data-ttu-id="1ce88-184">В настоящее время этот API поддерживает чтение, но в конечном итоге будет также поддерживать написание сообщений.</span><span class="sxs-lookup"><span data-stu-id="1ce88-184">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="1ce88-185">tabs</span><span class="sxs-lookup"><span data-stu-id="1ce88-185">tabs</span></span>|<span data-ttu-id="1ce88-186">Коллекция [teamsTab](../resources/teamstab.md)</span><span class="sxs-lookup"><span data-stu-id="1ce88-186">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="1ce88-187">Коллекция всех вкладок в канале.</span><span class="sxs-lookup"><span data-stu-id="1ce88-187">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="1ce88-188">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="1ce88-188">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1ce88-189">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ce88-189">JSON representation</span></span>

<span data-ttu-id="1ce88-190">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ce88-190">Here is a JSON representation of the resource</span></span>

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
