---
title: тип ресурса chatViewpoint
description: Представляет пользовательские свойства чата.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca6a542903aae7b203c6183a25dd99889b97f275
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236327"
---
# <a name="chatviewpoint-resource-type"></a><span data-ttu-id="69596-103">тип ресурса chatViewpoint</span><span class="sxs-lookup"><span data-stu-id="69596-103">chatViewpoint resource type</span></span>

<span data-ttu-id="69596-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69596-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69596-105">Представляет пользовательские свойства [чата.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="69596-105">Represents user-specific properties of a [chat](../resources/chat.md).</span></span> <span data-ttu-id="69596-106">Эти свойства могут изменяться в зависимости от того, кто является звонивцом API.</span><span class="sxs-lookup"><span data-stu-id="69596-106">These properties might change based on who the caller of the API is.</span></span>

> <span data-ttu-id="69596-107">**Примечание:** В настоящее время [только операция чатов](../api/chat-list.md) списка поддерживает **chatViewpoint.**</span><span class="sxs-lookup"><span data-stu-id="69596-107">**Note:** Currently, only the [list chats](../api/chat-list.md) operation supports **chatViewpoint**.</span></span>

## <a name="properties"></a><span data-ttu-id="69596-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="69596-108">Properties</span></span>
|<span data-ttu-id="69596-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="69596-109">Property</span></span>|<span data-ttu-id="69596-110">Тип</span><span class="sxs-lookup"><span data-stu-id="69596-110">Type</span></span>|<span data-ttu-id="69596-111">Описание</span><span class="sxs-lookup"><span data-stu-id="69596-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69596-112">lastMessageReadDateTime</span><span class="sxs-lookup"><span data-stu-id="69596-112">lastMessageReadDateTime</span></span>|<span data-ttu-id="69596-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69596-113">DateTimeOffset</span></span>|<span data-ttu-id="69596-114">Представляет dateTime до тех пор, пока пользователь звонка не прочитал [chatMessages в](../resources/chatmessage.md) определенном чате.</span><span class="sxs-lookup"><span data-stu-id="69596-114">Represents the dateTime up until which the calling user has read [chatMessages](../resources/chatmessage.md) in a specific chat.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69596-115">Связи</span><span class="sxs-lookup"><span data-stu-id="69596-115">Relationships</span></span>
<span data-ttu-id="69596-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="69596-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="69596-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="69596-117">JSON representation</span></span>
<span data-ttu-id="69596-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69596-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatViewpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatViewpoint",
  "lastMessageReadDateTime": "String (timestamp)"
}
```

