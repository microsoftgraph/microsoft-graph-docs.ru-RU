---
title: Тип ресурса Медиастреам
description: Тип Медиастреам.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 69d8088ba161bdf4dbf0482fdab8ad757347126d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342620"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="64811-103">Тип ресурса Медиастреам</span><span class="sxs-lookup"><span data-stu-id="64811-103">mediaStream resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64811-104">Тип Медиастреам.</span><span class="sxs-lookup"><span data-stu-id="64811-104">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="64811-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="64811-105">Properties</span></span>

| <span data-ttu-id="64811-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="64811-106">Property</span></span>    | <span data-ttu-id="64811-107">Тип</span><span class="sxs-lookup"><span data-stu-id="64811-107">Type</span></span>    | <span data-ttu-id="64811-108">Описание</span><span class="sxs-lookup"><span data-stu-id="64811-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="64811-109">direction</span><span class="sxs-lookup"><span data-stu-id="64811-109">direction</span></span>   | <span data-ttu-id="64811-110">String</span><span class="sxs-lookup"><span data-stu-id="64811-110">String</span></span>  | <span data-ttu-id="64811-111">Направление.</span><span class="sxs-lookup"><span data-stu-id="64811-111">The direction.</span></span> <span data-ttu-id="64811-112">`inactive`Возможные значения: `sendOnly`,, `receiveOnly`,. `sendReceive`</span><span class="sxs-lookup"><span data-stu-id="64811-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="64811-113">label</span><span class="sxs-lookup"><span data-stu-id="64811-113">label</span></span>       | <span data-ttu-id="64811-114">String</span><span class="sxs-lookup"><span data-stu-id="64811-114">String</span></span>  | <span data-ttu-id="64811-115">Метка потока мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="64811-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="64811-116">mediaType</span><span class="sxs-lookup"><span data-stu-id="64811-116">mediaType</span></span>   | <span data-ttu-id="64811-117">String</span><span class="sxs-lookup"><span data-stu-id="64811-117">String</span></span>  | <span data-ttu-id="64811-118">Тип мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="64811-118">The media type.</span></span> <span data-ttu-id="64811-119">Возможные `unknown`значения:, `audio` `video`,, `videoBasedScreenSharing`,. `data`</span><span class="sxs-lookup"><span data-stu-id="64811-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="64811-120">Сервермутед</span><span class="sxs-lookup"><span data-stu-id="64811-120">serverMuted</span></span> | <span data-ttu-id="64811-121">Логический</span><span class="sxs-lookup"><span data-stu-id="64811-121">Boolean</span></span> | <span data-ttu-id="64811-122">Если сервер отключен на носителе.</span><span class="sxs-lookup"><span data-stu-id="64811-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="64811-123">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="64811-123">sourceId</span></span>    | <span data-ttu-id="64811-124">String</span><span class="sxs-lookup"><span data-stu-id="64811-124">String</span></span>  | <span data-ttu-id="64811-125">Идентификатор источника.</span><span class="sxs-lookup"><span data-stu-id="64811-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="64811-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64811-126">JSON representation</span></span>

<span data-ttu-id="64811-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64811-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted"
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

## <a name="example"></a><span data-ttu-id="64811-128">Пример</span><span class="sxs-lookup"><span data-stu-id="64811-128">Example</span></span>

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
