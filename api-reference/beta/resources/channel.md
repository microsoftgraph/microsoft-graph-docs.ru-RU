---
title: Тип ресурса канала
description: 'Канал представляет коллекцию chatMessages в группе. '
author: nkramer
ms.openlocfilehash: 18a3293b757e641eab98b166a43ce023762ccc6d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326777"
---
# <a name="channel-resource-type"></a><span data-ttu-id="91e29-103">Тип ресурса канала</span><span class="sxs-lookup"><span data-stu-id="91e29-103">channel resource type</span></span>

> <span data-ttu-id="91e29-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="91e29-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91e29-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91e29-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91e29-106">Канал представляет коллекцию [chatMessages](chatmessage.md) внутри [групп](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="91e29-106">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="91e29-107">Канал представляет раздел и логическая изоляции обсуждения в группе.</span><span class="sxs-lookup"><span data-stu-id="91e29-107">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="91e29-108">Примеры может быть канала «Пятница Lunch группы» и «Архитектура обсуждений» канала.</span><span class="sxs-lookup"><span data-stu-id="91e29-108">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="91e29-109">Методы</span><span class="sxs-lookup"><span data-stu-id="91e29-109">Methods</span></span>

| <span data-ttu-id="91e29-110">Метод</span><span class="sxs-lookup"><span data-stu-id="91e29-110">Method</span></span>       | <span data-ttu-id="91e29-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="91e29-111">Return Type</span></span>  |<span data-ttu-id="91e29-112">Описание</span><span class="sxs-lookup"><span data-stu-id="91e29-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="91e29-113">Список каналов</span><span class="sxs-lookup"><span data-stu-id="91e29-113">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="91e29-114">Коллекция [канала](channel.md)</span><span class="sxs-lookup"><span data-stu-id="91e29-114">[channel](channel.md) collection</span></span> | <span data-ttu-id="91e29-115">Получите список каналов в данной группы.</span><span class="sxs-lookup"><span data-stu-id="91e29-115">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="91e29-116">Создание канала</span><span class="sxs-lookup"><span data-stu-id="91e29-116">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="91e29-117">канал</span><span class="sxs-lookup"><span data-stu-id="91e29-117">channel</span></span>](channel.md) | <span data-ttu-id="91e29-118">Создайте новый канал, включая отображаемое имя и описание.</span><span class="sxs-lookup"><span data-stu-id="91e29-118">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="91e29-119">Получение канала</span><span class="sxs-lookup"><span data-stu-id="91e29-119">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="91e29-120">канал</span><span class="sxs-lookup"><span data-stu-id="91e29-120">channel</span></span>](channel.md) | <span data-ttu-id="91e29-121">Чтение свойства и связи канала.</span><span class="sxs-lookup"><span data-stu-id="91e29-121">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="91e29-122">Обновление канала</span><span class="sxs-lookup"><span data-stu-id="91e29-122">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="91e29-123">канал</span><span class="sxs-lookup"><span data-stu-id="91e29-123">channel</span></span>](channel.md) | <span data-ttu-id="91e29-124">Обновление свойств канала.</span><span class="sxs-lookup"><span data-stu-id="91e29-124">Update properties of the channel.</span></span>|
|[<span data-ttu-id="91e29-125">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="91e29-125">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="91e29-126">Нет</span><span class="sxs-lookup"><span data-stu-id="91e29-126">None</span></span> | <span data-ttu-id="91e29-127">Удаление канала.</span><span class="sxs-lookup"><span data-stu-id="91e29-127">Delete a channel.</span></span>|
|[<span data-ttu-id="91e29-128">Список сообщения</span><span class="sxs-lookup"><span data-stu-id="91e29-128">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="91e29-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="91e29-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="91e29-130">Получение сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="91e29-130">Get messages in a channel</span></span> |
|[<span data-ttu-id="91e29-131">Создать поток разговора</span><span class="sxs-lookup"><span data-stu-id="91e29-131">Create chat thread</span></span>](../api/channel-post-chatthreads.md) | <span data-ttu-id="91e29-132">[chatThread](chatthread.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="91e29-132">[chatThread](chatthread.md) collection</span></span>| <span data-ttu-id="91e29-133">Создайте поток разговора в указанном канала.</span><span class="sxs-lookup"><span data-stu-id="91e29-133">Create a chat thread in the specified channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="91e29-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="91e29-134">Properties</span></span>
| <span data-ttu-id="91e29-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="91e29-135">Property</span></span>     | <span data-ttu-id="91e29-136">Тип</span><span class="sxs-lookup"><span data-stu-id="91e29-136">Type</span></span>   |<span data-ttu-id="91e29-137">Описание</span><span class="sxs-lookup"><span data-stu-id="91e29-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91e29-138">описание</span><span class="sxs-lookup"><span data-stu-id="91e29-138">description</span></span>|<span data-ttu-id="91e29-139">Строка</span><span class="sxs-lookup"><span data-stu-id="91e29-139">String</span></span>|<span data-ttu-id="91e29-140">Необязательное текстовое описание для канала.</span><span class="sxs-lookup"><span data-stu-id="91e29-140">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="91e29-141">displayName</span><span class="sxs-lookup"><span data-stu-id="91e29-141">displayName</span></span>|<span data-ttu-id="91e29-142">Строка</span><span class="sxs-lookup"><span data-stu-id="91e29-142">String</span></span>|<span data-ttu-id="91e29-143">Имя канала, как оно будет отображаться для пользователей в группах Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="91e29-143">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="91e29-144">id</span><span class="sxs-lookup"><span data-stu-id="91e29-144">id</span></span>|<span data-ttu-id="91e29-145">Строка</span><span class="sxs-lookup"><span data-stu-id="91e29-145">String</span></span>|<span data-ttu-id="91e29-146">Уникальный идентификатор, каналов.</span><span class="sxs-lookup"><span data-stu-id="91e29-146">The channels's unique identifier.</span></span> <span data-ttu-id="91e29-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="91e29-147">Read-only.</span></span>|
|<span data-ttu-id="91e29-148">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="91e29-148">isFavoriteByDefault</span></span>|<span data-ttu-id="91e29-149">Boolean.</span><span class="sxs-lookup"><span data-stu-id="91e29-149">Boolean</span></span>|<span data-ttu-id="91e29-150">Является ли канал должен автоматически помечаются «Избранное» для всех членов группы.</span><span class="sxs-lookup"><span data-stu-id="91e29-150">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="91e29-151">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="91e29-151">Default: `false`.</span></span>|
|<span data-ttu-id="91e29-152">email</span><span class="sxs-lookup"><span data-stu-id="91e29-152">email</span></span>|<span data-ttu-id="91e29-153">Boolean.</span><span class="sxs-lookup"><span data-stu-id="91e29-153">Boolean</span></span>| <span data-ttu-id="91e29-154">Адрес электронной почты для отправки сообщений на канал.</span><span class="sxs-lookup"><span data-stu-id="91e29-154">The email address for sending messages to the channel.</span></span> <span data-ttu-id="91e29-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="91e29-155">Read-only.</span></span>|
|<span data-ttu-id="91e29-156">webUrl</span><span class="sxs-lookup"><span data-stu-id="91e29-156">webUrl</span></span>|<span data-ttu-id="91e29-157">Строка</span><span class="sxs-lookup"><span data-stu-id="91e29-157">String</span></span>|<span data-ttu-id="91e29-158">Гиперссылка, можно перейти к канала в группах Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="91e29-158">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="91e29-159">Это URL-адрес, который вы получаете при щелкните правой кнопкой мыши канала в группах Майкрософт и выберите ссылку Get для канала.</span><span class="sxs-lookup"><span data-stu-id="91e29-159">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="91e29-160">Этот URL-адрес должен быть обрабатываются как непрозрачный больших двоичных объектов и не синтаксический анализ.</span><span class="sxs-lookup"><span data-stu-id="91e29-160">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="91e29-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="91e29-161">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="91e29-162">Связи</span><span class="sxs-lookup"><span data-stu-id="91e29-162">Relationships</span></span>
| <span data-ttu-id="91e29-163">Связь</span><span class="sxs-lookup"><span data-stu-id="91e29-163">Relationship</span></span> | <span data-ttu-id="91e29-164">Тип</span><span class="sxs-lookup"><span data-stu-id="91e29-164">Type</span></span>   |<span data-ttu-id="91e29-165">Описание</span><span class="sxs-lookup"><span data-stu-id="91e29-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91e29-166">messages</span><span class="sxs-lookup"><span data-stu-id="91e29-166">messages</span></span>|<span data-ttu-id="91e29-167">[chatMessage](chatmessage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="91e29-167">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="91e29-168">Коллекция всех сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="91e29-168">A collection of all the messages in the channel.</span></span> <span data-ttu-id="91e29-169">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="91e29-169">A navigation property.</span></span> <span data-ttu-id="91e29-170">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="91e29-170">Nullable.</span></span> <span data-ttu-id="91e29-171">В настоящее время этот интерфейс API только поддерживает чтение, но со временем будут поддерживать сообщения о записи слишком.</span><span class="sxs-lookup"><span data-stu-id="91e29-171">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="91e29-172">chatThreads</span><span class="sxs-lookup"><span data-stu-id="91e29-172">chatThreads</span></span>|<span data-ttu-id="91e29-173">[chatThread](chatthread.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="91e29-173">[chatThread](chatthread.md) collection</span></span>|<span data-ttu-id="91e29-174">(Это постепенно пользу свойства сообщения) chatThreads поддерживает создание новых сообщений, но не чтение сообщений.</span><span class="sxs-lookup"><span data-stu-id="91e29-174">(This is being phased out in favor of the messages property) chatThreads supports creating new messages but not reading messages.</span></span> <span data-ttu-id="91e29-175">ChatThreads — это свойство навигации, а значение NULL.</span><span class="sxs-lookup"><span data-stu-id="91e29-175">ChatThreads is a navigation property, and is Nullable.</span></span>|
|<span data-ttu-id="91e29-176">вкладки</span><span class="sxs-lookup"><span data-stu-id="91e29-176">tabs</span></span>|<span data-ttu-id="91e29-177">[teamsTab](../resources/teamstab.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="91e29-177">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="91e29-178">Коллекция всех вкладок в канале.</span><span class="sxs-lookup"><span data-stu-id="91e29-178">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="91e29-179">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="91e29-179">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="91e29-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91e29-180">JSON representation</span></span>

<span data-ttu-id="91e29-181">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91e29-181">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
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
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
