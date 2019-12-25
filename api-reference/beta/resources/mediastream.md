---
title: Тип ресурса Медиастреам
description: Содержит сведения о канале мультимедиа.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: de5c90453d9adb657c2df5ee761d847056664037
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870182"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="24443-103">Тип ресурса Медиастреам</span><span class="sxs-lookup"><span data-stu-id="24443-103">mediaStream resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24443-104">Содержит сведения о канале мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="24443-104">Contains information about the media channel.</span></span>

## <a name="properties"></a><span data-ttu-id="24443-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="24443-105">Properties</span></span>

| <span data-ttu-id="24443-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="24443-106">Property</span></span>    | <span data-ttu-id="24443-107">Тип</span><span class="sxs-lookup"><span data-stu-id="24443-107">Type</span></span>    | <span data-ttu-id="24443-108">Описание</span><span class="sxs-lookup"><span data-stu-id="24443-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="24443-109">direction</span><span class="sxs-lookup"><span data-stu-id="24443-109">direction</span></span>   | <span data-ttu-id="24443-110">String</span><span class="sxs-lookup"><span data-stu-id="24443-110">String</span></span>  | <span data-ttu-id="24443-111">Направление.</span><span class="sxs-lookup"><span data-stu-id="24443-111">The direction.</span></span> <span data-ttu-id="24443-112">`inactive`Возможные значения: `sendOnly`,, `receiveOnly`,. `sendReceive`</span><span class="sxs-lookup"><span data-stu-id="24443-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="24443-113">label</span><span class="sxs-lookup"><span data-stu-id="24443-113">label</span></span>       | <span data-ttu-id="24443-114">String</span><span class="sxs-lookup"><span data-stu-id="24443-114">String</span></span>  | <span data-ttu-id="24443-115">Метка потока мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="24443-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="24443-116">mediaType</span><span class="sxs-lookup"><span data-stu-id="24443-116">mediaType</span></span>   | <span data-ttu-id="24443-117">String</span><span class="sxs-lookup"><span data-stu-id="24443-117">String</span></span>  | <span data-ttu-id="24443-118">Тип мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="24443-118">The media type.</span></span> <span data-ttu-id="24443-119">Возможные `unknown`значения:, `audio` `video`,, `videoBasedScreenSharing`,. `data`</span><span class="sxs-lookup"><span data-stu-id="24443-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="24443-120">сервермутед</span><span class="sxs-lookup"><span data-stu-id="24443-120">serverMuted</span></span> | <span data-ttu-id="24443-121">Логический</span><span class="sxs-lookup"><span data-stu-id="24443-121">Boolean</span></span> | <span data-ttu-id="24443-122">Указывает, отключен ли сервер к мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="24443-122">Indicates whether the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="24443-123">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="24443-123">sourceId</span></span>    | <span data-ttu-id="24443-124">String</span><span class="sxs-lookup"><span data-stu-id="24443-124">String</span></span>  | <span data-ttu-id="24443-125">Идентификатор источника.</span><span class="sxs-lookup"><span data-stu-id="24443-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="24443-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24443-126">JSON representation</span></span>

<span data-ttu-id="24443-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24443-127">The following is a JSON representation of the resource.</span></span>

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
