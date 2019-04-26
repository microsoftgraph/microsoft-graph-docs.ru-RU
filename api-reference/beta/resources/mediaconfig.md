---
title: Тип ресурса Медиаконфиг
description: Конфигурация мультимедиа, используемая для подключения к вызову.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: aa8ec08ce5f4092a8f3d8c89af4a405d3a5c347d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342676"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="f1fb3-103">Тип ресурса Медиаконфиг</span><span class="sxs-lookup"><span data-stu-id="f1fb3-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1fb3-104">Конфигурация мультимедиа, используемая для подключения к вызову.</span><span class="sxs-lookup"><span data-stu-id="f1fb3-104">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="f1fb3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1fb3-105">Properties</span></span>

| <span data-ttu-id="f1fb3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1fb3-106">Property</span></span>       | <span data-ttu-id="f1fb3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f1fb3-107">Type</span></span>    | <span data-ttu-id="f1fb3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f1fb3-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f1fb3-109">Ремовефромдефаултаудиограуп</span><span class="sxs-lookup"><span data-stu-id="f1fb3-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="f1fb3-110">Логический</span><span class="sxs-lookup"><span data-stu-id="f1fb3-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="f1fb3-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1fb3-111">JSON representation</span></span>

<span data-ttu-id="f1fb3-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1fb3-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
   ],
  "abstract": true,
  "@odata.type": "microsoft.graph.mediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
