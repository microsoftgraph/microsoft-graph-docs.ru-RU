---
title: Тип ресурса channelModerationSettings
description: Используется для управления тем, кто может запускать новые записи и отвечать на них в канале.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b67d55eb57d1a4b554b027270f700cbd590d4416
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796586"
---
# <a name="channelmoderationsettings-resource-type"></a><span data-ttu-id="51f0c-103">Тип ресурса channelModerationSettings</span><span class="sxs-lookup"><span data-stu-id="51f0c-103">channelModerationSettings resource type</span></span>

<span data-ttu-id="51f0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51f0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51f0c-105">В Microsoft Teams владельцы команд могут включить модерацию для канала, чтобы контролировать, кто может запускать новые записи и отвечать на публикации в этом канале.</span><span class="sxs-lookup"><span data-stu-id="51f0c-105">In Microsoft Teams, team owners can turn on moderation for a channel to control who can start new posts and reply to posts in that channel.</span></span> <span data-ttu-id="51f0c-106">Например, владельцам может потребоваться сделать следующее:</span><span class="sxs-lookup"><span data-stu-id="51f0c-106">For example, owners might want to do the following:</span></span>

- <span data-ttu-id="51f0c-107">Используйте канал только для объявлений.</span><span class="sxs-lookup"><span data-stu-id="51f0c-107">Use a channel for announcements only.</span></span>
- <span data-ttu-id="51f0c-108">Используйте канал для обсуждений в группе класса, где только преподаватель может начинать новые обсуждения.</span><span class="sxs-lookup"><span data-stu-id="51f0c-108">Use a channel for discussions in a class team where only the teacher can start new discussions.</span></span>
- <span data-ttu-id="51f0c-109">Используйте канал для проблем с сайтами, в которых соединители могут начать новые публикации.</span><span class="sxs-lookup"><span data-stu-id="51f0c-109">Use a channel for livesite issues where new posts can be started by connectors.</span></span>

<span data-ttu-id="51f0c-110">По умолчанию модерация — это означает, что обычные параметры канала применяются к владельцам и участникам команды с дополнительным контролем, чтобы разрешить только участникам команды или всем, включая гостей, запускать новую публикацию `OFF` канала.</span><span class="sxs-lookup"><span data-stu-id="51f0c-110">By default, moderation is `OFF`, which means that the usual channel settings apply to team owners and team members, with additional control to allow only team members or everyone including guests to start a new channel post.</span></span> <span data-ttu-id="51f0c-111">Настройка модерации канала, позволяющая только модераторам запускать новые записи с дополнительным контролем `ON` для участников группы.</span><span class="sxs-lookup"><span data-stu-id="51f0c-111">Setting channel moderation to `ON` allows only moderators to start new posts, with additional control for team members.</span></span>

<span data-ttu-id="51f0c-112">Для поддержки параметров модерации каналов с помощью API Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="51f0c-112">To support channel moderation settings via Microsoft Graph APIs:</span></span>

- <span data-ttu-id="51f0c-113">Участники группы должны иметь возможность запрашивать параметры модерации канала.</span><span class="sxs-lookup"><span data-stu-id="51f0c-113">Team members should be able to query channel moderation settings.</span></span>
- <span data-ttu-id="51f0c-114">Владельцы команд должны иметь возможность устанавливать параметры модерации каналов.</span><span class="sxs-lookup"><span data-stu-id="51f0c-114">Team owners should be able to set channel moderation settings.</span></span>

## <a name="properties"></a><span data-ttu-id="51f0c-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="51f0c-115">Properties</span></span>
|<span data-ttu-id="51f0c-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="51f0c-116">Property</span></span>|<span data-ttu-id="51f0c-117">Тип</span><span class="sxs-lookup"><span data-stu-id="51f0c-117">Type</span></span>|<span data-ttu-id="51f0c-118">Описание</span><span class="sxs-lookup"><span data-stu-id="51f0c-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51f0c-119">allowNewMessageFromBots</span><span class="sxs-lookup"><span data-stu-id="51f0c-119">allowNewMessageFromBots</span></span>|<span data-ttu-id="51f0c-120">Логический</span><span class="sxs-lookup"><span data-stu-id="51f0c-120">Boolean</span></span>|<span data-ttu-id="51f0c-121">Указывает, разрешено ли ботам размещать сообщения.</span><span class="sxs-lookup"><span data-stu-id="51f0c-121">Indicates whether bots are allowed to post messages.</span></span>|
|<span data-ttu-id="51f0c-122">allowNewMessageFromConnectors</span><span class="sxs-lookup"><span data-stu-id="51f0c-122">allowNewMessageFromConnectors</span></span>|<span data-ttu-id="51f0c-123">Логический</span><span class="sxs-lookup"><span data-stu-id="51f0c-123">Boolean</span></span>|<span data-ttu-id="51f0c-124">Указывает, разрешено ли соединитетелям отправлять сообщения.</span><span class="sxs-lookup"><span data-stu-id="51f0c-124">Indicates whether connectors are allowed to post messages.</span></span>|
|<span data-ttu-id="51f0c-125">replyRestriction</span><span class="sxs-lookup"><span data-stu-id="51f0c-125">replyRestriction</span></span>|<span data-ttu-id="51f0c-126">replyRestriction</span><span class="sxs-lookup"><span data-stu-id="51f0c-126">replyRestriction</span></span>|<span data-ttu-id="51f0c-127">Указывает, кому разрешено отвечать на канал teams.</span><span class="sxs-lookup"><span data-stu-id="51f0c-127">Indicates who is allowed to reply to the teams channel.</span></span> <span data-ttu-id="51f0c-128">Возможные значения: `everyone`, `authorAndModerators`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="51f0c-128">Possible values are: `everyone`, `authorAndModerators`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="51f0c-129">userNewMessageRestriction</span><span class="sxs-lookup"><span data-stu-id="51f0c-129">userNewMessageRestriction</span></span>|<span data-ttu-id="51f0c-130">userNewMessageRestriction</span><span class="sxs-lookup"><span data-stu-id="51f0c-130">userNewMessageRestriction</span></span>|<span data-ttu-id="51f0c-131">Указывает, кому разрешено отправлять сообщения в канал Teams.</span><span class="sxs-lookup"><span data-stu-id="51f0c-131">Indicates who is allowed to post messages to teams channel.</span></span> <span data-ttu-id="51f0c-132">Возможные значения: `everyone`, `everyoneExceptGuests`, `moderators`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="51f0c-132">Possible values are: `everyone`, `everyoneExceptGuests`, `moderators`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51f0c-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51f0c-133">JSON representation</span></span>
<span data-ttu-id="51f0c-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51f0c-134">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelModerationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelModerationSettings",
  "userNewMessageRestriction": "String",
  "replyRestriction": "String",
  "allowNewMessageFromBots": "Boolean",
  "allowNewMessageFromConnectors": "Boolean"
}
```

## <a name="see-also"></a><span data-ttu-id="51f0c-135">См. также</span><span class="sxs-lookup"><span data-stu-id="51f0c-135">See also</span></span>

- <span data-ttu-id="51f0c-136">Чтобы изменить параметры модерации канала, см. пример 2 в [канале Update.](../api/channel-patch.md)</span><span class="sxs-lookup"><span data-stu-id="51f0c-136">To modify moderation settings of a channel, see example 2 in [Update channel](../api/channel-patch.md).</span></span>
