---
title: тип ресурсов channelIdentity
description: Представляет удостоверение канала в Microsoft Teams.
author: Kanaka
doc_type: resourcePageType
localization_priority: Normal
ms.prod: teamwork
ms.openlocfilehash: 866469745a4dd3aaf7b22c2a6710e327992e9fee
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582962"
---
# <a name="channelidentity-resource-type"></a><span data-ttu-id="b363a-103">тип ресурсов channelIdentity</span><span class="sxs-lookup"><span data-stu-id="b363a-103">channelIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="b363a-104">Содержит основные сведения об идентификации канала в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b363a-104">Contains basic identification information about a channel in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="b363a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b363a-105">Properties</span></span>

| <span data-ttu-id="b363a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b363a-106">Property</span></span>   | <span data-ttu-id="b363a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b363a-107">Type</span></span> |<span data-ttu-id="b363a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b363a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b363a-109">channelId</span><span class="sxs-lookup"><span data-stu-id="b363a-109">channelId</span></span>|<span data-ttu-id="b363a-110">string</span><span class="sxs-lookup"><span data-stu-id="b363a-110">string</span></span>|  <span data-ttu-id="b363a-111">Идентификатор канала, в котором было размещено сообщение.</span><span class="sxs-lookup"><span data-stu-id="b363a-111">The identity of the channel in which the message was posted.</span></span>|
|<span data-ttu-id="b363a-112">teamId</span><span class="sxs-lookup"><span data-stu-id="b363a-112">teamId</span></span>|<span data-ttu-id="b363a-113">string</span><span class="sxs-lookup"><span data-stu-id="b363a-113">string</span></span>|  <span data-ttu-id="b363a-114">Удостоверение группы, в которой было размещено сообщение.</span><span class="sxs-lookup"><span data-stu-id="b363a-114">The identity of the team in which the message was posted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b363a-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b363a-115">JSON representation</span></span>

<span data-ttu-id="b363a-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b363a-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    
  ],
  "@odata.type": "microsoft.graph.channelIdentity"
}-->

```json
{
  "channelId": "string",
  "teamId": "string",
  
}
```

<!-- uuid: 4DFA000D-1A5F-4299-B3DD-835E4DD2F3BF
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel identity  resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
