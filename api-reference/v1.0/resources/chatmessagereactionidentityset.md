---
title: тип ресурса chatMessageReactionIdentitySet
description: Представляет пользователя, который реагировал на сообщение в чате или канале.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 086cca8963bbb019ab7754a6aba3b644a5e14e2e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211119"
---
# <a name="chatmessagereactionidentityset-resource-type"></a><span data-ttu-id="ae882-103">тип ресурса chatMessageReactionIdentitySet</span><span class="sxs-lookup"><span data-stu-id="ae882-103">chatMessageReactionIdentitySet resource type</span></span>

<span data-ttu-id="ae882-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae882-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ae882-105">Представляет **пользователя, который** реагировал на [сообщение](../resources/chatmessage.md) в чате или канале.</span><span class="sxs-lookup"><span data-stu-id="ae882-105">Represents a **user** that reacted to a [message](../resources/chatmessage.md) in a chat or a channel.</span></span> <span data-ttu-id="ae882-106">Только `user` свойство имеет значение.</span><span class="sxs-lookup"><span data-stu-id="ae882-106">Only the `user` property has a value.</span></span>


<span data-ttu-id="ae882-107">Наследует от [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="ae882-107">Inherits from [identitySet](../resources/identityset.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ae882-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae882-108">Properties</span></span>
|<span data-ttu-id="ae882-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae882-109">Property</span></span>|<span data-ttu-id="ae882-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ae882-110">Type</span></span>|<span data-ttu-id="ae882-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ae882-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae882-112">application</span><span class="sxs-lookup"><span data-stu-id="ae882-112">application</span></span>|[<span data-ttu-id="ae882-113">identity</span><span class="sxs-lookup"><span data-stu-id="ae882-113">identity</span></span>](../resources/identity.md)|<span data-ttu-id="ae882-114">Наследуется от [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="ae882-114">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="ae882-115">Не установлено, так как приложения не могут реагировать на сообщения.</span><span class="sxs-lookup"><span data-stu-id="ae882-115">Not set because applications can't react to messages.</span></span>|
|<span data-ttu-id="ae882-116">device;</span><span class="sxs-lookup"><span data-stu-id="ae882-116">device</span></span>|[<span data-ttu-id="ae882-117">identity</span><span class="sxs-lookup"><span data-stu-id="ae882-117">identity</span></span>](../resources/identity.md)|<span data-ttu-id="ae882-118">Наследуется от [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="ae882-118">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="ae882-119">Не установлено, так как устройства не могут реагировать на сообщения.</span><span class="sxs-lookup"><span data-stu-id="ae882-119">Not set because devices can't react to messages.</span></span>|
|<span data-ttu-id="ae882-120">user</span><span class="sxs-lookup"><span data-stu-id="ae882-120">user</span></span>|[<span data-ttu-id="ae882-121">identity</span><span class="sxs-lookup"><span data-stu-id="ae882-121">identity</span></span>](../resources/identity.md)|<span data-ttu-id="ae882-122">Наследуется от [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="ae882-122">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="ae882-123">Сведения о пользователе, который отреагировал на сообщение.</span><span class="sxs-lookup"><span data-stu-id="ae882-123">Details about the user who reacted to the message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae882-124">Связи</span><span class="sxs-lookup"><span data-stu-id="ae882-124">Relationships</span></span>
<span data-ttu-id="ae882-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ae882-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae882-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ae882-126">JSON representation</span></span>
<span data-ttu-id="ae882-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae882-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageReactionIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageReactionIdentitySet",
  "user": {
    "@odata.type": "microsoft.graph.identity"
  },
  "application": {
    "@odata.type": "microsoft.graph.identity"
  },
  "device": {
    "@odata.type": "microsoft.graph.identity"
  }
}
```

