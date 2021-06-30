---
title: тип ресурса chatMessageReactionIdentitySet
description: Представляет пользователя, который реагировал на сообщение в чате или канале.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 032b335656d768f505cdb673b56ef0955cf9ed58
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211353"
---
# <a name="chatmessagereactionidentityset-resource-type"></a><span data-ttu-id="f147a-103">тип ресурса chatMessageReactionIdentitySet</span><span class="sxs-lookup"><span data-stu-id="f147a-103">chatMessageReactionIdentitySet resource type</span></span>

<span data-ttu-id="f147a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f147a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f147a-105">Представляет **пользователя, который** реагировал на [сообщение](../resources/chatmessage.md) в чате или канале.</span><span class="sxs-lookup"><span data-stu-id="f147a-105">Represents a **user** that reacted to a [message](../resources/chatmessage.md) in a chat or a channel.</span></span> <span data-ttu-id="f147a-106">Только `user` свойство имеет значение.</span><span class="sxs-lookup"><span data-stu-id="f147a-106">Only the `user` property has a value.</span></span>


<span data-ttu-id="f147a-107">Наследует от [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="f147a-107">Inherits from [identitySet](../resources/identityset.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f147a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f147a-108">Properties</span></span>
|<span data-ttu-id="f147a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f147a-109">Property</span></span>|<span data-ttu-id="f147a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f147a-110">Type</span></span>|<span data-ttu-id="f147a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f147a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f147a-112">application</span><span class="sxs-lookup"><span data-stu-id="f147a-112">application</span></span>|[<span data-ttu-id="f147a-113">identity</span><span class="sxs-lookup"><span data-stu-id="f147a-113">identity</span></span>](../resources/identity.md)|<span data-ttu-id="f147a-114">Наследуется от [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="f147a-114">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="f147a-115">Не установлено, так как приложения не могут реагировать на сообщения.</span><span class="sxs-lookup"><span data-stu-id="f147a-115">Not set because applications can't react to messages.</span></span>|
|<span data-ttu-id="f147a-116">device;</span><span class="sxs-lookup"><span data-stu-id="f147a-116">device</span></span>|[<span data-ttu-id="f147a-117">identity</span><span class="sxs-lookup"><span data-stu-id="f147a-117">identity</span></span>](../resources/identity.md)|<span data-ttu-id="f147a-118">Наследуется от [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="f147a-118">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="f147a-119">Не установлено, так как устройства не могут реагировать на сообщения.</span><span class="sxs-lookup"><span data-stu-id="f147a-119">Not set because devices can't react to messages.</span></span>|
|<span data-ttu-id="f147a-120">user</span><span class="sxs-lookup"><span data-stu-id="f147a-120">user</span></span>|[<span data-ttu-id="f147a-121">identity</span><span class="sxs-lookup"><span data-stu-id="f147a-121">identity</span></span>](../resources/identity.md)|<span data-ttu-id="f147a-122">Наследуется от [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="f147a-122">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="f147a-123">Сведения о пользователе, который отреагировал на сообщение.</span><span class="sxs-lookup"><span data-stu-id="f147a-123">Details about the user who reacted to the message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f147a-124">Связи</span><span class="sxs-lookup"><span data-stu-id="f147a-124">Relationships</span></span>
<span data-ttu-id="f147a-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f147a-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f147a-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f147a-126">JSON representation</span></span>
<span data-ttu-id="f147a-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f147a-127">The following is a JSON representation of the resource.</span></span>
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

