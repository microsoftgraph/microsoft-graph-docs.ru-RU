---
title: Тип ресурса Медиастреам
description: Тип Медиастреам.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 906eccc7004aaac26dc29948e51e42cfd5e86631
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866266"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="8efc0-103">Тип ресурса Медиастреам</span><span class="sxs-lookup"><span data-stu-id="8efc0-103">mediaStream resource type</span></span>

<span data-ttu-id="8efc0-104">Содержит сведения о канале мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="8efc0-104">This contains information about the media channel.</span></span>

## <a name="properties"></a><span data-ttu-id="8efc0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8efc0-105">Properties</span></span>

| <span data-ttu-id="8efc0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8efc0-106">Property</span></span>    | <span data-ttu-id="8efc0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8efc0-107">Type</span></span>    | <span data-ttu-id="8efc0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8efc0-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="8efc0-109">direction</span><span class="sxs-lookup"><span data-stu-id="8efc0-109">direction</span></span>   | <span data-ttu-id="8efc0-110">String</span><span class="sxs-lookup"><span data-stu-id="8efc0-110">String</span></span>  | <span data-ttu-id="8efc0-111">Направление.</span><span class="sxs-lookup"><span data-stu-id="8efc0-111">The direction.</span></span> <span data-ttu-id="8efc0-112">`inactive`Возможные значения: `sendOnly`,, `receiveOnly`,. `sendReceive`</span><span class="sxs-lookup"><span data-stu-id="8efc0-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="8efc0-113">label</span><span class="sxs-lookup"><span data-stu-id="8efc0-113">label</span></span>       | <span data-ttu-id="8efc0-114">String</span><span class="sxs-lookup"><span data-stu-id="8efc0-114">String</span></span>  | <span data-ttu-id="8efc0-115">Метка потока мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="8efc0-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="8efc0-116">mediaType</span><span class="sxs-lookup"><span data-stu-id="8efc0-116">mediaType</span></span>   | <span data-ttu-id="8efc0-117">String</span><span class="sxs-lookup"><span data-stu-id="8efc0-117">String</span></span>  | <span data-ttu-id="8efc0-118">Тип мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="8efc0-118">The media type.</span></span> <span data-ttu-id="8efc0-119">Возможные `unknown`значения:, `audio` `video`,, `videoBasedScreenSharing`,. `data`</span><span class="sxs-lookup"><span data-stu-id="8efc0-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="8efc0-120">сервермутед</span><span class="sxs-lookup"><span data-stu-id="8efc0-120">serverMuted</span></span> | <span data-ttu-id="8efc0-121">Логический</span><span class="sxs-lookup"><span data-stu-id="8efc0-121">Boolean</span></span> | <span data-ttu-id="8efc0-122">Если сервер отключен на носителе.</span><span class="sxs-lookup"><span data-stu-id="8efc0-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="8efc0-123">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="8efc0-123">sourceId</span></span>    | <span data-ttu-id="8efc0-124">String</span><span class="sxs-lookup"><span data-stu-id="8efc0-124">String</span></span>  | <span data-ttu-id="8efc0-125">Идентификатор источника.</span><span class="sxs-lookup"><span data-stu-id="8efc0-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="8efc0-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8efc0-126">JSON representation</span></span>

<span data-ttu-id="8efc0-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8efc0-127">The following is a JSON representation of the resource.</span></span>

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
