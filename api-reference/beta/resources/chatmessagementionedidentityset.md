---
title: тип ресурса chatMessageMentionedIdentitySet
description: Представляет ресурс, @mentioned в сообщении в чате или канале.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9bbd65344616a979916a1b2bf32528bc8cd00814
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211356"
---
# <a name="chatmessagementionedidentityset-resource-type"></a><span data-ttu-id="c03a8-103">тип ресурса chatMessageMentionedIdentitySet</span><span class="sxs-lookup"><span data-stu-id="c03a8-103">chatMessageMentionedIdentitySet resource type</span></span>

<span data-ttu-id="c03a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c03a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c03a8-105">Представляет ресурс (пользователь, приложение или беседа) @mentioned [в](../resources/chatmessage.md) сообщении в чате или канале.</span><span class="sxs-lookup"><span data-stu-id="c03a8-105">Represents the resource (user, application, or conversation) @mentioned in a [message](../resources/chatmessage.md) in a chat or a channel.</span></span>


<span data-ttu-id="c03a8-106">Наследует от [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="c03a8-106">Inherits from [identitySet](../resources/identityset.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c03a8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c03a8-107">Properties</span></span>
|<span data-ttu-id="c03a8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c03a8-108">Property</span></span>|<span data-ttu-id="c03a8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c03a8-109">Type</span></span>|<span data-ttu-id="c03a8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c03a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c03a8-111">application</span><span class="sxs-lookup"><span data-stu-id="c03a8-111">application</span></span>|[<span data-ttu-id="c03a8-112">identity</span><span class="sxs-lookup"><span data-stu-id="c03a8-112">identity</span></span>](../resources/identity.md)|<span data-ttu-id="c03a8-113">Наследуется от [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="c03a8-113">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="c03a8-114">Если присутствует, представляет приложение (например, бот) @mentioned в [сообщении.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="c03a8-114">If present, represents an application (for example, bot) @mentioned in a [message](../resources/chatmessage.md).</span></span>|
|<span data-ttu-id="c03a8-115">conversation</span><span class="sxs-lookup"><span data-stu-id="c03a8-115">conversation</span></span>|[<span data-ttu-id="c03a8-116">teamworkConversationIdentity</span><span class="sxs-lookup"><span data-stu-id="c03a8-116">teamworkConversationIdentity</span></span>](../resources/teamworkconversationidentity.md)|<span data-ttu-id="c03a8-117">При этом представляет беседу (например, команду или канал) @mentioned в [сообщении.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="c03a8-117">If present, represents a conversation (for example, team or channel) @mentioned in a [message](../resources/chatmessage.md).</span></span>|
|<span data-ttu-id="c03a8-118">device;</span><span class="sxs-lookup"><span data-stu-id="c03a8-118">device</span></span>|[<span data-ttu-id="c03a8-119">identity</span><span class="sxs-lookup"><span data-stu-id="c03a8-119">identity</span></span>](../resources/identity.md)|<span data-ttu-id="c03a8-120">Наследуется от [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="c03a8-120">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="c03a8-121">Не используется, так как не поддерживается для @mention устройств.</span><span class="sxs-lookup"><span data-stu-id="c03a8-121">Not used because it's not supported to @mention devices.</span></span>|
|<span data-ttu-id="c03a8-122">user</span><span class="sxs-lookup"><span data-stu-id="c03a8-122">user</span></span>|[<span data-ttu-id="c03a8-123">identity</span><span class="sxs-lookup"><span data-stu-id="c03a8-123">identity</span></span>](../resources/identity.md)|<span data-ttu-id="c03a8-124">Наследуется от [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="c03a8-124">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="c03a8-125">Если присутствует, представляет пользователя @mentioned в [сообщении](../resources/chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="c03a8-125">If present, represents a user @mentioned in a [message](../resources/chatmessage.md).</span></span>|
|<span data-ttu-id="c03a8-126">tag</span><span class="sxs-lookup"><span data-stu-id="c03a8-126">tag</span></span>|[<span data-ttu-id="c03a8-127">teamworkTagIdentity</span><span class="sxs-lookup"><span data-stu-id="c03a8-127">teamworkTagIdentity</span></span>](../resources/teamworktagidentity.md)|<span data-ttu-id="c03a8-128">Если присутствует, представляет тег, @mentioned в командном [сообщении.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="c03a8-128">If present, represents a tag @mentioned in a team [message](../resources/chatmessage.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c03a8-129">Связи</span><span class="sxs-lookup"><span data-stu-id="c03a8-129">Relationships</span></span>
<span data-ttu-id="c03a8-130">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c03a8-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c03a8-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c03a8-131">JSON representation</span></span>
<span data-ttu-id="c03a8-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c03a8-132">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageMentionedIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageMentionedIdentitySet",
  "user": {
    "@odata.type": "microsoft.graph.identity"
  },
  "application": {
    "@odata.type": "microsoft.graph.identity"
  },
  "device": {
    "@odata.type": "microsoft.graph.identity"
  },
  "conversation": {
    "@odata.type": "microsoft.graph.teamworkConversationIdentity"
  },
  "tag": {
    "@odata.type": "microsoft.graph.teamworkTagIdentity"
  }
}
```