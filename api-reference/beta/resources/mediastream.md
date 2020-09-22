---
title: Тип ресурса Медиастреам
description: Содержит сведения о канале мультимедиа.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 37ed8ce10f62888a7bf1be67f489c6b8a0b95c76
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971736"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="69f83-103">Тип ресурса Медиастреам</span><span class="sxs-lookup"><span data-stu-id="69f83-103">mediaStream resource type</span></span>

<span data-ttu-id="69f83-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69f83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69f83-105">Содержит сведения о канале мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="69f83-105">Contains information about the media channel.</span></span>

## <a name="properties"></a><span data-ttu-id="69f83-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="69f83-106">Properties</span></span>

| <span data-ttu-id="69f83-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="69f83-107">Property</span></span>    | <span data-ttu-id="69f83-108">Тип</span><span class="sxs-lookup"><span data-stu-id="69f83-108">Type</span></span>    | <span data-ttu-id="69f83-109">Описание</span><span class="sxs-lookup"><span data-stu-id="69f83-109">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="69f83-110">direction</span><span class="sxs-lookup"><span data-stu-id="69f83-110">direction</span></span>   | <span data-ttu-id="69f83-111">String</span><span class="sxs-lookup"><span data-stu-id="69f83-111">String</span></span>  | <span data-ttu-id="69f83-112">Направление.</span><span class="sxs-lookup"><span data-stu-id="69f83-112">The direction.</span></span> <span data-ttu-id="69f83-113">Возможные значения: `inactive` ,, `sendOnly` `receiveOnly` , `sendReceive` .</span><span class="sxs-lookup"><span data-stu-id="69f83-113">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="69f83-114">label</span><span class="sxs-lookup"><span data-stu-id="69f83-114">label</span></span>       | <span data-ttu-id="69f83-115">String</span><span class="sxs-lookup"><span data-stu-id="69f83-115">String</span></span>  | <span data-ttu-id="69f83-116">Метка потока мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="69f83-116">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="69f83-117">MediaType</span><span class="sxs-lookup"><span data-stu-id="69f83-117">mediaType</span></span>   | <span data-ttu-id="69f83-118">String</span><span class="sxs-lookup"><span data-stu-id="69f83-118">String</span></span>  | <span data-ttu-id="69f83-119">Тип мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="69f83-119">The media type.</span></span> <span data-ttu-id="69f83-120">Возможные значения:,,, `unknown` `audio` `video` `videoBasedScreenSharing` , `data` .</span><span class="sxs-lookup"><span data-stu-id="69f83-120">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="69f83-121">сервермутед</span><span class="sxs-lookup"><span data-stu-id="69f83-121">serverMuted</span></span> | <span data-ttu-id="69f83-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="69f83-122">Boolean</span></span> | <span data-ttu-id="69f83-123">Указывает, отключен ли сервер к мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="69f83-123">Indicates whether the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="69f83-124">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="69f83-124">sourceId</span></span>    | <span data-ttu-id="69f83-125">String</span><span class="sxs-lookup"><span data-stu-id="69f83-125">String</span></span>  | <span data-ttu-id="69f83-126">Идентификатор источника.</span><span class="sxs-lookup"><span data-stu-id="69f83-126">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="69f83-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69f83-127">JSON representation</span></span>

<span data-ttu-id="69f83-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69f83-128">The following is a JSON representation of the resource.</span></span>

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


