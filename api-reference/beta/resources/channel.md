---
title: Тип ресурса channel
description: 'Канал — это коллекция объектов chatMessages в команде. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d58a3e0b867a675e378fa126108331fd5b27856c
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994470"
---
# <a name="channel-resource-type"></a><span data-ttu-id="bdf51-103">Тип ресурса channel</span><span class="sxs-lookup"><span data-stu-id="bdf51-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdf51-104">Канал — это коллекция объектов [chatMessages](chatmessage.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="bdf51-104">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="bdf51-105">Канал представляет тему и логически обособляет обсуждение в команде.</span><span class="sxs-lookup"><span data-stu-id="bdf51-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="bdf51-106">Примеры: канал "Пятничный обед команды" и канал "Обсуждение архитектуры".</span><span class="sxs-lookup"><span data-stu-id="bdf51-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="bdf51-107">Методы</span><span class="sxs-lookup"><span data-stu-id="bdf51-107">Methods</span></span>

| <span data-ttu-id="bdf51-108">Метод</span><span class="sxs-lookup"><span data-stu-id="bdf51-108">Method</span></span>       | <span data-ttu-id="bdf51-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bdf51-109">Return Type</span></span>  |<span data-ttu-id="bdf51-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bdf51-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bdf51-111">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="bdf51-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="bdf51-112">Коллекция [channel](channel.md)</span><span class="sxs-lookup"><span data-stu-id="bdf51-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="bdf51-113">Получение списка каналов в команде.</span><span class="sxs-lookup"><span data-stu-id="bdf51-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="bdf51-114">Создание канала</span><span class="sxs-lookup"><span data-stu-id="bdf51-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="bdf51-115">channel</span><span class="sxs-lookup"><span data-stu-id="bdf51-115">channel</span></span>](channel.md) | <span data-ttu-id="bdf51-116">Создание нового канала путем добавления отображаемого имени и описания.</span><span class="sxs-lookup"><span data-stu-id="bdf51-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="bdf51-117">Получение канала</span><span class="sxs-lookup"><span data-stu-id="bdf51-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="bdf51-118">channel</span><span class="sxs-lookup"><span data-stu-id="bdf51-118">channel</span></span>](channel.md) | <span data-ttu-id="bdf51-119">Чтение свойств и связей канала.</span><span class="sxs-lookup"><span data-stu-id="bdf51-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="bdf51-120">Обновление канала</span><span class="sxs-lookup"><span data-stu-id="bdf51-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="bdf51-121">channel</span><span class="sxs-lookup"><span data-stu-id="bdf51-121">channel</span></span>](channel.md) | <span data-ttu-id="bdf51-122">Обновление свойств канала.</span><span class="sxs-lookup"><span data-stu-id="bdf51-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="bdf51-123">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="bdf51-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="bdf51-124">Нет</span><span class="sxs-lookup"><span data-stu-id="bdf51-124">None</span></span> | <span data-ttu-id="bdf51-125">Удаление канала.</span><span class="sxs-lookup"><span data-stu-id="bdf51-125">Delete a channel.</span></span>|
|[<span data-ttu-id="bdf51-126">Перечисление сообщений в каналах</span><span class="sxs-lookup"><span data-stu-id="bdf51-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="bdf51-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="bdf51-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="bdf51-128">Получение сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="bdf51-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="bdf51-129">Отправка сообщения канала</span><span class="sxs-lookup"><span data-stu-id="bdf51-129">Send channel message</span></span>](../api/channel-post-chatmessage.md)  | [<span data-ttu-id="bdf51-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="bdf51-130">chatMessage</span></span>](../resources/chatmessage.md) | [<span data-ttu-id="bdf51-131">Отправка сообщения в канал</span><span class="sxs-lookup"><span data-stu-id="bdf51-131">Send a message to a channel</span></span>](../api/channel-post-chatmessage.md) |


## <a name="properties"></a><span data-ttu-id="bdf51-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="bdf51-132">Properties</span></span>
| <span data-ttu-id="bdf51-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="bdf51-133">Property</span></span>     | <span data-ttu-id="bdf51-134">Тип</span><span class="sxs-lookup"><span data-stu-id="bdf51-134">Type</span></span>   |<span data-ttu-id="bdf51-135">Описание</span><span class="sxs-lookup"><span data-stu-id="bdf51-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdf51-136">description</span><span class="sxs-lookup"><span data-stu-id="bdf51-136">description</span></span>|<span data-ttu-id="bdf51-137">String</span><span class="sxs-lookup"><span data-stu-id="bdf51-137">String</span></span>|<span data-ttu-id="bdf51-138">Необязательное текстовое описание канала.</span><span class="sxs-lookup"><span data-stu-id="bdf51-138">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="bdf51-139">displayName</span><span class="sxs-lookup"><span data-stu-id="bdf51-139">displayName</span></span>|<span data-ttu-id="bdf51-140">String</span><span class="sxs-lookup"><span data-stu-id="bdf51-140">String</span></span>|<span data-ttu-id="bdf51-141">Имя канала, отображаемое для пользователя в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="bdf51-141">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="bdf51-142">id</span><span class="sxs-lookup"><span data-stu-id="bdf51-142">id</span></span>|<span data-ttu-id="bdf51-143">String</span><span class="sxs-lookup"><span data-stu-id="bdf51-143">String</span></span>|<span data-ttu-id="bdf51-144">Уникальный идентификатор канала.</span><span class="sxs-lookup"><span data-stu-id="bdf51-144">The channels's unique identifier.</span></span> <span data-ttu-id="bdf51-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bdf51-145">Read-only.</span></span>|
|<span data-ttu-id="bdf51-146">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="bdf51-146">isFavoriteByDefault</span></span>|<span data-ttu-id="bdf51-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="bdf51-147">Boolean</span></span>|<span data-ttu-id="bdf51-148">Должен ли канал автоматически помечаться как "Избранное" для всех участников команды.</span><span class="sxs-lookup"><span data-stu-id="bdf51-148">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="bdf51-149">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="bdf51-149">Default: `false`.</span></span>|
|<span data-ttu-id="bdf51-150">email</span><span class="sxs-lookup"><span data-stu-id="bdf51-150">email</span></span>|<span data-ttu-id="bdf51-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="bdf51-151">Boolean</span></span>| <span data-ttu-id="bdf51-152">Адрес электронной почты для отправки сообщений в канал.</span><span class="sxs-lookup"><span data-stu-id="bdf51-152">The email address for sending messages to the channel.</span></span> <span data-ttu-id="bdf51-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bdf51-153">Read-only.</span></span>|
|<span data-ttu-id="bdf51-154">webUrl</span><span class="sxs-lookup"><span data-stu-id="bdf51-154">webUrl</span></span>|<span data-ttu-id="bdf51-155">String</span><span class="sxs-lookup"><span data-stu-id="bdf51-155">String</span></span>|<span data-ttu-id="bdf51-156">Гиперссылка, ведущая к каналу в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="bdf51-156">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="bdf51-157">Это URL-адрес, получаемый при щелчке правой кнопкой мыши по каналу в Microsoft Teams и выборе пункта "Получить ссылку на канал".</span><span class="sxs-lookup"><span data-stu-id="bdf51-157">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="bdf51-158">Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться.</span><span class="sxs-lookup"><span data-stu-id="bdf51-158">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="bdf51-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bdf51-159">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="bdf51-160">Отношения</span><span class="sxs-lookup"><span data-stu-id="bdf51-160">Relationships</span></span>
| <span data-ttu-id="bdf51-161">Связь</span><span class="sxs-lookup"><span data-stu-id="bdf51-161">Relationship</span></span> | <span data-ttu-id="bdf51-162">Тип</span><span class="sxs-lookup"><span data-stu-id="bdf51-162">Type</span></span>   |<span data-ttu-id="bdf51-163">Описание</span><span class="sxs-lookup"><span data-stu-id="bdf51-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdf51-164">messages</span><span class="sxs-lookup"><span data-stu-id="bdf51-164">messages</span></span>|<span data-ttu-id="bdf51-165">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="bdf51-165">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="bdf51-166">Коллекция всех сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="bdf51-166">A collection of all the messages in the channel.</span></span> <span data-ttu-id="bdf51-167">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="bdf51-167">A navigation property.</span></span> <span data-ttu-id="bdf51-168">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bdf51-168">Nullable.</span></span> <span data-ttu-id="bdf51-169">В настоящее время этот API поддерживает чтение, но в конечном итоге будет также поддерживать написание сообщений.</span><span class="sxs-lookup"><span data-stu-id="bdf51-169">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="bdf51-170">tabs</span><span class="sxs-lookup"><span data-stu-id="bdf51-170">tabs</span></span>|<span data-ttu-id="bdf51-171">Коллекция [teamsTab](../resources/teamstab.md)</span><span class="sxs-lookup"><span data-stu-id="bdf51-171">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="bdf51-172">Коллекция всех вкладок в канале.</span><span class="sxs-lookup"><span data-stu-id="bdf51-172">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="bdf51-173">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="bdf51-173">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="bdf51-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bdf51-174">JSON representation</span></span>

<span data-ttu-id="bdf51-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bdf51-175">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/channel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
