---
title: Тип ресурса Медиастреам
description: Содержит сведения о канале мультимедиа.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8d6bce42c31e39f5b36e3beccdac2fc660f9cb30
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522759"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="7bfa9-103">Тип ресурса Медиастреам</span><span class="sxs-lookup"><span data-stu-id="7bfa9-103">mediaStream resource type</span></span>

<span data-ttu-id="7bfa9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bfa9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bfa9-105">Содержит сведения о канале мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="7bfa9-105">Contains information about the media channel.</span></span>

## <a name="properties"></a><span data-ttu-id="7bfa9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7bfa9-106">Properties</span></span>

| <span data-ttu-id="7bfa9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bfa9-107">Property</span></span>    | <span data-ttu-id="7bfa9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7bfa9-108">Type</span></span>    | <span data-ttu-id="7bfa9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7bfa9-109">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="7bfa9-110">direction</span><span class="sxs-lookup"><span data-stu-id="7bfa9-110">direction</span></span>   | <span data-ttu-id="7bfa9-111">String</span><span class="sxs-lookup"><span data-stu-id="7bfa9-111">String</span></span>  | <span data-ttu-id="7bfa9-112">Направление.</span><span class="sxs-lookup"><span data-stu-id="7bfa9-112">The direction.</span></span> <span data-ttu-id="7bfa9-113">`inactive`Возможные значения: `sendOnly`,, `receiveOnly`,. `sendReceive`</span><span class="sxs-lookup"><span data-stu-id="7bfa9-113">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="7bfa9-114">label</span><span class="sxs-lookup"><span data-stu-id="7bfa9-114">label</span></span>       | <span data-ttu-id="7bfa9-115">String</span><span class="sxs-lookup"><span data-stu-id="7bfa9-115">String</span></span>  | <span data-ttu-id="7bfa9-116">Метка потока мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="7bfa9-116">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="7bfa9-117">mediaType</span><span class="sxs-lookup"><span data-stu-id="7bfa9-117">mediaType</span></span>   | <span data-ttu-id="7bfa9-118">String</span><span class="sxs-lookup"><span data-stu-id="7bfa9-118">String</span></span>  | <span data-ttu-id="7bfa9-119">Тип мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="7bfa9-119">The media type.</span></span> <span data-ttu-id="7bfa9-120">Возможные `unknown`значения:, `audio` `video`,, `videoBasedScreenSharing`,. `data`</span><span class="sxs-lookup"><span data-stu-id="7bfa9-120">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="7bfa9-121">сервермутед</span><span class="sxs-lookup"><span data-stu-id="7bfa9-121">serverMuted</span></span> | <span data-ttu-id="7bfa9-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="7bfa9-122">Boolean</span></span> | <span data-ttu-id="7bfa9-123">Указывает, отключен ли сервер к мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="7bfa9-123">Indicates whether the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="7bfa9-124">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="7bfa9-124">sourceId</span></span>    | <span data-ttu-id="7bfa9-125">String</span><span class="sxs-lookup"><span data-stu-id="7bfa9-125">String</span></span>  | <span data-ttu-id="7bfa9-126">Идентификатор источника.</span><span class="sxs-lookup"><span data-stu-id="7bfa9-126">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="7bfa9-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7bfa9-127">JSON representation</span></span>

<span data-ttu-id="7bfa9-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bfa9-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted",
    "label"
  ],
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "inactive | sendOnly | receiveOnly | sendReceive",
  "label": "String",
  "mediaType": "unknown | audio | video | videoBasedScreenSharing | data",
  "serverMuted": true,
  "sourceId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
