---
title: Тип ресурса Медиастреам
description: Тип Медиастреам.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 63fad1d064c4ab967bba6df8bed6dbcdd20a3d69
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006657"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="c7fee-103">Тип ресурса Медиастреам</span><span class="sxs-lookup"><span data-stu-id="c7fee-103">mediaStream resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7fee-104">Тип Медиастреам.</span><span class="sxs-lookup"><span data-stu-id="c7fee-104">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="c7fee-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7fee-105">Properties</span></span>

| <span data-ttu-id="c7fee-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7fee-106">Property</span></span>    | <span data-ttu-id="c7fee-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c7fee-107">Type</span></span>    | <span data-ttu-id="c7fee-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c7fee-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="c7fee-109">direction</span><span class="sxs-lookup"><span data-stu-id="c7fee-109">direction</span></span>   | <span data-ttu-id="c7fee-110">String</span><span class="sxs-lookup"><span data-stu-id="c7fee-110">String</span></span>  | <span data-ttu-id="c7fee-111">Направление.</span><span class="sxs-lookup"><span data-stu-id="c7fee-111">The direction.</span></span> <span data-ttu-id="c7fee-112">`inactive`Возможные значения: `sendOnly`,, `receiveOnly`,. `sendReceive`</span><span class="sxs-lookup"><span data-stu-id="c7fee-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="c7fee-113">label</span><span class="sxs-lookup"><span data-stu-id="c7fee-113">label</span></span>       | <span data-ttu-id="c7fee-114">String</span><span class="sxs-lookup"><span data-stu-id="c7fee-114">String</span></span>  | <span data-ttu-id="c7fee-115">Метка потока мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="c7fee-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="c7fee-116">mediaType</span><span class="sxs-lookup"><span data-stu-id="c7fee-116">mediaType</span></span>   | <span data-ttu-id="c7fee-117">String</span><span class="sxs-lookup"><span data-stu-id="c7fee-117">String</span></span>  | <span data-ttu-id="c7fee-118">Тип мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="c7fee-118">The media type.</span></span> <span data-ttu-id="c7fee-119">Возможные `unknown`значения:, `audio` `video`,, `videoBasedScreenSharing`,. `data`</span><span class="sxs-lookup"><span data-stu-id="c7fee-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="c7fee-120">сервермутед</span><span class="sxs-lookup"><span data-stu-id="c7fee-120">serverMuted</span></span> | <span data-ttu-id="c7fee-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7fee-121">Boolean</span></span> | <span data-ttu-id="c7fee-122">Если сервер отключен на носителе.</span><span class="sxs-lookup"><span data-stu-id="c7fee-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="c7fee-123">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="c7fee-123">sourceId</span></span>    | <span data-ttu-id="c7fee-124">String</span><span class="sxs-lookup"><span data-stu-id="c7fee-124">String</span></span>  | <span data-ttu-id="c7fee-125">Идентификатор источника.</span><span class="sxs-lookup"><span data-stu-id="c7fee-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="c7fee-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c7fee-126">JSON representation</span></span>

<span data-ttu-id="c7fee-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7fee-127">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="c7fee-128">Пример</span><span class="sxs-lookup"><span data-stu-id="c7fee-128">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "sendReceive",
  "label": "main-audio",
  "mediaType": "audio",
  "serverMuted": false,
  "sourceId": "1024"
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
