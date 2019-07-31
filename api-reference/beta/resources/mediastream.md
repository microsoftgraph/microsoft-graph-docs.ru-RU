---
title: Тип ресурса Медиастреам
description: Тип Медиастреам.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c39c4eb0754f327361fec04852293ef084b0c412
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966829"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="3f3dc-103">Тип ресурса Медиастреам</span><span class="sxs-lookup"><span data-stu-id="3f3dc-103">mediaStream resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f3dc-104">Тип Медиастреам.</span><span class="sxs-lookup"><span data-stu-id="3f3dc-104">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="3f3dc-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f3dc-105">Properties</span></span>

| <span data-ttu-id="3f3dc-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f3dc-106">Property</span></span>    | <span data-ttu-id="3f3dc-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3f3dc-107">Type</span></span>    | <span data-ttu-id="3f3dc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3f3dc-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="3f3dc-109">direction</span><span class="sxs-lookup"><span data-stu-id="3f3dc-109">direction</span></span>   | <span data-ttu-id="3f3dc-110">String</span><span class="sxs-lookup"><span data-stu-id="3f3dc-110">String</span></span>  | <span data-ttu-id="3f3dc-111">Направление.</span><span class="sxs-lookup"><span data-stu-id="3f3dc-111">The direction.</span></span> <span data-ttu-id="3f3dc-112">`inactive`Возможные значения: `sendOnly`,, `receiveOnly`,. `sendReceive`</span><span class="sxs-lookup"><span data-stu-id="3f3dc-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="3f3dc-113">label</span><span class="sxs-lookup"><span data-stu-id="3f3dc-113">label</span></span>       | <span data-ttu-id="3f3dc-114">String</span><span class="sxs-lookup"><span data-stu-id="3f3dc-114">String</span></span>  | <span data-ttu-id="3f3dc-115">Метка потока мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="3f3dc-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="3f3dc-116">mediaType</span><span class="sxs-lookup"><span data-stu-id="3f3dc-116">mediaType</span></span>   | <span data-ttu-id="3f3dc-117">String</span><span class="sxs-lookup"><span data-stu-id="3f3dc-117">String</span></span>  | <span data-ttu-id="3f3dc-118">Тип мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="3f3dc-118">The media type.</span></span> <span data-ttu-id="3f3dc-119">Возможные `unknown`значения:, `audio` `video`,, `videoBasedScreenSharing`,. `data`</span><span class="sxs-lookup"><span data-stu-id="3f3dc-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="3f3dc-120">Сервермутед</span><span class="sxs-lookup"><span data-stu-id="3f3dc-120">serverMuted</span></span> | <span data-ttu-id="3f3dc-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f3dc-121">Boolean</span></span> | <span data-ttu-id="3f3dc-122">Если сервер отключен на носителе.</span><span class="sxs-lookup"><span data-stu-id="3f3dc-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="3f3dc-123">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="3f3dc-123">sourceId</span></span>    | <span data-ttu-id="3f3dc-124">String</span><span class="sxs-lookup"><span data-stu-id="3f3dc-124">String</span></span>  | <span data-ttu-id="3f3dc-125">Идентификатор источника.</span><span class="sxs-lookup"><span data-stu-id="3f3dc-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="3f3dc-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f3dc-126">JSON representation</span></span>

<span data-ttu-id="3f3dc-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f3dc-127">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="3f3dc-128">Пример</span><span class="sxs-lookup"><span data-stu-id="3f3dc-128">Example</span></span>

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
