---
title: Тип ресурса channel
description: 'Канал — это коллекция сообщений в команде. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 6c1f73746081e5b1e4f78acb91d43e33c1c9bf73
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569461"
---
# <a name="channel-resource-type"></a><span data-ttu-id="05850-103">Тип ресурса channel</span><span class="sxs-lookup"><span data-stu-id="05850-103">channel resource type</span></span>

<span data-ttu-id="05850-104">[Команды](../resources/team.md) состоят из каналов, являющихся беседами с сотрудниками.</span><span class="sxs-lookup"><span data-stu-id="05850-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="05850-105">Каждый канал предназначен для определенной темы, отдела или проекта.</span><span class="sxs-lookup"><span data-stu-id="05850-105">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="05850-106">Каналы — это место, где фактически выполняется работа. В них проходят командные обсуждения с помощью текста, аудио и видео, а также выполняется обмен файлами и добавление вкладок.</span><span class="sxs-lookup"><span data-stu-id="05850-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="05850-107">Методы</span><span class="sxs-lookup"><span data-stu-id="05850-107">Methods</span></span>

| <span data-ttu-id="05850-108">Метод</span><span class="sxs-lookup"><span data-stu-id="05850-108">Method</span></span>       | <span data-ttu-id="05850-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="05850-109">Return Type</span></span>  |<span data-ttu-id="05850-110">Описание</span><span class="sxs-lookup"><span data-stu-id="05850-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="05850-111">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="05850-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="05850-112">Коллекция [channel](channel.md)</span><span class="sxs-lookup"><span data-stu-id="05850-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="05850-113">Получение списка каналов в команде.</span><span class="sxs-lookup"><span data-stu-id="05850-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="05850-114">Создание канала</span><span class="sxs-lookup"><span data-stu-id="05850-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="05850-115">channel</span><span class="sxs-lookup"><span data-stu-id="05850-115">channel</span></span>](channel.md) | <span data-ttu-id="05850-116">Создание нового канала путем добавления отображаемого имени и описания.</span><span class="sxs-lookup"><span data-stu-id="05850-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="05850-117">Получение канала</span><span class="sxs-lookup"><span data-stu-id="05850-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="05850-118">channel</span><span class="sxs-lookup"><span data-stu-id="05850-118">channel</span></span>](channel.md) | <span data-ttu-id="05850-119">Чтение свойств и связей канала.</span><span class="sxs-lookup"><span data-stu-id="05850-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="05850-120">Обновление канала</span><span class="sxs-lookup"><span data-stu-id="05850-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="05850-121">channel</span><span class="sxs-lookup"><span data-stu-id="05850-121">channel</span></span>](channel.md) | <span data-ttu-id="05850-122">Обновление свойств канала.</span><span class="sxs-lookup"><span data-stu-id="05850-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="05850-123">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="05850-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="05850-124">Нет</span><span class="sxs-lookup"><span data-stu-id="05850-124">None</span></span> | <span data-ttu-id="05850-125">Удаление канала.</span><span class="sxs-lookup"><span data-stu-id="05850-125">Delete a channel.</span></span>|
|[<span data-ttu-id="05850-126">Перечисление вкладок</span><span class="sxs-lookup"><span data-stu-id="05850-126">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="05850-127">teamsTab</span><span class="sxs-lookup"><span data-stu-id="05850-127">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="05850-128">Перечисление вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="05850-128">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="05850-129">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="05850-129">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="05850-130">teamsTab</span><span class="sxs-lookup"><span data-stu-id="05850-130">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="05850-131">Чтение вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="05850-131">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="05850-132">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="05850-132">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="05850-133">teamsTab</span><span class="sxs-lookup"><span data-stu-id="05850-133">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="05850-134">Добавление (закрепление) вкладки в канал.</span><span class="sxs-lookup"><span data-stu-id="05850-134">Adds (installs) a tab to a team's channel.</span></span>|
|[<span data-ttu-id="05850-135">Удаление вкладки</span><span class="sxs-lookup"><span data-stu-id="05850-135">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="05850-136">Нет</span><span class="sxs-lookup"><span data-stu-id="05850-136">None</span></span> | <span data-ttu-id="05850-137">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="05850-137">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="05850-138">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="05850-138">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="05850-139">teamsTab</span><span class="sxs-lookup"><span data-stu-id="05850-139">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="05850-140">Обновление свойств вкладки.</span><span class="sxs-lookup"><span data-stu-id="05850-140">Updates the tab properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="05850-141">Свойства</span><span class="sxs-lookup"><span data-stu-id="05850-141">Properties</span></span>
| <span data-ttu-id="05850-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="05850-142">Property</span></span>     | <span data-ttu-id="05850-143">Тип</span><span class="sxs-lookup"><span data-stu-id="05850-143">Type</span></span>   |<span data-ttu-id="05850-144">Описание</span><span class="sxs-lookup"><span data-stu-id="05850-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05850-145">description</span><span class="sxs-lookup"><span data-stu-id="05850-145">description</span></span>|<span data-ttu-id="05850-146">String</span><span class="sxs-lookup"><span data-stu-id="05850-146">String</span></span>|<span data-ttu-id="05850-147">Необязательное текстовое описание канала.</span><span class="sxs-lookup"><span data-stu-id="05850-147">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="05850-148">displayName</span><span class="sxs-lookup"><span data-stu-id="05850-148">displayName</span></span>|<span data-ttu-id="05850-149">String</span><span class="sxs-lookup"><span data-stu-id="05850-149">String</span></span>|<span data-ttu-id="05850-150">Имя канала, отображаемое для пользователя в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="05850-150">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="05850-151">email</span><span class="sxs-lookup"><span data-stu-id="05850-151">email</span></span>|<span data-ttu-id="05850-152">String</span><span class="sxs-lookup"><span data-stu-id="05850-152">String</span></span>| <span data-ttu-id="05850-153">Адрес электронной почты для отправки сообщений в канал.</span><span class="sxs-lookup"><span data-stu-id="05850-153">The email address for sending messages to the channel.</span></span> <span data-ttu-id="05850-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="05850-154">Read-only.</span></span>|
|<span data-ttu-id="05850-155">id</span><span class="sxs-lookup"><span data-stu-id="05850-155">id</span></span>|<span data-ttu-id="05850-156">String</span><span class="sxs-lookup"><span data-stu-id="05850-156">String</span></span>|<span data-ttu-id="05850-157">Уникальный идентификатор канала.</span><span class="sxs-lookup"><span data-stu-id="05850-157">The channels's unique identifier.</span></span> <span data-ttu-id="05850-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="05850-158">Read-only.</span></span>|
|<span data-ttu-id="05850-159">webUrl</span><span class="sxs-lookup"><span data-stu-id="05850-159">webUrl</span></span>|<span data-ttu-id="05850-160">String</span><span class="sxs-lookup"><span data-stu-id="05850-160">String</span></span>|<span data-ttu-id="05850-161">Гиперссылка, ведущая к каналу в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="05850-161">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="05850-162">Это URL-адрес, получаемый при щелчке правой кнопкой мыши по каналу в Microsoft Teams и выборе пункта "Получить ссылку на канал".</span><span class="sxs-lookup"><span data-stu-id="05850-162">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="05850-163">Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться.</span><span class="sxs-lookup"><span data-stu-id="05850-163">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="05850-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="05850-164">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05850-165">Отношения</span><span class="sxs-lookup"><span data-stu-id="05850-165">Relationships</span></span>
| <span data-ttu-id="05850-166">Отношение</span><span class="sxs-lookup"><span data-stu-id="05850-166">Relationship</span></span> | <span data-ttu-id="05850-167">Тип</span><span class="sxs-lookup"><span data-stu-id="05850-167">Type</span></span>   |<span data-ttu-id="05850-168">Описание</span><span class="sxs-lookup"><span data-stu-id="05850-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05850-169">tabs</span><span class="sxs-lookup"><span data-stu-id="05850-169">tabs</span></span>|<span data-ttu-id="05850-170">Коллекция [teamsTab](../resources/teamstab.md)</span><span class="sxs-lookup"><span data-stu-id="05850-170">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="05850-171">Коллекция всех вкладок в канале.</span><span class="sxs-lookup"><span data-stu-id="05850-171">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="05850-172">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="05850-172">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="05850-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05850-173">JSON representation</span></span>

<span data-ttu-id="05850-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05850-174">Here is a JSON representation of the resource</span></span>

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
