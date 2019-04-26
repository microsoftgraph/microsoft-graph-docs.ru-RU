---
title: Тип ресурса Номедиаконфиг
description: Конфигурация мультимедиа, указывающая на отсутствие носителя.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ec1c70e233f46ad0098a6a7ee76d4d46f3b82c20
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342158"
---
# <a name="nomediaconfig-resource-type"></a><span data-ttu-id="f88a7-103">Тип ресурса Номедиаконфиг</span><span class="sxs-lookup"><span data-stu-id="f88a7-103">noMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f88a7-104">Конфигурация мультимедиа, указывающая на отсутствие носителя.</span><span class="sxs-lookup"><span data-stu-id="f88a7-104">Media configuration for indicating no media.</span></span>

## <a name="properties"></a><span data-ttu-id="f88a7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f88a7-105">Properties</span></span>

| <span data-ttu-id="f88a7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f88a7-106">Property</span></span>       | <span data-ttu-id="f88a7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f88a7-107">Type</span></span>    | <span data-ttu-id="f88a7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f88a7-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f88a7-109">Ремовефромдефаултаудиограуп</span><span class="sxs-lookup"><span data-stu-id="f88a7-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="f88a7-110">Логический</span><span class="sxs-lookup"><span data-stu-id="f88a7-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="f88a7-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f88a7-111">JSON representation</span></span>

<span data-ttu-id="f88a7-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f88a7-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.noMediaConfig"
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
  "description": "noMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
