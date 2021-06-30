---
title: тип ресурса chatMessageFromIdentitySet
description: Представляет отправитель сообщения в чате или канале.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6f200e5dcaf3c722dc3e185fc1e12946f7ad1151
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211316"
---
# <a name="chatmessagefromidentityset-resource-type"></a><span data-ttu-id="daea5-103">тип ресурса chatMessageFromIdentitySet</span><span class="sxs-lookup"><span data-stu-id="daea5-103">chatMessageFromIdentitySet resource type</span></span>

<span data-ttu-id="daea5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daea5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daea5-105">Представляет отправитель сообщения [в](../resources/chatmessage.md) чате или канале.</span><span class="sxs-lookup"><span data-stu-id="daea5-105">Represents the sender of a [message](../resources/chatmessage.md) in a chat or a channel.</span></span> <span data-ttu-id="daea5-106">Этот объект может быть для сообщения, которое было удалено или отправлено внутренней системой Microsoft Teams, например для сообщений событий для добавления `null` участников.</span><span class="sxs-lookup"><span data-stu-id="daea5-106">This object may be `null` for a message that has been deleted or sent by the Microsoft Teams internal system; for example, event messages for addition of members.</span></span>


<span data-ttu-id="daea5-107">Наследует от [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="daea5-107">Inherits from [identitySet](../resources/identityset.md).</span></span>

## <a name="properties"></a><span data-ttu-id="daea5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="daea5-108">Properties</span></span>
|<span data-ttu-id="daea5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="daea5-109">Property</span></span>|<span data-ttu-id="daea5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="daea5-110">Type</span></span>|<span data-ttu-id="daea5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="daea5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daea5-112">application</span><span class="sxs-lookup"><span data-stu-id="daea5-112">application</span></span>|[<span data-ttu-id="daea5-113">identity</span><span class="sxs-lookup"><span data-stu-id="daea5-113">identity</span></span>](../resources/identity.md)|<span data-ttu-id="daea5-114">Наследуется от [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="daea5-114">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="daea5-115">При этом представляет приложение (например, бот), отправив сообщение.</span><span class="sxs-lookup"><span data-stu-id="daea5-115">If present, represents the application (for example, bot) that sent the message.</span></span>|
|<span data-ttu-id="daea5-116">device;</span><span class="sxs-lookup"><span data-stu-id="daea5-116">device</span></span>|[<span data-ttu-id="daea5-117">identity</span><span class="sxs-lookup"><span data-stu-id="daea5-117">identity</span></span>](../resources/identity.md)|<span data-ttu-id="daea5-118">Наследуется от [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="daea5-118">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="daea5-119">Не используется.</span><span class="sxs-lookup"><span data-stu-id="daea5-119">Not used.</span></span>|
|<span data-ttu-id="daea5-120">user</span><span class="sxs-lookup"><span data-stu-id="daea5-120">user</span></span>|[<span data-ttu-id="daea5-121">identity</span><span class="sxs-lookup"><span data-stu-id="daea5-121">identity</span></span>](../resources/identity.md)|<span data-ttu-id="daea5-122">Наследуется от [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="daea5-122">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="daea5-123">Если присутствует, представляет пользователя, отправив сообщение.</span><span class="sxs-lookup"><span data-stu-id="daea5-123">If present, represents the user that sent the message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="daea5-124">Связи</span><span class="sxs-lookup"><span data-stu-id="daea5-124">Relationships</span></span>
<span data-ttu-id="daea5-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="daea5-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="daea5-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="daea5-126">JSON representation</span></span>
<span data-ttu-id="daea5-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="daea5-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageFromIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageFromIdentitySet",
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

